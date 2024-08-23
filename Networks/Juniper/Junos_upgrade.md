file copy ftp://ftp:ftp@10.1.1.1/jinstall-ppc-11.4R2.15-export-signed.tgz    /var/tmp/jinstall-ppc-11.4R2.15-export-signed.tgz <br>

request system software add validate /var/tmp/jinstall-ppc-11.4R2.15-export-signed.tg

=========== mx960 upgrade =============

0) Copy software to temp dir

file copy ftp://ftp:ftp@10.1.1.1/junos-install-mx-x86-64-17.3R3.10.tgz    /var/tmp/junos-install-mx-x86-64-17.3R3.10.tgz

1) Delete redundancy

set chassis redundancy failover on-loss-of-keepalives

set chassis redundancy failover on-disk-failure

set chassis redundancy graceful-switchover

2) List temp dir and find correct software

file list /var/tmp/

3) upgrade backup RE

#Go to backup RE:

request routing-engine login backup 

#Check it:

> show chassis alarms 

error: Aborted! This command can only be used on the master routing engine.

# "show chassis alarms" is not working on the backup RE

request system software add validate /var/tmp/junos-install-mx-x86-64-17.3R3.10.tgz

# reboot backup RE:

request system reboot

4) Switchover !!!DROP TRAFFIC!!!

request chassis routing-engine master switch

5) Upgrade new backup RE

6)

request system snapshot re1

request system snapshot re0