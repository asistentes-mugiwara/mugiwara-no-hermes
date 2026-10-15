# ⚔️ Entrega software guiada por resultados

## Qué explica este documento

En el dominio de Zoro, la entrega empieza por el **resultado pedido**, los requisitos reales y la evidencia disponible. Después se diseña lo necesario, se implementa con pruebas cuando cambia el comportamiento y se verifica el bloque funcional completo antes de darlo por cerrado.

El nombre histórico de este archivo conserva el enlace a nuestro modelo SDD anterior. La secuencia formal de exploración, propuesta, spec, diseño, tareas, aplicación, verify y archivo sigue siendo una herramienta posible, **no una obligación para cada cambio**.

Este documento cuenta la disciplina pública sin revelar prompts, perfiles, rutas ni mecanismos internos.

## 🧭 La ruta pública

1. **Entender el resultado** — aclarar alcance, restricciones y criterios verificables sin abrir fases por inercia.
2. **Diseñar lo necesario** — elegir el cambio funcional más pequeño; usar especificaciones o tareas formales cuando el riesgo o el proyecto lo requieran.
3. **Implementar y probar** — para comportamiento nuevo, observar un fallo causal antes de corregirlo y comprobar que la solución pasa; para documentación, revisar el texto y su estructura.
4. **Verificar** — contrastar el resultado completo con los requisitos y los checks aplicables. La revisión independiente se añade cuando el riesgo lo pide, no por el número de ficheros.
5. **Dejar continuidad** — registrar decisiones y evidencias proporcionadas para poder retomar el trabajo, sin convertir el registro en el producto.

El límite de tamaño de una revisión ayuda a leer un cambio; no justifica inventar arquitectura, infraestructura ni entregas artificiales. El mapa sirve al viaje, no al revés. 🗺️

## 🧪 Evidencia antes que relato

- Los cambios de comportamiento necesitan pruebas o comprobaciones proporcionadas y resultados observados, no una explicación convincente.
- Un fallo esperado se identifica antes de corregirlo; no se fabrica un fallo para comportamiento ya demostrado.
- Cuando no cabe una prueba automatizada razonable, se declara la comprobación manual y lo que queda sin verificar.
- Un resultado sin evidencia suficiente se comunica como parcial o bloqueado, no como aprobado.

## 🔍 Verificar sin mover la diana

Verificar no sustituye implementar ni equivale a publicar. Se evalúa el candidato conocido frente al resultado pedido y las restricciones; si una comprobación cambia el estado evaluado, hay que recuperar un estado limpio y repetir la evidencia afectada. Los hallazgos vuelven como trabajo explícito, nunca como correcciones silenciosas que hagan pasar otra versión.

La comprobación independiente, de solo lectura cuando corresponda, escala con el riesgo. Una revisión adversarial con dos miradas independientes se reserva para los casos que la requieren; tampoco autoriza por sí sola un commit o una release.

## 🧱 Frontera pública

Sí contamos el criterio de diseño, pruebas, verificación, revisión proporcionada y continuidad. No publicamos perfiles o prompts internos, rutas del entorno privado, logs, memoria viva, comandos, configuración ni wiring operativo. Las specs y fases siguen teniendo sitio cuando aportan claridad real, pero este escaparate no prescribe un ritual universal.

## Relación con otros documentos

- [`docs/workflow-model.md`](workflow-model.md) explica el flujo general de publicación y saneado.
- [`docs/operations-model.md`](operations-model.md) explica custodia por dominio.
- [`docs/stack-and-credits.md`](stack-and-credits.md) reconoce las piezas del stack.
- [`docs/publishing-policy.md`](publishing-policy.md) marca la frontera de seguridad editorial.

> Menos ceremonia, más resultado verificable; menos humo, más evidencia.
