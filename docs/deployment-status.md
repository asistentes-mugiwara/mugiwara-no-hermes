# 🚦 Deployment Status

## Idea central

`Mugiwara no Hermes` no es solo una idea bonita con sombrero de paja. En este mini PC ya hay una parte del sistema **realmente montada**.

La gracia de este documento es separar tres cosas que conviene no mezclar:

- lo que existe en el **canon Mugiwara**
- lo que está **configurado**
- lo que está **activo hoy de verdad**

## 🧭 Cómo leer este estado

En este repo usamos estas etiquetas conceptuales:

- **Definido** → existe en canon, políticas o roster
- **Configurado** → tiene perfil, memoria o runtime preparados
- **Activo** → está desplegado y funcionando ahora mismo
- **Estable** → además de estar activo, forma parte ya del baseline operativo

## 👒 Tripulación: canon vs estado real

### Definidos en canon
Toda la tripulación Mugiwara existe en la arquitectura oficial:

- Luffy
- Zoro
- Franky
- Nami
- Usopp
- Robin
- Sanji
- Chopper
- Brook
- Jinbe

### Activos hoy
En este mini PC, los perfiles activos y operativos hoy son:

- **Luffy**
- **Zoro**
- **Franky**
- **Nami**
- **Usopp**
- **Robin**
- **Chopper**
- **Brook**
- **Sanji**
- **Jinbe**

No publicamos aquí el cableado fino de cada perfil. La señal pública útil es más simple: la tripulación canónica completa ya figura como activa, con responsabilidades separadas y límites de publicación claros.

![Mapa público del sistema Hermes + Mugiwara](../public-assets/diagrams/hermes-mugiwara-system-map.svg)

## ⚙️ Qué piezas del sistema están activas hoy

### Gateways persistentes por perfil
Los agentes activos no dependen de un arranque manual improvisado. La nave ya usa **gateways persistentes por perfil** para:

- **Luffy**
- **Zoro**
- **Franky**
- **Nami**
- **Usopp**
- **Robin**
- **Chopper**
- **Brook**
- **Sanji**
- **Jinbe**

Eso significa que la capa conversacional está separada por perfil y se mantiene viva como servicio estable.

### Memoria por capas
El modelo de memoria no es solo teórico. Ya hay una separación real entre:

- **builtin memory** como fallback compacto
- **Honcho** como memoria relacional compartida
- **Engram** como memoria viva técnica por proyecto
- **vault** como canon duradero y curado

### Automatización recurrente
También hay automatización viva en la máquina para tareas como:

- sincronización del vault
- backup nocturno local
- subida offsite del backup
- health check periódico del sistema
- revisión editorial nocturna del repo público

### Safeguards operativos
No todo es “que arranque”. También existen controles ligeros para verificar:

- gateways activos
- salud de la capa de memoria compartida
- backup reciente con checksum
- estado general del sistema
- errores globales y señales básicas de presión operativa

## 🧱 Qué significa “activo” en este sistema

En Mugiwara, un agente no pasa a considerarse activo solo porque exista un nombre o un doc.

Normalmente, para considerarlo activo hacen falta varias piezas a la vez:

- perfil Hermes existente
- contrato operativo claro
- memoria alineada con el modelo Mugiwara
- gateway persistente o mecanismo equivalente
- límites de rol y escalado ya definidos

## 🚫 Qué no enseña este documento

Este documento no publica:

- systemd units literales
- IDs internos o direcciones sensibles
- wiring exacto del runtime
- configuración viva de perfiles
- secretos, `.env`, auth o credenciales
- estado crudo de memoria o sesiones

## 📌 Lectura honesta

La conclusión correcta no es “todo detalle de Mugiwara debe publicarse”.
La conclusión correcta es otra:

> ya existe una base operativa real más amplia y estable en este mini PC, con la tripulación canónica completa activa, pero la publicación pública sigue siendo deliberadamente progresiva y saneada.

Y eso, francamente, da más confianza que fingir que el barco entero ya está navegando a velocidad máxima. ⚓
