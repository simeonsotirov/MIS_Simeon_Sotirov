- gw, enp0s3 (WAN): DHCP, 10.0.2.15
- gw, enp0s8 (LAN1, Сливен): 10.210.0.1/24
- gw, enp0s9 (LAN2, Нова Загора): 10.211.0.1/24
- srv, enp0s3 (LAN1, Сливен): 10.210.0.10/24, gateway 10.210.0.1

Проверки

- srv към gw: ping 10.210.0.1 - 0% загуба
- gw към srv: ping 10.210.0.10 - 0% загуба
- gw към интернет: ping 8.8.8.8 - 0% загуба
- IP forwarding на gw: net.ipv4.ip_forward = 1
- snapshot Clean-TextileCraft на двете машини