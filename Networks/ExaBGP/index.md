Запуск exabgp:

server# exabgp config.conf

cat config.conf

neighbor 192.168.127.128 { 

  description "a quagga test peer"; 

  router-id 192.168.127.1; 

  local-address 192.168.127.1; 

  local-as 65000; 

  peer-as 65000; 

  graceful-restart; 

 

  static { 

    route 10.0.3.0/24 { 

      next-hop 10.0.255.254; 

      community [ 30740:30740 30740:0 ]; 

      local-preference 200; 

    } 

    route 10.0.5.0/24 next-hop 10.0.255.254 local-preference 200; 

  } 

  flow { 

    route slow-down-the-proxy-for-the-office { 

      match { 

        source 10.0.0.1/32; 

        destination 192.168.0.1/32; 

        destination-port >8080&<8088 =3128; 

        source-port >1024; 

        protocol tcp; 

      } 

      then { 

        rate-limit 9600; 

      } 

    }

    route drop_from_11_8 {

        match {

            source 11.0.0.0/8;

        }

        then {

            discard;

        }

    }

     

  } 

}