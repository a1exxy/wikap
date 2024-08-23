Ubuntu 18.04:

apt install pmacct

service nfacctd start

root@pmacct:/etc/pmacct# cat nfacctd.conf 

! nfacctd configuration

!

!

!

daemonize: true

pidfile: /var/run/nfacctd.pid

syslog: daemon

!

! interested in in and outbound traffic

aggregate: src_host,dst_host

! on this network

!pcap_filter: net 127.0.0.0/8

!pcap_filter: net 192.168.1.0/24

! on this interface

interface: eth0

nfacctd_port: 1234

!

plugins: print

print_refresh_time: 300

!print_refresh_time: 900

print_output: csv

print_output_file: /root/PMACCT/ipfix-%Y%m%d-%H%M.csv

print_latest_file: /root/PMACCT/latest

!print_time_roundoff: m

! storage methods

!plugins: pgsql

!sql_host: localhost

!sql_passwd:

! refresh the db every minute

!sql_refresh_time: 60

! reduce the size of the insert/update clause

!sql_optimize_clauses: true

! accumulate values in each row for up to an hour

!sql_history: 1h

! create new rows on the minute, hour, day boundaries

!sql_history_roundoff: mhd

! in case of emergency, log to this file

!sql_recovery_logfile: /var/lib/pmacct/nfacctd_recovery_log