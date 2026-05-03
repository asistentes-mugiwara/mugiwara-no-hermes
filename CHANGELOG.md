# 📜 Changelog

Todos los cambios relevantes del escaparate público se documentan aquí.

Formato: pragmático, claro y sin drama innecesario. Bueno, con un poco de drama pirate-friendly sí. 🏴‍☠️

## [Unreleased]
### Changed
- `docs-check` protege también `CONTRIBUTING.md` y `docs/operations-model.md`, alineando la verificación con el mapa editorial público del README.

### Security
- El ajuste solo amplía la cobertura de presencia documental; no publica runtime, configuración viva, rutas internas ni superficie reconstructiva.

## [0.6.5] - 2026-05-02
### Changed
- README añade `docs/operations-model.md` al mapa de lectura para que la custodia por dominio tenga una entrada visible desde la portada.
- `docs/operations-safeguards.md`, `docs/deployment-status.md` y `docs/stack-and-credits.md` aclaran el principio público de separación entre espacios runtime privados de skills y canon gobernado.
- README actualiza la versión editorial a `v0.6.5`.

### Security
- La aclaración evita publicar rutas internas, configuración de carga, inventario vivo de skills o automatismos concretos; solo documenta el principio de revisión antes de canonizar capacidades.
- El cambio de navegación editorial no añade runtime, configuración viva, rutas internas ni detalle reconstructivo.

## [0.6.4] - 2026-04-30
### Changed
- `docs/architecture.md` evita duplicar el roster y formula mejor la regla pública de diseño: agentes por dominio, perímetro reconocible y límites de publicación claros.
- `docs/crew-roster.md` aclara la diferencia entre núcleo transversal y especialistas activos por dominio, sin sugerir que solo una parte de la tripulación esté operativa.

### Security
- La aclaración es editorial y de jerarquía documental: no añade runtime, rutas, configuración viva, wiring operativo ni inventario sensible.

## [0.6.3] - 2026-04-29
### Changed
- README comprimido como portada editorial: mantiene propuesta de valor, mapa de lectura, frontera sistema/escaparate, tripulación y stack, pero reduce repetición con docs temáticos y mejora el onboarding inicial.
- README añade una sección de proyecto hermano para `mugiwara-control-panel`, con enlace al repositorio público y explicación de sus capturas revisadas.
- `docs/control-plane.md` amplía la descripción pública del control panel con dashboard, skills, memoria, vault, healthcheck, Git, uso agregado y criterio visual revisado.

### Security
- La poda editorial no añade runtime, rutas internas, configuración viva, memoria real ni nuevos detalles reconstructivos; solo reorganiza información ya pública.
- La referencia a capturas del control panel queda limitada a imágenes revisadas que no publican secretos, credenciales ni configuración operativa.

## [0.6.2] - 2026-04-28
### Changed
- README, `docs/deployment-status.md`, `docs/operations-safeguards.md` y `docs/stack-and-credits.md` explican en versión pública saneada que las skills forman una capa gobernada de capacidades reutilizables, separada por dominio y tratada como catálogo controlado.
- README actualiza la versión editorial a `v0.6.2`.

### Security
- La actualización no publica rutas internas, inventarios vivos de skills, configuración de perfiles, prompts, automatismos sensibles ni wiring operativo; solo añade el principio público de gobierno de capacidades.

## [0.6.1] - 2026-04-28
### Changed
- `docs/autonomy-model.md` alinea la autonomía pública con la custodia por dominio: Zoro mantiene el perímetro técnico, Usopp el editorial y Chopper/otros Mugiwara intervienen cuando su especialidad marca el límite.
- `docs/control-plane.md`, `docs/deployment-status.md`, `docs/operations-safeguards.md` y `docs/stack-and-credits.md` actualizan el estado público del control plane: ya tiene despliegue privado operativo, manteniendo fuera del escaparate el wiring, la configuración viva y los datos reales.
- README actualiza la versión editorial a `v0.6.1`.

### Security
- La actualización solo publica madurez operativa de alto nivel: no añade puertos, hosts, rutas internas, unidades reales, logs, healthchecks crudos, memoria viva, `.env`, secretos ni detalles suficientes para reconstruir el despliegue.

## [0.6.0] - 2026-04-27
### Added
- Nuevo documento `docs/control-plane.md` para explicar públicamente, de forma saneada, la existencia del control plane privado de Mugiwara/Hermes y su relación con este escaparate.

### Changed
- README, `docs/deployment-status.md`, `docs/operations-safeguards.md` y `docs/stack-and-credits.md` enlazan el modelo público del control plane sin publicar despliegue, configuración viva ni wiring operativo.
- `docs-check` verifica que el nuevo documento de control plane siga presente.
- `docs/workflow-model.md` afina la custodia por dominio para que Zoro quede como responsable técnico y Usopp como responsable editorial del escaparate público.

### Security
- El nuevo contenido se limita a arquitectura y gobierno de alto nivel: no publica URLs privadas, rutas internas, logs, dumps de memoria, secretos, healthchecks reales ni endpoints operativos.

## [0.5.1] - 2026-04-26
### Changed
- README, `CONTRIBUTING.md`, `docs/crew-roster.md`, `docs/operations-model.md` y `docs/workflow-model.md` aclaran la custodia por dominio: Zoro mantiene el perímetro técnico y Usopp el mantenimiento editorial del escaparate público.

### Security
- La aclaración queda en nivel de gobierno público y no publica wiring operativo, rutas internas, perfiles vivos ni mecanismos concretos de coordinación.

## [0.5.0] - 2026-04-25
### Added
- `docs/workflow-model.md` amplía el modelo público con el circuito saneado de revisión de PRs por perímetro: Zoro construye, Franky revisa operación, Chopper revisa seguridad y Usopp revisa diseño/UX cuando corresponde.

### Changed
- README actualizado a la versión editorial `v0.5.0` y reforzado con la idea de separar construcción, review y merge sin publicar wiring operativo sensible.

### Security
- El nuevo contenido mantiene el modelo en nivel de gobernanza pública: no incluye comandos internos, rutas privadas, comentarios reales de PR ni mecanismos de invocación entre agentes.

## [0.4.3] - 2026-04-24
### Changed
- `README.md`, `docs/crew-roster.md`, `docs/deployment-status.md` y el mapa público alineados para reflejar la activación pública saneada de **Sanji** y **Jinbe**.
- Estado público actualizado de ocho perfiles activos a la tripulación canónica completa activa, sin publicar wiring sensible ni detalles internos de runtime.

### Fixed
- Desfase entre el canon operativo actualizado del vault y la representación pública de la tripulación pendiente de activación formal.

## [0.4.2] - 2026-04-24
### Changed
- `README.md`, `docs/crew-roster.md` y `docs/deployment-status.md` alineados para reflejar a **Brook** como especialista activo de datos y analítica.
- Estado público actualizado de siete a ocho perfiles activos, manteniendo a **Sanji** y **Jinbe** como tripulación canónica pendiente de activación formal.

### Fixed
- Desfase editorial entre el canon operativo actual y la representación pública de la tripulación activa.

## [0.4.1] - 2026-04-23
### Changed
- `docs/deployment-status.md` actualizado para reflejar siete perfiles activos hoy y no solo el núcleo inicial.
- `docs/crew-roster.md` ampliado para distinguir entre núcleo operativo, especialistas ya activos y tripulación aún pendiente de activación formal.
- README alineado con el estado público verificado del sistema y con la versión editorial `v0.4.1`.

### Fixed
- Desfase entre el canon/runtime verificados y la representación pública del estado de activación de la tripulación.
- Señal pública demasiado conservadora sobre cuántos perfiles Mugiwara están ya desplegados.

## [0.4.0] - 2026-04-22
### Added
- `docs/deployment-status.md` para explicar qué partes del sistema Hermes + Mugiwara están activas hoy en este mini PC.
- `docs/operations-safeguards.md` para explicar las salvaguardas operativas reales del sistema en versión pública saneada.
- `docs/system-vs-showcase.md` para separar explícitamente el sistema vivo del escaparate público.
- `public-assets/diagrams/hermes-mugiwara-system-map.svg` con un mapa visual del sistema desplegado y su frontera pública.

### Changed
- README ampliado para enlazar los nuevos docs de estado, safeguards y frontera sistema/escaparate.
- README y docs clave ahora incorporan un apoyo visual para entender mejor el sistema montado.
- `docs-check` ampliado para verificar también el nuevo asset gráfico público.

### Fixed
- Falta de visibilidad pública sobre qué parte del sistema Hermes + Mugiwara ya está realmente desplegada.
- Brecha entre explicación textual del sistema y comprensión visual del conjunto.

## [0.3.0] - 2026-04-22
### Added
- `docs/configuration-model.md` para explicar qué configuración pública existe y qué queda fuera del escaparate.
- `docs/workflow-model.md` para explicar cómo fluyen decisión, delegación, saneado, verify y publicación en Hermes + Mugiwara.
- Atribución visible a **[Pablo](https://github.com/Prodelaya)** como creador del sistema de agentes Mugiwara desde el README.

### Changed
- README ampliado para enlazar el modelo público de configuración y workflow.
- Workflow `docs-check` ampliado para verificar los nuevos documentos.
- El repo ya explica mejor no solo quién navega y con qué stack, sino también cómo se ordena y cómo trabaja la tripulación.

### Fixed
- Brecha documental entre arquitectura de alto nivel y flujo operativo público.
- Falta de contexto público sobre configuración saneada frente a runtime real.

## [0.2.0] - 2026-04-22
### Added
- Nuevo tono editorial inspirado en la energía, el humor y la épica ligera de One Piece.
- Documento `docs/crew-roster.md` con la tripulación pública y su reparto de roles.
- Documento `docs/stack-and-credits.md` con tecnologías usadas, capas del sistema y agradecimientos públicos.
- Más contexto narrativo para explicar el modelo Mugiwara sin perder precisión técnica.

### Changed
- README rehecho para mejorar onboarding, personalidad y legibilidad.
- README ampliado para presentar directamente a toda la tripulación y enlazar el roster público.
- README ampliado para explicar stack, herramientas y créditos desde la portada.
- Documentación principal reescrita en español con más carisma, estructura y claridad.
- Políticas de publicación, seguridad y releases alineadas con una voz más viva y memorable.
- Workflow `docs-check` actualizado para verificar documentación nueva relevante del escaparate.
- Skill de gobierno editorial del repo actualizada para reflejar el nuevo estándar.

### Fixed
- Coherencia de estilo entre README, docs y políticas públicas.
- Señalización explícita de qué se puede contar y qué debe quedarse fuera del barco.

## [0.1.0] - 2026-04-22
### Added
- Scaffold inicial del repositorio público escaparate.
- README y documentación base del proyecto.
- Publishing policy con reglas `deny-by-default`.
- Release policy para versionado editorial.
- Ejemplo dummy de configuración pública.
- Modelo de gobierno autónomo con Zoro como custodio del repo.
