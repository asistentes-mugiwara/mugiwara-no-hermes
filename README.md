# Mugiwara no Hermes

Escaparate público del sistema **Hermes + Mugiwara** de Pablo: una arquitectura multiagente operada sobre Hermes, con especialización real por agente, canon en vault y gobierno editorial automatizable.

> Este repositorio está concebido para ser **gestionado autónomamente por Zoro** como custodio técnico/editorial del escaparate público.

## Qué es

`Mugiwara no Hermes` no es el sistema productivo real. Es su **representación pública saneada**:

- explica la arquitectura
- muestra el modelo operativo
- documenta decisiones y convenciones compartibles
- enseña ejemplos públicos y no sensibles
- sirve como demostración de un repositorio gobernado por un agente Mugiwara

## Qué demuestra

- orquestación multiagente con roles diferenciados
- separación entre memoria viva, memoria relacional y canon curado
- gobierno por capas (`AGENTS`, `SOUL`, vault, skills)
- operación técnica y documental con trazabilidad por agente
- publicación pública con política de saneado **deny-by-default**

## Qué NO contiene

Este repositorio **no** contiene:

- secretos, tokens, `.env` ni credenciales
- configuración productiva real
- topología interna completa del sistema
- memoria viva, logs reales o estado runtime
- prompts internos completos cuando revelen lógica sensible
- identificadores operativos innecesarios

## Cómo leer este repo

1. `docs/overview.md`
2. `docs/architecture.md`
3. `docs/operations-model.md`
4. `docs/publishing-policy.md`
5. `docs/release-policy.md`
6. `examples/public-demo-config.yaml`

## Modelo de gobierno

- **Luffy** coordina a nivel ejecutivo, pero no gobierna el día a día editorial de este repo.
- **Zoro** es el custodio autónomo de publicación, estructura, versionado, releases y documentación.
- La regla maestra es: **si hay duda sobre si algo debe ser público, no se publica**.

## Estado

- tipo: repositorio público escaparate
- mantenedor operativo: `zoro`
- política de publicación: `deny-by-default`
- versión editorial inicial: `v0.1.0`

## Roadmap inmediato

- estabilizar arquitectura pública explicada
- añadir diagramas públicos saneados
- documentar el modelo de memoria por capas
- mostrar ejemplos de flujos multiagente sin exponer runtime sensible
- publicar releases editoriales con changelog claro

## Licencia

MIT.
