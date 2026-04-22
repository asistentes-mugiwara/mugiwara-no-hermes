# 🛡️ Security Policy

## Alcance

Este repositorio es un **escaparate público saneado** de un sistema multiagente real.

Eso significa que la seguridad manda más que la completitud: preferimos contar un poco menos antes que enseñar algo que no debíamos.

## 🚨 Cómo reportar un problema

Si crees que algo sensible, peligroso o demasiado revelador se ha publicado aquí por error:

1. **no abras una issue pública** con el material sensible
2. contacta por privado con la cuenta propietaria del repositorio si te es posible
3. indica la ruta afectada y el tipo de exposición, **sin repetir el secreto**
4. si hay duda, asume que la prioridad es retirar primero y discutir después

## ⚖️ Política de respuesta

- el material sensible debe retirarse rápido
- las redacciones por seguridad son válidas y esperables
- la seguridad operativa está por encima de la completitud pública
- si una sección “quedaba increíble” pero expone demasiado, se va por la borda

## 🔍 Qué vigilamos especialmente

- secretos, tokens, cookies y credenciales
- `.env` y configuración de producción
- logs reales o estados de sesión
- topología interna con detalle explotable
- rutas, IDs, endpoints o metadatos innecesariamente reveladores
- prompts o bypasses operativos que acerquen demasiado al runtime real

## 🧠 Regla práctica

> Si un detalle ayuda poco a entender y mucho a atacar, sobra.
