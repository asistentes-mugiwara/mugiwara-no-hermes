# 🧭 Configuration Model

## Idea central

Este repositorio no publica una copia viva de la configuración interna.
Publica su **modelo saneado**: qué clases de configuración existen en el ecosistema Hermes + Mugiwara, cuáles son públicas y cuáles se quedan fuera por seguridad o por simple criterio editorial.

## Qué entendemos por configuración

Aquí “configuración” significa el conjunto de decisiones declarativas que permiten entender cómo se gobierna el escaparate y cómo se ordena el sistema a nivel público:

- identidad del repo
- límites de publicación
- estructura documental
- roles y responsabilidades
- convenciones editoriales
- ejemplos públicos seguros
- separación entre memoria, canon y runtime

No significa credenciales, runtime vivo ni parámetros operativos sensibles.

## 🧱 Capas públicas de configuración

### 1. Configuración del runtime base
Es la capa que explica que **Hermes** actúa como superficie de ejecución y que **Mugiwara** se monta encima como tripulación especializada.

A nivel público solo interesa contar:

- que existe una base de ejecución
- que los agentes tienen perfiles/roles diferenciados
- que la operación no vive entera dentro de este repo

### 2. Configuración por agente
Sirve para explicar qué está configurado conceptualmente por cada Mugiwara:

- alcance del rol
- tipo de decisiones que puede tomar
- límites de autonomía
- relación con Luffy, Zoro, Franky y el resto

Lo público aquí es el **contrato**, no la config literal del perfil.

### 3. Configuración por proyecto
Es la capa que dice cómo se ordena un proyecto o repo concreto:

- slug o identidad pública
- política de publicación
- estructura de docs
- examples dummy
- reglas de versionado editorial

En este repo eso se ve, por ejemplo, en `openspec/config.yaml` y en `examples/public-demo-config.yaml`, siempre en versión pública y saneada.

### 4. Configuración de memoria y canon
Aquí se explica la separación entre capas, porque en Mugiwara no todo va al mismo cajón:

- memoria compacta de perfil
- memoria relacional compartida
- memoria viva técnica por proyecto
- vault como canon curado

Lo importante no es enseñar wiring interno, sino que **cada clase de información tiene su sitio**.

### 5. Configuración de gobierno editorial
Es la capa que define cómo se decide qué entra en el escaparate:

- qué puede cambiar Zoro sin escalar
- qué debe revisarse con más cuidado
- qué jamás debe publicarse
- qué tono y nivel de detalle son aceptables

## 🧪 Qué puede enseñarse con ejemplos

La configuración pública sí puede apoyarse en ejemplos, pero solo si son claramente seguros:

- valores dummy
- nombres genéricos
- fragmentos mínimos
- estructuras pedagógicas
- ejemplos que ilustren sin habilitar abuso

## 🚫 Qué se queda fuera

No se documenta aquí:

- secretos
- `.env`
- tokens, cookies o credenciales
- IDs operativos reales
- topología interna detallada
- estados de sesión o memoria cruda
- wiring exacto del runtime
- prompts internos completos

## 📏 Regla de lectura

Si una pieza de configuración ayuda a entender el proyecto sin permitir reconstruirlo, puede publicarse.
Si ayuda demasiado a reconstruirlo, se queda fuera.

Dicho en versión Grand Line: mostramos la carta de navegación, no el compartimento secreto del casco. 🗺️

## Documentos relacionados

- [`docs/publishing-policy.md`](publishing-policy.md)
- [`docs/operations-model.md`](operations-model.md)
- [`docs/autonomy-model.md`](autonomy-model.md)
- [`docs/architecture.md`](architecture.md)
- [`examples/public-demo-config.yaml`](../examples/public-demo-config.yaml)
