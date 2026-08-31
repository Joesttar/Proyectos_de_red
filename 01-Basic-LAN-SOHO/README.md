# Proyecto 1: Fundamentos de LAN y Aprendizaje de MAC

## Descripción
Este proyecto demuestra la implementación de una red de área local (LAN) básica siguiendo los conceptos de la capa de acceso de Cisco. Se configuró seguridad inicial en el switch y se verificó el funcionamiento de la tabla CAM (Content Addressable Memory).

## Conceptos Aplicados
- **Capa 2 (Enlace de Datos):** Direccionamiento físico mediante direcciones MAC.
- **Configuración de IOS:** Uso de hostnames, banners y contraseñas secretas.
- **Protocolo ICMP:** Verificación de conectividad mediante Ping.

## Topología
- 1 Switch Cisco 2960
- 3 PCs (Red 192.168.1.0/24)

## Verificación
Para verificar el aprendizaje del switch, se utilizó el comando:
`show mac address-table`