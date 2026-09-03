# Proyecto 3: Implementación de DHCP Server en Router Cisco

## Descripción
En este proyecto automaticé la asignación de direcciones IPv4 utilizando el protocolo DHCP en el router central. Se configuraron pools separados para distintos departamentos y se aplicaron exclusiones para proteger las direcciones de los Gateways y futuros servidores.

## Conceptos Aplicados
- **Módulo 11:** Proceso DORA (Discover, Offer, Request, Acknowledge).
- **Exclusiones de IP:** Prevención de conflictos de direccionamiento.
- **Gestión de Red:** Verificación de asignaciones mediante `show ip dhcp binding`.

## Nota de Seguridad (Ethical Hacking)
DHCP no tiene autenticación por defecto. En este escenario, la red es vulnerable a ataques de 'Rogue DHCP Server' (un servidor falso que da Gateways falsos para interceptar tráfico) y 'DHCP Starvation'.