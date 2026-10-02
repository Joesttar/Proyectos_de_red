Cisco Enterprise Network Engineering Portfolio
Bienvenido al repositorio central de arquitectura, diseño e implementación de infraestructura de red empresarial basado en tecnologías Cisco Systems.

Este repositorio documenta el desarrollo progresivo y la construcción modular de una red corporativa desde sus fundamentos (Small Office / Home Office) hasta una infraestructura Enterprise Multi-Tier con ruteo Capa 3, servicios centralizados, seguridad y salida a Internet (NAT/PAT).

📌 Arquitectura General del Repositorio
El proyecto está estructurado en 6 fases/proyectos consecutivos, donde cada carpeta representa un hito técnico evolutivo dentro del diseño de red:

Plaintext


.
├── 📁 01-Basic-LAN-SOHO/                        # Fundamentos L2, direccionamiento plano y conectividad ICMP
├── 📁 02-Network-Segmentation-Routing/         # Segmentación por VLANs, Trunking 802.1Q e Inter-VLAN Routing
├── 📁 03-Configuracion-Servidor-DHCP/          # Asignación dinámica de direcciones multi-pool e IP Helper
├── 📁 04-Servicios-WebDNS-SSH/                 # Servicios de aplicación (DNS/HTTP) y Hardening con SSH v2
├── 📁 05-SimulatingProblems-Troubleshooting/  # Metodología de diagnóstico, simulación de fallas y resolución OSI
└── 📁 06-Enterprise-Network/                   # Núcleo L3, enlace P2P de tránsito, R-EDGE-01 y egress WAN (NAT)


Resumen de Proyectos
01-Basic-LAN-SOHO
Objetivo: Creación de la topología base en una sola subred (192.168.1.0/24). Verificación de conectividad nivel de acceso y tabla de direcciones MAC.

02-Network-Segmentation-Routing
Objetivo: Eliminación de dominios de broadcast masivos. Creación de la base de datos de VLANs corporativas, configuración de troncales 802.1Q e implementación de Inter-VLAN routing (Router-on-a-Stick / SVIs).

03-Configuracion-Servidor-DHCP
Objetivo: Automatización de direccionamiento IP. Creación de múltiples pools de DHCP en el Core Switch con reserva de direcciones de infraestructura mediante ip dhcp excluded-address.

04-Servicios-WebDNS-SSH
Objetivo: Despliegue de servicios de red en el segmento corporativo (DNS y Servidor Web) y aseguramiento del plano de administración de la infraestructura utilizando par de llaves RSA de 2048 bits para SSH v2.

05-SimulatingProblems-Troubleshooting
Objetivo: Laboratorio intensivo de resolución de fallas basado en la metodología del modelo OSI (errores en MDIX/Duplex, mismatches en VLAN Nativa, bucles de Spanning Tree, fallos de asignación APIPA).

06-Enterprise-Network
Objetivo: Integración final del modelo jerárquico. Conexión L3 entre el switch distribuido (DSW-CORE-01) y el router de borde (R-EDGE-01), ruteo de tránsito, summarization y traducción de direcciones (NAT/PAT) hacia el proveedor de servicios (ISP).
