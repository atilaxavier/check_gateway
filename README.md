# check_gateway
Verifica PGW de onde vem conexão Surf, com base no IP publico do dispositivo, indicando se está no gateway de Santo Andre ou de Vila Anastacio.

IPs publicos:
SNE:
170.244.198.0/24
170.244.199.0/24
191.128.232.0/24
191.128.233.0/24
191.128.234.0/23
191.128.236.0/24
191.128.237.0/24

SPO:
189.76.168.0/22
189.76.170.0/24
189.76.172.0/23
189.76.174.0/24

IPs privados:
10.50.0.0/16 # IPs PGW SNE
10.140.0.0/16 # IP PGW SPO pela VPN
10.141.0.0/16 # IP PGW SPO Direct Connect

IPv4 Privado - SNE - ip-local-pool "private-pool-1" (Principal usado pela surf.br)

ipv4-prefix "10.1.0.0/16"
                ipv4-prefix "10.2.0.0/16"
                ipv4-prefix "10.3.0.0/16"
                ipv4-prefix "10.4.0.0/16"
                ipv4-prefix "10.5.0.0/16"
                ipv4-prefix "10.6.0.0/16"
                ipv4-prefix "10.7.0.0/16"
                ipv4-prefix "10.8.0.0/16"
                ipv4-prefix "10.9.0.0/16"
                ipv4-prefix "10.10.0.0/16"
                ipv4-prefix "10.11.0.0/16"
                ipv4-prefix "10.12.0.0/16"
                ipv4-prefix "10.13.0.0/16"
                ipv4-prefix "10.14.0.0/16"
                ipv4-prefix "10.15.0.0/16"
                ipv4-prefix "10.16.0.0/16"
                ipv4-prefix "10.17.0.0/16"
                ipv4-prefix "10.18.0.0/16"
                ipv4-prefix "10.19.0.0/16"
                ipv4-prefix "10.80.0.0/16"
                ipv4-prefix "10.81.0.0/16"
                ipv4-prefix "10.82.0.0/16"
                ipv4-prefix "10.83.0.0/16"
                ipv4-prefix "10.84.0.0/16"
                ipv4-prefix "10.85.0.0/16"
                ipv4-prefix "10.86.0.0/16"
                ipv4-prefix "10.87.0.0/16"
                ipv4-prefix "10.88.0.0/16"
                ipv4-prefix "10.89.0.0/16"

ip-local-pool "IP-POOL-IPV6" (principal, usado pela surf.br)
                reserved-ip-list "IPVSEIS"
                ipv6-prefix "2804:38c4::/48"
                ipv6-prefix "2804:38c4:2::/48"
                ipv6-prefix "2804:38c4:3::/48"
                ipv6-prefix "2804:38c4:4::/48"
                ipv6-prefix "2804:38c4:5::/48"
                ipv6-prefix "2804:38c4:6::/48"
                ipv6-prefix "2804:38c4:7::/48"
                ipv6-prefix "2804:38c4:8::/48"
                ipv6-prefix "2804:38c4:9::/48"
                ipv6-prefix "2804:38c4:10::/48"
                ipv6-prefix "2804:38c4:11::/48"
                ipv6-prefix "2804:38c4:12::/48"
                ipv6-prefix "2804:38c4:13::/48"
                ipv6-prefix "2804:38c4:14::/48"
                ipv6-prefix "2804:38c4:15::/48"
                ipv6-prefix "2804:38c4:16::/48"
                ipv6-prefix "2804:38c4:17::/48"
                ipv6-prefix "2804:38c4:18::/48"
                ipv6-prefix "2804:38c4:19::/48"
                ipv6-prefix "2804:38c4:20::/48"

        
IPv4 Privado - SPO-

 ip-local-pool "private-pool-1" (Principal usado pela surf.br)
ipv4-prefix "10.100.0.0/16"
                ipv4-prefix "10.101.0.0/16"
                ipv4-prefix "10.102.0.0/16"
                ipv4-prefix "10.103.0.0/16"
                ipv4-prefix "10.104.0.0/16"
                ipv4-prefix "10.105.0.0/16"
                ipv4-prefix "10.106.0.0/16"
                ipv4-prefix "10.107.0.0/16"
                ipv4-prefix "10.108.0.0/16"
                ipv4-prefix "10.109.0.0/16"
                ipv4-prefix "10.170.0.0/16"
                ipv4-prefix "10.171.0.0/16"
                ipv4-prefix "10.172.0.0/16"
                ipv4-prefix "10.173.0.0/16"
                ipv4-prefix "10.174.0.0/16"
                ipv4-prefix "10.175.0.0/16"
                ipv4-prefix "10.176.0.0/16"
                ipv4-prefix "10.177.0.0/16"
                ipv4-prefix "10.178.0.0/16"
                ipv4-prefix "10.179.0.0/16"

ip-local-pool "IP-POOL-IPV6" (principal, usado pela surf.br)
                reserved-ip-list "IPVSEIS"
              ipv6-prefix "2804:748::/48"
                ipv6-prefix "2804:748:1::/48"
                ipv6-prefix "2804:748:2::/48"
                ipv6-prefix "2804:748:3::/48"
                ipv6-prefix "2804:748:4::/48"
                ipv6-prefix "2804:748:5::/48"
                ipv6-prefix "2804:748:6::/48"
                ipv6-prefix "2804:748:7::/48"
                ipv6-prefix "2804:748:8::/48"
                ipv6-prefix "2804:748:9::/48"


