# Proyecto 2: Segmentación de Red y Gateway Predeterminado

## Descripción
En este laboratorio implementé la segmentación de red para reducir el "Blast Radius" de posibles ataques, tal como se sugiere en los conceptos de defensa en profundidad.

## Conceptos Aplicados
- **Módulo 8/9:** División de redes lógicas para control administrativo y seguridad.
- **Módulo 12:** Configuración de interfaces de Router como Default Gateway.
- **Enrutamiento:** Interconexión de dos dominios de difusión distintos.

## Por qué es importante (Hacker Perspective)
Como se menciona en el material, una red plana permite el "Movimiento Lateral" fácil para un atacante. Al segmentar, obligamos al tráfico a pasar por el Router, donde en el futuro podremos aplicar Listas de Control de Acceso (ACLs).