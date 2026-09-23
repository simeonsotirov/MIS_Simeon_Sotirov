Адреси
-gw, enp0s3 (WAN): DHCP, 10.0.2.15
-gw, enp0s8 (LAN1): 192.168.10.1/24
-gw, enp0s9 (LAN2): 192.168.20.1/24
-srv, enp0s3 (LAN1): 192.168.10.10/24, gateway 192.168.10.1

Проверкa
-srv към gw: ping 192.168.10.1 - 0% загуба
-gw към srv: ping 192.168.10.10 - 0% загуба
-gw към интернет: ping 8.8.8.8 - 0% загуба
-IP forwarding на gw: net.ipv4.ip_forward = 1