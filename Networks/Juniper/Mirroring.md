https://www.juniper.net/documentation/en_US/junos/topics/example/port-mirroring-local-ex-series.html

user@switch# show

ethernet-switching-options {

analyzer employee-monitor {

input {

ingress {

interface ge-0/0/0.0;

interface ge-0/0/1.0;

}

}

output {

interface {

ge-0/0/10.0;

}

}

}

}