# 🚫 Publishing Policy

## Postura por defecto

**Deny by default.**

Si hay duda sobre si algo es seguro de publicar, se queda fuera.
No hay debate dramático, no hay moneda al aire y no hay “pero quedaba increíble”.

## ✅ Sí se puede publicar

- arquitectura de alto nivel
- descripciones abstractas de roles
- ejemplos saneados
- convenciones públicas seguras
- changelog y release notes editoriales
- diagramas sin detalle operativo sensible

## 🧼 Requiere saneado fuerte

- fragmentos de config
- extractos de prompts
- descripciones de workflows
- logs o screenshots
- ejemplos operativos

## ❌ No se publica

- secretos, tokens, cookies o credenciales
- contenidos de `.env`
- identificadores reales de runtime
- topología interna con detalle explotable
- memoria cruda o estado de sesión
- logs de producción
- prompts inseguros o lógica de bypass operativo

## 🧪 Checklist antes de publicar

Antes de hacer commit o release, verifica:

- que no haya material secreto
- que no aparezcan IDs operativos vivos
- que no haya rutas locales innecesarias
- que no se revele topología sensible
- que no se cuele runtime state
- que no haya metadatos ocultos en archivos o imágenes
- que el cambio aporte valor público real

## 🧠 Regla de desempate

Si una pieza aporta mucho color pero poca claridad, pierde.
Si una pieza aporta mucha claridad pero sube el riesgo, también pierde.
Solo zarpan los cambios que mejoran el escaparate **sin agrandar la superficie de exposición**.
