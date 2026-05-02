# 🌊 Mugiwara no Hermes

> Escaparate público de un sistema multiagente privado: suficiente para entenderlo, no para reconstruirlo.

`Mugiwara no Hermes` es la capa pública curada de un sistema multiagente real construido sobre Hermes y el modelo Mugiwara de **[Pablo](https://github.com/Prodelaya)**.

No es el runtime vivo.<br>
No es un dump de configuración.<br>
No es una colección simpática de agentes con sombrero.

Es una forma de enseñar **arquitectura, memoria, gobernanza y operación** sin abrir la sala de máquinas. ⚓

## 🎯 Qué es este repo

Este repositorio versiona el **relato técnico público** del sistema:

- roles reales de una tripulación de agentes especializados
- separación entre memoria viva, memoria relacional y canon curado
- criterios de delegación, revisión y publicación
- ejemplos y diagramas saneados para explicar sin exponer
- documentación con carisma Mugiwara, pero con disciplina técnica

La promesa es sencilla: que el lector entienda cómo piensa el sistema sin recibir material útil para levantarlo tal cual.

## 🧭 Qué aprenderás aquí

Si subes a esta cubierta, vienes a entender:

- cómo evitar que “multiagente” signifique “el mismo bot con diez sombreros”
- cómo repartir responsabilidad entre agentes con dominios reales
- cómo ordenar capas de memoria sin mezclar conversación, proyecto y canon
- cómo publicar documentación técnica sin filtrar superficie sensible
- cómo combinar criterio técnico, gobierno editorial y una voz reconocible

## 🚫 Qué no vas a encontrar

Este repo **no** contiene:

- secretos, tokens, `.env` o credenciales
- configuración real de producción
- wiring interno completo del runtime
- memoria viva, estados de sesión o logs reales
- topología interna con detalle explotable
- prompts sensibles o bypasses operativos
- material que ayude más a reconstruir el sistema que a entenderlo

Regla práctica:

> si una pieza ayuda poco a comprender y mucho a exponer, se queda fuera.

## 🗺️ Mapa de lectura

### Empieza aquí
- [`docs/overview.md`](docs/overview.md) → tesis breve del proyecto
- [`docs/architecture.md`](docs/architecture.md) → arquitectura pública de alto nivel
- [`docs/system-vs-showcase.md`](docs/system-vs-showcase.md) → frontera entre sistema vivo y escaparate

### Para entender gobierno y publicación
- [`docs/operations-model.md`](docs/operations-model.md) → quién custodia cada tipo de decisión pública
- [`docs/workflow-model.md`](docs/workflow-model.md) → cómo se decide, sanea, verifica y publica
- [`docs/autonomy-model.md`](docs/autonomy-model.md) → qué puede decidir cada custodia de dominio
- [`docs/publishing-policy.md`](docs/publishing-policy.md) → qué puede zarpar y qué se queda en puerto
- [`SECURITY.md`](SECURITY.md) → cómo reportar exposición o riesgo

### Para ampliar contexto
- [`docs/crew-roster.md`](docs/crew-roster.md) → quién es quién en la tripulación
- [`docs/deployment-status.md`](docs/deployment-status.md) → estado público de activación
- [`docs/operations-safeguards.md`](docs/operations-safeguards.md) → safeguards operativos en versión saneada
- [`docs/control-plane.md`](docs/control-plane.md) → control plane privado explicado sin abrirlo
- [`docs/configuration-model.md`](docs/configuration-model.md) → modelo público de configuración
- [`docs/stack-and-credits.md`](docs/stack-and-credits.md) → stack, capas y créditos
- [`docs/release-policy.md`](docs/release-policy.md) → versionado editorial
- [`examples/public-demo-config.yaml`](examples/public-demo-config.yaml) → ejemplo dummy y seguro

## 👥 La tripulación, en corto

Mugiwara funciona con especialización real, no con skins intercambiables:

- **Luffy** → coordinación, prioridad y cierre ejecutivo
- **Zoro** → software, arquitectura, implementación y verify técnico
- **Franky** → infraestructura, automatización y sistemas
- **Nami** → finanzas y reporting
- **Usopp** → marketing, diseño, narrativa visual y mantenimiento editorial
- **Robin** → research e inteligencia
- **Chopper** → ciberseguridad
- **Brook** → datos y analítica
- **Sanji** → compras, reservas, viajes y vigilancia práctica
- **Jinbe** → legal, regulación y burocracia española

Más detalle en [`docs/crew-roster.md`](docs/crew-roster.md).

## 🧰 Stack público

La explicación pública se apoya en estas capas:

- **Hermes** → runtime base y orquestación
- **OpenCode** → runtime software en el dominio de Zoro
- **gentle-ai** → framework y assets de trabajo
- **Engram** → memoria técnica viva por proyecto
- **Honcho** → memoria relacional compartida
- **Vault** → canon duradero y curado
- **Skills gobernadas** → catálogo de capacidades reutilizables por dominio
- **[Control Panel](https://github.com/asistentes-mugiwara/mugiwara-control-panel)** → consola privada de observabilidad y navegación, con código público saneado
- **Git + GitHub** → trazabilidad, revisión y publicación

Créditos y enlaces: [`docs/stack-and-credits.md`](docs/stack-and-credits.md).

## 🕹️ Proyecto hermano: Mugiwara Control Panel

El escaparate cuenta el mapa; el **[Mugiwara Control Panel](https://github.com/asistentes-mugiwara/mugiwara-control-panel)** enseña una pieza navegable del barco.

Es una consola privada para observar Mugiwara/Hermes con prudencia: dashboard, tripulación, skills, memoria, vault, healthchecks, repos Git y uso agregado. Su README incluye **capturas reales revisadas** para mostrar la experiencia visual sin publicar secretos, credenciales ni configuración operativa.

La frontera es deliberada:

- aquí se explica el modelo público del sistema;
- allí se desarrolla el control plane como producto software;
- en ambos casos manda la misma regla: claridad sí, exposición innecesaria no.

Más contexto: [`docs/control-plane.md`](docs/control-plane.md).

## 🖼️ Mapa visual

![Mapa público del sistema Hermes + Mugiwara](public-assets/diagrams/hermes-mugiwara-system-map.svg)

> La carta náutica enseña la forma del sistema; no entrega las llaves de la bodega.

## 🧱 Frontera sistema vivo vs escaparate

El sistema real ejecuta agentes, mantiene memoria viva, opera servicios, gateways, automatizaciones y wiring privado.

Este repo explica el modelo, documenta principios, ofrece ejemplos saneados y protege la operación real.

Si quieres ver esa frontera mejor dibujada, lee [`docs/system-vs-showcase.md`](docs/system-vs-showcase.md).

## 📌 Estado actual

- tipo: repositorio público escaparate
- gobierno técnico: `zoro`
- mantenimiento editorial: `usopp`
- política de publicación: `deny-by-default`
- estilo editorial: épica técnica con humor Mugiwara y emojis con cabeza ⚔️
- versión editorial actual: `v0.6.4`

## 🤝 Contribuir

Suman especialmente:

- mejoras de claridad documental
- ejemplos dummy pedagógicos
- diagramas públicos saneados
- correcciones técnicas precisas
- mejoras editoriales que hagan el repo más útil y legible

Guía: [`CONTRIBUTING.md`](CONTRIBUTING.md).

## 🛡️ Seguridad

Si ves algo que expone demasiado:

- **no abras una issue pública** con contenido sensible
- contacta por privado con la cuenta propietaria del repo si puedes
- indica ruta afectada y tipo de exposición sin repetir secretos
- si hay duda, primero se retira y luego se discute

Política completa: [`SECURITY.md`](SECURITY.md).

## 📜 Releases

Las releases no miden cuánto se revela del sistema real. Miden madurez documental, claridad arquitectónica, calidad del escaparate y seguridad editorial.

Historial: [`CHANGELOG.md`](CHANGELOG.md).

## 👑 Cierre

`Mugiwara no Hermes` no compite por ser la copia pública más completa del sistema real.

Compite por algo más difícil:

> ser un escaparate técnico útil, legible y con carisma<br>
> **sin dejar de ser prudente**.

Buen viaje. ⚓
