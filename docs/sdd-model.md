# ⚔️ Spec-Driven Development Model

## Qué explica este documento

Mugiwara no Hermes no trata el software como una carrera de “pídele algo al bot y cruza los dedos”.

En el dominio de Zoro, el sistema trabaja con un modelo público de **Spec-Driven Development**: primero se entiende el cambio, luego se diseña, después se implementa con pruebas y finalmente se verifica contra lo prometido.

Este documento cuenta la idea sin publicar prompts internos, nombres de perfiles runtime, rutas privadas ni wiring operativo.

## 🧭 La ruta pública

El ciclo público se puede leer así:

1. **Explorar** — reducir incertidumbre antes de prometer una solución.
2. **Proponer** — formular intención, alcance y tradeoffs.
3. **Especificar** — convertir la idea en requisitos y escenarios verificables.
4. **Diseñar** — decidir arquitectura, límites y estrategia de pruebas.
5. **Trocear tareas** — hacer el trabajo implementable y revisable.
6. **Aplicar con TDD** — cambiar código siguiendo red, green y refactor cuando toca.
7. **Verificar** — contrastar implementación contra spec, diseño y tareas.
8. **Archivar** — dejar trazabilidad y continuidad para la siguiente navegación.

No es una coreografía decorativa. Es una forma de evitar que la velocidad aparente sustituya al criterio técnico.

## 🧪 TDD como guardarraíl

La implementación debe dejar evidencia real, no solo una explicación convincente.

En versión pública, el principio es:

- si el cambio toca comportamiento, debe tener una prueba o verificación proporcionada;
- si una prueba falla por una razón esperada, se documenta antes de corregir;
- si no hay prueba automatizada razonable, se deja un smoke o revisión manual explícita;
- si falta evidencia, el cambio no se da por cerrado.

Zoro puede blandir la espada, pero el verify decide si el corte fue limpio. ⚔️

## 🧑‍⚖️ Revisión adversarial cuando hay riesgo

Para cambios de software significativos, el modelo contempla revisión adversarial: dos miradas independientes revisan criterios similares y Zoro sintetiza coincidencias, sospechas y bloqueos.

La versión pública no necesita saber cómo se invoca eso por dentro. Lo importante es el patrón:

- revisión read-only cuando el riesgo lo pide;
- criterios compartidos;
- síntesis explícita de hallazgos;
- bloqueo si la evidencia no basta.

## 🧱 Qué se publica y qué no

### Sí se puede publicar

- fases del ciclo a alto nivel;
- criterios de calidad y verify;
- relación entre specs, diseño, tareas y pruebas;
- ejemplos dummy o documentos saneados;
- decisiones editoriales y releases.

### No se publica

- prompts internos;
- nombres o configuración de perfiles runtime;
- rutas del host o mecanismos de carga;
- logs de ejecución reales;
- memoria viva de proyecto;
- comandos privados, endpoints, tokens o wiring reconstructivo.

## Relación con otros documentos

- [`docs/workflow-model.md`](workflow-model.md) explica el flujo general de publicación y saneado.
- [`docs/operations-model.md`](operations-model.md) explica custodia por dominio.
- [`docs/stack-and-credits.md`](stack-and-credits.md) reconoce las piezas del stack que inspiran o sostienen este modelo.
- [`docs/publishing-policy.md`](publishing-policy.md) marca la frontera de seguridad editorial.

## Cierre

La promesa pública del SDD de Zoro es sencilla:

> menos magia, más contrato; menos humo, más evidencia.

Y si una parte del mapa ayuda más a reconstruir la sala de máquinas que a entender el viaje, no zarpa.
