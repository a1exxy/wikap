CentOS7.3

cat /etc/vsftpd/vsftpd.conf

listen=YES

# делаем анонимный доступ, с правом записи

anonymous_enable=YES

no_anon_password=NO

anon_root=/home/ftp

anon_upload_enable=YES

anon_mkdir_write_enable=YES

anon_other_write_enable=YES

anon_umask=002

# разрешаем вход локальным пользователям

# с правом записи в домашних директориях

local_enable=YES

local_umask=002

write_enable=YES

local_root=/home/

passwd_chroot_enable=YES

# помещаем локальных юзеров в их домашние каталоги,

# иначе пользователю будет доступен корень системы.

chroot_local_user=YES

chroot_list_enable=NO

# настройки журналирования

#syslog_enable=YES

xferlog_std_format=NO

log_ftp_protocol=YES

xferlog_enable=YES

vsftpd_log_file=/var/log/vsftpd.log

pam_service_name=vsftpd

#allow_writable_root=YES

#

#guest_username=ftp

#guest_enable=YES