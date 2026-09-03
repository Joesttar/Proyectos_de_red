# Proyecto 4: Simulación de Salida a Internet con NAT y DNS

## Descripción
En este proyecto conecté la red local a un entorno que simula Internet. Implementé **NAT Overload (PAT)** para permitir que múltiples hosts privados naveguen con una sola IP pública y configuré servicios de **DNS y HTTP**.

## Conceptos Aplicados
- **Módulo 12.2:** Traducción de Direcciones de Red (NAT).
- **Módulo 14.2.4:** Rutas estáticas predeterminadas (0.0.0.0/0).
- **Módulo 16.3/16.4:** Resolución de nombres (DNS) y transferencia de hipertexto (HTTP).

## Seguridad (Hacker Perspective)
Como se detalla en el material (Módulo 12.2), el NAT oculta las IPs internas, pero **no es un firewall**. Se debe complementar con ACLs para evitar ataques de 'NAT Slipstreaming' o 'Exfiltración de datos'.