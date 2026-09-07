# Proyecto 5: Diagnóstico de Fallas y Herramientas de Red

## Descripción
En este proyecto apliqué metodologías de Troubleshooting para resolver 3 fallas críticas de red (Gateway mal configurado, DNS erróneo y falta de ruta estática). Utilicé las herramientas estándar de la industria para identificar el origen de los fallos.

## Evidencias de Diagnóstico:
1. **IPCONFIG /ALL:** Detectó inconsistencias en el Default Gateway del departamento de Contabilidad.
2. **NSLOOKUP:** Identificó que las peticiones DNS estaban siendo enviadas a un servidor inexistente.
3. **TRACERT:** Confirmó que los paquetes morían en el Router Central debido a la falta de una ruta de salida (Gateway of last resort).

## Comando Detective (Hacker Insight)
Utilicé `ping -i` (TTL) para mapear la distancia hacia el servidor de Google y determinar cuántos routers intermedios existían en la topología, una técnica básica de reconocimiento (Footprinting).