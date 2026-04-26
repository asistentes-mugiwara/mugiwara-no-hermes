# 🛡️ Operations Safeguards

## Idea central

Un sistema así no se sostiene solo con prompts buenos y una sonrisa confiada. Se sostiene con **salvaguardas operativas**.

Este documento explica, a alto nivel y sin enseñar piezas sensibles, qué mecanismos ayudan a que Hermes + Mugiwara no se convierta en una taberna caótica con Wi‑Fi.

## 🔒 Principio operativo

La regla no es “publicar todo lo interesante”.
La regla es:

> operar con criterio, verificar lo suficiente y publicar solo lo que siga siendo seguro.

## 1. Separación por perfil

Los agentes activos funcionan como perfiles separados, no como una masa borrosa que cambia de sombrero según convenga.

Eso permite:

- límites más claros
- trazabilidad por agente
- runtime más ordenado
- menor confusión entre responsabilidades

## 2. Gateways persistentes

La capa conversacional de los perfiles activos no depende de arrancar manualmente cada vez.

A nivel público, lo importante es esto:

- los perfiles activos tienen **gateway persistente por perfil**
- la disponibilidad del agente no depende de una sesión abierta a mano
- el sistema puede vigilar mejor qué está vivo y qué no

## 3. Memoria por capas

Una de las defensas más importantes no es de red ni de puertos: es de **orden mental**.

La arquitectura separa:

- memoria compacta y estable
- memoria relacional compartida
- memoria viva técnica por proyecto
- canon duradero en vault

Esto reduce mezcla peligrosa entre:

- contexto humano
- debugging técnico
- decisiones estables
- artefactos públicos

## 4. Healthchecks ligeros

El sistema ya usa comprobaciones periódicas para evitar una operativa “a ojo”.

Sin entrar en detalle sensible, hay verificaciones sobre cosas como:

- disponibilidad de gateways
- salud de capas críticas
- backup reciente
- señales básicas del host
- errores globales

La idea no es montar una nave espacial de observabilidad, sino detectar pronto si algo deja de flotar.

## 5. Control plane con frontera clara

Mugiwara también cuenta con un proyecto de control plane privado para observabilidad y navegación del sistema.

La safeguard importante no es “tener una consola bonita”. Es que esa consola se diseñe con frontera clara:

- código público saneado, despliegue privado
- lectura controlada antes que escritura peligrosa
- allowlists antes que exploración libre del host
- estados degradados honestos antes que telemetría fingida
- nada de logs, dumps, secretos ni rutas sensibles en la capa pública

Más contexto público:
- [`docs/control-plane.md`](control-plane.md)

## 6. Backups y continuidad

También hay una capa de continuidad operativa:

- backup local recurrente
- checksum del artefacto
- copia offsite
- cobertura de piezas importantes del sistema

No publicamos el wiring exacto de ese pipeline, pero sí el hecho importante: **la continuidad no depende de cruzar los dedos**.

## 7. Gobierno editorial deny-by-default

El repo público vive bajo una regla que también es una safeguard operativa:

- si algo aporta poco y expone mucho, se queda fuera
- si una pieza necesita demasiada explicación para parecer segura, probablemente no lo sea
- si hay duda, no se publica

Esto protege tanto la superficie pública como la calidad del escaparate.

## 8. Verificación antes de cierre

En Mugiwara, cerrar no es solo “me gusta cómo suena”.
Cerrar implica una verificación razonable del cambio:

- coherencia del contenido
- seguridad del detalle publicado
- consistencia con políticas del repo
- checks documentales mínimos
- criterio de si el cambio merece realmente entrar

## 🚫 Qué no se detalla aquí

Por seguridad y por higiene operativa, este documento no entra en:

- units literales
- rutas internas finas
- nombres técnicos sensibles
- secretos o credenciales
- payloads reales
- logs operativos
- topología reconstruible del sistema

## 🧠 Lectura final

Las safeguards de este mini PC no buscan impresionar. Buscan algo más importante:

- que el sistema siga estable
- que cada capa viva donde toca
- que lo público no traicione a lo privado
- y que la nave pueda seguir avanzando sin agujeros innecesarios en el casco
