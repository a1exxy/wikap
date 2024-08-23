#!/usr/bin/env bash

# Bash history tuning

add_to_bashrc(){

if [ -f $1 ]; then

sed -i 's/HISTSIZE=.*/HISTSIZE=100000/' $1

sed -i 's/HISTFILESIZE=.*/HISTFILESIZE=5000000/' $1

cat <<EOF >> $1 

shopt -s cmdhist

shopt -s histappend

HISTTIMEFORMAT='%F %T '

if ! [ -z \$PROMPT_COMMAND ]; then 

    PROMPT_COMMAND='\$PROMPT_COMMAND; history -a'; 

else 

    PROMPT_COMMAND='history -a'; 

fi

EOF

fi

}

for Home in $(ls -1 /home/); do 

    add_to_bashrc "/home/$Home/.bashrc"

done

add_to_bashrc "/root/.bashrc"

cat <<EOF > /etc/cron.daily/bash_history_backup

#!/usr/bin/env bash

CopyHist(){

if [ -f .bash_history ]; then

    cp -p .bash_history .bash_history_backup_last

    cp -p .bash_history_backup_last .bash_history_backup_\$(date +%F__%T)

fi

}

for Home in \$(ls -1 /home/); do 

        cd /home/\$Home || continue

        cmp -s .bash_history_backup_last .bash_history && continue

        CopyHist 

done

    cd /root

    cmp -s .bash_history_backup_last .bash_history && exit 0

    CopyHist 

EOF

chmod +x /etc/cron.daily/bash_history_backup