# 🕹️ Control Plane: código público, uso privado

## Idea central

Mugiwara no solo necesita agentes con roles claros. También necesita una forma ordenada de **mirar el barco por dentro** sin convertir la cubierta pública en una sala de máquinas abierta.

Por eso existe un proyecto hermano:

- [`mugiwara-control-panel`](https://github.com/asistentes-mugiwara/mugiwara-control-panel)

Ese repo contiene el código público de un **control plane privado** para Mugiwara/Hermes. La frase parece contradictoria, así que conviene separarla bien:

- **código público** → arquitectura, contratos y documentación que pueden revisarse sin exponer secretos
- **uso privado** → despliegue real, datos vivos, configuración y acceso operativo se quedan fuera

## Qué problema resuelve

A alto nivel, el control plane existe para ayudar a la tripulación a consultar el estado del sistema sin depender de memoria humana ni comandos improvisados.

Su misión pública se puede resumir así:

- dar una vista de estado del sistema desde un dashboard claro
- navegar perfiles Mugiwara y responsabilidades sin convertir roles en ruido
- consultar skills, memoria y vault como capas separadas, no como un cajón desastre
- observar healthchecks, repos Git y señales de uso sin publicar logs, dumps ni métricas crudas
- mantener una frontera clara entre lectura segura y acciones permitidas
- enseñar una línea visual reconocible mediante capturas revisadas, sin abrir secretos ni configuración operativa

Dicho en idioma de cubierta: mirar la brújula está bien; regalar el mapa completo de la sala de máquinas, no. ⚓

## Principios de diseño

El control plane sigue los mismos principios que este escaparate:

1. **Deny by default**: si una fuente no está permitida explícitamente, no se expone.
2. **Lectura antes que escritura**: la superficie operativa empieza por observabilidad y navegación, no por botones peligrosos.
3. **Backend como frontera de seguridad**: la capa de API decide qué se puede leer, cómo se sanea y cómo se degrada.
4. **Estados honestos**: cuando una fuente no está configurada, está stale o usa fallback, se dice sin fingir telemetría viva.
5. **Sin material crudo**: nada de logs reales, dumps de memoria, rutas sensibles, stdout/stderr, tokens ni payloads internos.

## Qué se cuenta aquí y qué no

Este documento cuenta el **modelo público** del control plane:

- existe como proyecto software oficial
- se diseña para observabilidad y navegación privada
- usa allowlists y revisión editorial como frontera
- separa código público de despliegue privado
- conserva una política de exposición estricta

Este documento no cuenta:

- rutas internas de despliegue
- URLs privadas o hosts
- configuración runtime
- credenciales, tokens o `.env`
- registros reales de healthcheck
- contenido real de memoria viva
- detalles suficientes para reconstruir la topología operativa

## Relación con este repo

`mugiwara-no-hermes` explica el **modelo público del sistema**.

`mugiwara-control-panel` implementa una pieza concreta del sistema: una consola privada para observar y navegar Mugiwara/Hermes con cuidado.

La relación sana entre ambos es esta:

- este repo explica el mapa conceptual
- el control panel desarrolla una herramienta real
- ambos mantienen política pública estricta
- ninguno debe filtrar el runtime privado

El README del control panel funciona ahora como pequeña cubierta de producto: describe la consola con más energía, enlaza este escaparate y muestra capturas reales revisadas de sus páginas principales. Esas imágenes sirven para enseñar dirección visual, navegación y composición en un corte concreto, manteniendo fuera secretos, credenciales y configuración operativa.

## Estado público actual

El control plane ya no es solo una pieza planificada o un repo de código: tiene un **despliegue privado operativo** para observabilidad y navegación interna.

La versión pública de ese estado se cuenta con brocha gruesa, porque el detalle fino pertenece al sistema vivo:

- la interfaz se consume desde un perímetro privado
- la API queda detrás de una frontera interna, no como API pública abierta
- las superficies de lectura priorizan dashboard, tripulación, memoria, vault, healthcheck, uso agregado y Git en modo controlado
- las escrituras siguen restringidas a capacidades explícitas y revisadas
- los estados degradados se muestran como degradados, no como telemetría mágica

La señal importante para el escaparate es esta:

> Mugiwara ya está pasando de “agentes bien definidos” a “sistema observable y gobernable”, sin abandonar la regla de no publicar más de la cuenta.

Eso es un avance de madurez, no una invitación a abrir la bodega. 🛡️
