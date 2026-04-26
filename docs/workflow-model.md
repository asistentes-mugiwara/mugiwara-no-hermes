# 🧩 Workflow Model

## Idea central

Este repositorio publica un flujo de trabajo **editorial y técnico**, no el detalle operativo del sistema privado.
El objetivo es mostrar cómo se decide, se delega, se sanea, se verifica y se publica sin abrir la sala de máquinas.

## 🌊 Flujo base

### 1. Entrada por Luffy
En el modelo público, **Luffy** actúa como punto de entrada cuando el cambio nace como necesidad, duda o iniciativa transversal.

Su papel es:

- entender el objetivo
- decidir si hace falta especialista
- marcar rumbo cuando hay conflicto o ambigüedad estratégica

### 2. Delegación a especialistas
Cuando el trabajo cae en un dominio claro, entra la tripulación adecuada:

- **Zoro** para software, arquitectura, docs técnicas, verify y releases
- **Usopp** para framing público, onboarding, tono, copy visible y legibilidad del escaparate
- **Franky** cuando hacen falta automatización, sistemas o workflows de soporte
- otros Mugiwara cuando el dominio lo pida

Aquí lo importante no es enseñar el runtime interno completo, sino dejar claro que **la responsabilidad se delega con criterio y dueño reconocible**.

### 3. Clasificar valor y riesgo
Antes de tocar nada, se pregunta:

- ¿aporta valor público real?
- ¿expone secretos?
- ¿revela runtime vivo?
- ¿rompe la publishing policy?
- ¿merece README, doc, changelog o release?

### 4. Sanear
Si el material es publicable, se limpia:

- se eliminan datos sensibles
- se sustituyen valores reales por ejemplos dummy
- se recorta detalle operativo innecesario
- se conserva lo didáctico y reusable

### 5. Implementar y actualizar docs
El cambio se refleja en la capa pública adecuada:

- README si afecta onboarding o framing
- docs temáticas si mejora comprensión del sistema
- changelog si cambia el valor público del escaparate
- release si hay salto narrativo/editorial claro

### 6. Verify
Antes de publicar, el cambio debe pasar una verificación razonable.
En este repo eso significa, como mínimo:

- revisar coherencia del texto
- comprobar que el contenido sigue siendo seguro
- pasar los checks documentales del repo
- confirmar que no se ha colado material interno

### 7. Revisar PRs según perímetro
Cuando un cambio público vive en una PR relevante, el modelo Mugiwara separa **quién construye** de **quién revisa el riesgo**.

La regla pública saneada es:

- **Zoro** construye, verifica y abre la PR
- **Franky** revisa si el cambio toca operación, runtime, CI/CD o automatización
- **Chopper** revisa si el cambio toca seguridad, permisos, auth, secretos, dependencias o exposición
- **Usopp** revisa si el cambio toca diseño, UI, UX, copy visible o percepción pública
- si el cambio mezcla perímetros, se combinan reviewers

La idea no es añadir teatro: es evitar que una misma espada corte, juzgue y selle la cubierta cuando hay riesgo real. ⚔️

En cambios triviales o puramente documentales de bajo riesgo, Zoro puede cerrar con verify local y revisión editorial propia si la política del repo lo permite.

### 8. Publicar o cortar
Si pasa el filtro, se publica.
Si no lo pasa, se corta sin drama, aunque el texto “quedase increíble”.

## 👥 Roles dentro del flujo

### Luffy
- entrada principal cuando la duda es transversal
- dirección de rumbo y prioridad
- arbitraje cuando la decisión ya no es solo técnica

### Zoro
- custodio técnico del repo
- responsable principal de arquitectura pública, verify y releases
- filtro de precisión técnica y saneado cuando el cambio toca estructura, ejemplos o riesgo operativo

### Franky
- apoyo en automatización, tooling y workflows de soporte
- refuerzo cuando el cambio toca más operación que narrativa

### Chopper
- revisión de seguridad cuando una PR toca auth, secretos, permisos, dependencias, endpoints o exposición accidental
- voz de bloqueo cuando el riesgo residual no está suficientemente controlado

### Usopp
- revisión visual/UX cuando el cambio afecta interfaz, jerarquía visual, copy visible o percepción de marca
- apoyo para que lo público sea claro, legible y no solo técnicamente correcto
- mantenimiento editorial recurrente del escaparate cuando el cambio sea de framing, onboarding o narrativa pública

## 🧠 Qué se promociona y qué no

El workflow público también depende de decidir bien el destino de cada cosa:

- **repo público** → explicación segura, docs, ejemplos dummy, changelog
- **vault** → canon duradero y resumido
- **memoria viva** → continuidad de trabajo y contexto técnico, no material público
- **nada** → todo lo que no aporte o aumente riesgo

## 🚫 Qué no describe este documento

Este documento no describe:

- el pipeline interno real completo
- prompts operativos sensibles
- secuencias privadas de agentes
- estados de sesión, memoria o wiring interno

Describe la **versión pública y segura** del movimiento del barco.

## Documentos relacionados

- [`docs/publishing-policy.md`](publishing-policy.md)
- [`docs/operations-model.md`](operations-model.md)
- [`docs/autonomy-model.md`](autonomy-model.md)
- [`docs/release-policy.md`](release-policy.md)
- [`docs/configuration-model.md`](configuration-model.md)
