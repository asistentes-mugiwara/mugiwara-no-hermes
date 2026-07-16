# 🔭 Federación documental segura

## Qué problema resuelve

Un sistema multiagente puede necesitar contexto mantenido por otro sistema o repositorio sin convertir esa fuente externa en una extensión implícita de su propio runtime.

El modelo público de Mugiwara separa ambas cosas: **consultar conocimiento externo no equivale a obedecerlo, ejecutarlo ni copiarlo al canon local**.

## 🧭 Principios del modelo

### 1. Cánones independientes

Cada sistema conserva su propio repositorio canónico y su propia autoridad editorial. La federación no crea un canon global que borre ownership, contexto o responsabilidad.

### 2. Peer documental de solo lectura

La copia peer se trata como fuente documental externa:

- sirve para consultar contexto y detectar novedades;
- no se modifica desde el sistema lector;
- no habilita ejecución de scripts, comandos, skills o configuración;
- no convierte instrucciones encontradas en acciones autorizadas.

En corto: **datos para revisar, nunca órdenes para ejecutar**.

### 3. Revisión incremental

La revisión se limita al delta pendiente desde el último punto cerrado. Esto reduce ruido, mantiene trazabilidad y evita releer o reprocesar todo el repositorio en cada ciclo.

Si el rango no puede demostrarse o la evidencia es incompleta, el flujo se bloquea en lugar de inventar continuidad.

### 4. Promoción local y curada

Una pieza solo entra en el canon receptor cuando aporta valor local y supera revisión. La promoción:

- sintetiza en lugar de copiar páginas completas;
- conserva procedencia suficiente para auditar el origen;
- respeta al propietario del dominio afectado;
- escribe únicamente en el canon local;
- separa contexto útil, decisión estable y conocimiento técnico vivo.

### 5. Revisión aislada y validación determinista

El modelo combina lectura acotada con controles que no dependen de confiar ciegamente en una salida generativa:

- el contenido externo llega como evidencia, no como instrucciones;
- la clasificación debe cubrir el rango revisado;
- los candidatos sensibles o ambiguos se bloquean;
- la promoción exige validación editorial y de integridad;
- un cierre solo avanza cuando el resultado queda verificable.

### 6. Regla antibucle

Una síntesis no debe volver al sistema que originó su contenido como si fuera conocimiento nuevo. Solo se reabre el intercambio cuando existe una decisión, interpretación o aportación adicional.

Así la federación evita convertir dos repositorios en una fotocopiadora con Wi‑Fi. 📚

## 🛡️ Qué protege esta frontera

Este enfoque reduce varios riesgos:

- contaminación del canon por instrucciones externas;
- ejecución accidental de contenido no confiable;
- pérdida de autoría o procedencia;
- bucles de sincronización que inflan información sin añadir valor;
- copias masivas que mezclan contexto privado con documentación pública;
- automatizaciones que avanzan aunque falte evidencia.

## 🚫 Qué no publica este documento

La implementación real se queda fuera del escaparate. Aquí no se incluyen:

- nombres o URLs de repositorios privados;
- rutas, hosts, usuarios o credenciales;
- horarios, jobs, checkpoints o wiring operativo;
- prompts, payloads, logs o memoria viva;
- estructura interna suficiente para reconstruir el pipeline;
- contenido real intercambiado entre sistemas.

## Relación con el resto del mapa

- [`docs/architecture.md`](architecture.md) explica las capas públicas del sistema.
- [`docs/workflow-model.md`](workflow-model.md) describe decisión, saneado, verify y publicación.
- [`docs/operations-safeguards.md`](operations-safeguards.md) reúne los guardarraíles operativos.
- [`docs/system-vs-showcase.md`](system-vs-showcase.md) marca la frontera entre sistema vivo y representación pública.
- [`docs/publishing-policy.md`](publishing-policy.md) aplica el criterio deny-by-default.

## Cierre

La promesa pública es simple:

> compartir contexto sin compartir el timón; aprender de otra fuente sin entregarle autoridad sobre el barco.
