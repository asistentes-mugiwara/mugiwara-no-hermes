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

- Repo original: [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent)

### OpenCode
**Rol en el sistema:** runtime multiagente de software usado especialmente en la capa de trabajo de Zoro.

Aquí aporta ejecución práctica para flujos de implementación, delegación técnica y operación software con estructura.

- Repo original: [anomalyco/opencode](https://github.com/anomalyco/opencode)

### gentle-ai
**Rol en el sistema:** marco de trabajo y assets para especialización, SDD, generated-multi, Engram y composición de agentes.

Aquí cumple el papel de astillero conceptual y operativo sobre el que se afina la tripulación Mugiwara.

- Repo original: [Gentleman-Programming/gentle-ai](https://github.com/Gentleman-Programming/gentle-ai)

### Engram
**Rol en el sistema:** memoria viva técnica por proyecto.

Sirve para guardar decisiones locales, continuidad de debugging, convenciones de repo y contexto de trabajo que no debería contaminar el canon global.

- Repo original: [Gentleman-Programming/engram](https://github.com/Gentleman-Programming/engram)

### Honcho
**Rol en el sistema:** memoria relacional compartida.

Ayuda a mantener contexto útil sobre preferencias, relaciones y continuidad conversacional sin mezclarlo con la memoria técnica viva.

- Repo original: [plastic-labs/honcho](https://github.com/plastic-labs/honcho)

### Vault canónico
**Rol en el sistema:** capa de canon duradero y curado.

Aquí viven summaries, decisiones estables, playbooks y conocimiento compartible que debe sobrevivir más allá de una sesión.

> Nota: el vault aquí es una capa propia del sistema Mugiwara, no un proyecto externo con repo público de referencia.

### Skills gobernadas
**Rol en el sistema:** catálogo de capacidades reutilizables, separadas por dominio y agente responsable.

Las skills ayudan a que aprendizajes operativos, flujos probados y criterios específicos no dependan de la memoria improvisada de una sesión. El principio público es separar los espacios runtime privados del canon gobernado y promocionar capacidades solo tras revisión; el inventario vivo y los detalles internos de carga se quedan fuera.

### Mugiwara Control Panel
**Rol en el sistema:** proyecto hermano para observabilidad y navegación privada de Mugiwara/Hermes.

Su código público ayuda a enseñar arquitectura y gobierno. Su despliegue privado ya opera como consola interna, pero configuración viva, datos operativos y acceso real siguen fuera del escaparate.

- Repo público: [asistentes-mugiwara/mugiwara-control-panel](https://github.com/asistentes-mugiwara/mugiwara-control-panel)
- Modelo público: [`docs/control-plane.md`](control-plane.md)

### Git + GitHub
**Rol en el sistema:** trazabilidad, revisión, versionado y publicación.

Permiten gobernar cambios, revisar PRs, mantener releases y dejar claro qué entra en cubierta y qué no.

- Git: [git/git](https://github.com/git/git)
- GitHub: [github.com](https://github.com)

## 🧠 Capas de memoria, en versión corta

El sistema diferencia varias capas porque no toda memoria merece el mismo destino:

- **builtin memory** → compacta, estable y mínima
- **Honcho** → relacional y compartida
- **Engram** → viva y técnica por proyecto
- **Vault** → canónica, duradera y curada

Esa separación es parte de la gracia del modelo: menos caos, menos mezcla y más criterio.

## 🙏 Agradecimientos

### [Gentleman-Programming/gentle-ai](https://github.com/Gentleman-Programming/gentle-ai)
Agradecimiento explícito al trabajo detrás de **gentle-ai**, por aportar marco, primitives y enfoque para construir sistemas multiagente con más estructura y menos humo.

### [anomalyco/opencode](https://github.com/anomalyco/opencode)
Agradecimiento a **OpenCode** como pieza importante del runtime software multiagente que hace viable parte de la operativa técnica de Zoro.

### [Gentleman-Programming/engram](https://github.com/Gentleman-Programming/engram)
Agradecimiento por la idea y la pieza de **memoria viva por proyecto**, clave para que un sistema especializado no acabe confundiendo continuidad técnica con canon definitivo.

### [plastic-labs/honcho](https://github.com/plastic-labs/honcho)
Agradecimiento por la capa de **memoria relacional**, útil para mantener contexto humano compartido sin convertir cada conversación en un vertedero de estado.

### Ecosistema open-source y tooling usado
También hay deuda buena con el ecosistema que hace posible lo demás: **[Git](https://github.com/git/git)**, **[GitHub](https://github.com)** y otras herramientas que sostienen la disciplina operativa, el versionado y la colaboración.

## 📌 Nota editorial

Este documento reconoce tecnologías y proyectos usados o influyentes a nivel de arquitectura pública.
No pretende reclamar autoría ajena ni convertir el repo en una vitrina de logos.

La idea es más simple y más honesta:

> decir con qué navegamos, enlazar a quienes construyeron piezas clave y agradecer sin hinchar el escaparate.
