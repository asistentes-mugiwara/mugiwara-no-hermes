# 🎭 System vs Showcase

## Idea central

`Mugiwara no Hermes` no es el sistema vivo completo.
Es su **escaparate público curado**.

Parece una obviedad, pero conviene dejarlo por escrito porque aquí vive una diferencia importante:

- una cosa es el **sistema real montado en este mini PC**
- otra, la **versión pública que puede enseñarse sin hacer tonterías**

## 🚢 Qué es el sistema real

El sistema real incluye, entre otras capas:

- perfiles Hermes por agente
- gateways operativos
- memoria por capas
- automatizaciones recurrentes
- healthchecks
- backups
- runtime local
- servicios y wiring que no tiene sentido publicar tal cual

Es una máquina viva, no una colección de markdowns simpáticos.

## 🗺️ Qué es el escaparate público

Este repo es la capa que responde a preguntas como:

- qué es Mugiwara
- cómo se reparte la tripulación
- qué principios técnicos y editoriales sigue
- qué stack conceptual lo sostiene
- cómo se organiza la memoria
- cómo se decide qué puede publicarse

Es una representación **útil, honesta y segura** del sistema.

![Mapa público del sistema Hermes + Mugiwara](../public-assets/diagrams/hermes-mugiwara-system-map.svg)

## Qué sí proyecta el escaparate

El repo público sí enseña:

- roles y fronteras de agentes
- arquitectura de alto nivel
- workflow editorial/técnico público
- modelo de configuración pública
- safeguards operativos en versión abstracta
- estado de despliegue en términos de madurez y categorías

## Qué no proyecta

El repo público no enseña:

- el wiring completo del runtime
- configuración viva de perfiles
- secretos o auth
- estado de memoria real
- logs y sesiones
- cableado exacto de automatizaciones
- detalles que acerquen demasiado la reproducción del sistema real

## 🧱 Por qué existe esta separación

Porque enseñar bien no es lo mismo que enseñar todo.

La separación entre sistema y escaparate sirve para:

- proteger superficie sensible
- evitar que la documentación pública se convierta en manual de reconstrucción
- mantener el repo útil para terceros
- conservar honestidad: esto no es un fake, pero tampoco es un dump

## 📐 Regla práctica

Si una pieza ayuda a entender **cómo piensa y se ordena** el sistema, probablemente tiene hueco aquí.
Si ayuda demasiado a entender **cómo levantar exactamente** el sistema vivo, probablemente no.

## 👑 Consecuencia editorial

Este repo no compite por ser la copia más completa del sistema real.
Compite por ser algo más difícil:

> un resumen técnico público que siga siendo interesante sin volverse irresponsable.

## Documentos relacionados

- [`docs/deployment-status.md`](deployment-status.md)
- [`docs/operations-safeguards.md`](operations-safeguards.md)
- [`docs/configuration-model.md`](configuration-model.md)
- [`docs/workflow-model.md`](workflow-model.md)
- [`docs/publishing-policy.md`](publishing-policy.md)
