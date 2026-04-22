# 🧰 Stack & Credits

## Por qué este documento existe

Un sistema como `Mugiwara no Hermes` no sale de la nada ni de una sola espada.
Se apoya en varias piezas, ideas y herramientas que merece la pena explicar y agradecer.

Este documento hace dos cosas:

- mostrar, a nivel público, qué tecnologías y capas forman parte del ecosistema
- reconocer a los creadores y proyectos sobre los que este barco navega

## ⚙️ Piezas principales del stack

### Hermes
**Rol en el sistema:** runtime y superficie operativa base para perfiles, herramientas, automatización y ejecución agente-a-herramienta.

Sin Hermes no hay cubierta donde la tripulación pueda trabajar con disciplina.

### OpenCode
**Rol en el sistema:** runtime multiagente de software usado especialmente en la capa de trabajo de Zoro.

Aquí aporta ejecución práctica para flujos de implementación, delegación técnica y operación software con estructura.

### gentle-ai
**Rol en el sistema:** marco de trabajo y assets para especialización, SDD, generated-multi, Engram y composición de agentes.

Aquí cumple el papel de astillero conceptual y operativo sobre el que se afina la tripulación Mugiwara.

### Engram
**Rol en el sistema:** memoria viva técnica por proyecto.

Sirve para guardar decisiones locales, continuidad de debugging, convenciones de repo y contexto de trabajo que no debería contaminar el canon global.

### Honcho
**Rol en el sistema:** memoria relacional compartida.

Ayuda a mantener contexto útil sobre preferencias, relaciones y continuidad conversacional sin mezclarlo con la memoria técnica viva.

### Vault canónico
**Rol en el sistema:** capa de canon duradero y curado.

Aquí viven summaries, decisiones estables, playbooks y conocimiento compartible que debe sobrevivir más allá de una sesión.

### Git + GitHub
**Rol en el sistema:** trazabilidad, revisión, versionado y publicación.

Permiten gobernar cambios, revisar PRs, mantener releases y dejar claro qué entra en cubierta y qué no.

## 🧠 Capas de memoria, en versión corta

El sistema diferencia varias capas porque no toda memoria merece el mismo destino:

- **builtin memory** → compacta, estable y mínima
- **Honcho** → relacional y compartida
- **Engram** → viva y técnica por proyecto
- **Vault** → canónica, duradera y curada

Esa separación es parte de la gracia del modelo: menos caos, menos mezcla y más criterio.

## 🙏 Agradecimientos

### gentleman-programing / gentle-ai
Agradecimiento explícito al trabajo detrás de **gentle-ai**, por aportar marco, primitives y enfoque para construir sistemas multiagente con más estructura y menos humo.

### OpenCode
Agradecimiento a **OpenCode** como pieza importante del runtime software multiagente que hace viable parte de la operativa técnica de Zoro.

### Engram
Agradecimiento por la idea y la pieza de **memoria viva por proyecto**, clave para que un sistema especializado no acabe confundiendo continuidad técnica con canon definitivo.

### Honcho
Agradecimiento por la capa de **memoria relacional**, útil para mantener contexto humano compartido sin convertir cada conversación en un vertedero de estado.

### Ecosistema open-source y tooling usado
También hay deuda buena con el ecosistema que hace posible lo demás: Git, GitHub y otras herramientas que sostienen la disciplina operativa, el versionado y la colaboración.

## 📌 Nota editorial

Este documento reconoce tecnologías y proyectos usados o influyentes a nivel de arquitectura pública.
No pretende reclamar autoría ajena ni convertir el repo en una vitrina de logos.

La idea es más simple y más honesta:

> decir con qué navegamos y agradecer a quienes ayudaron a construir el barco.
