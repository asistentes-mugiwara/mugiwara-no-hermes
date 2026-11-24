# 🧱 Arquitectura de Mugiwara

Hermes es la capa de ejecución de agentes; Mugiwara define cómo se reparte el trabajo y cómo se conserva lo aprendido. La consola es una aplicación separada que consulta el estado del sistema. Este repositorio explica ese modelo: no contiene el runtime ni levanta la consola.

## De una petición a un resultado verificable

1. **Coordinar.** Cuando una petición cruza dominios, Luffy fija el objetivo y deriva el trabajo al especialista adecuado con alcance, restricciones y criterio de cierre. El rol describe una responsabilidad; el perfil es su configuración de ejecución. Ninguno demuestra por sí solo que haya un proceso o servicio activo. Véanse el [contrato de delegación](workflow-model.md#2-delegación-a-especialistas) y los [estados documentados](deployment-status.md).
2. **Ejecutar y verificar.** El especialista trabaja en Hermes con las herramientas autorizadas para la tarea. Una skill recoge un procedimiento reutilizable, no concede permisos adicionales. En software, por ejemplo, CodeGraph ayuda a estudiar el impacto antes de cambiar código; la evidencia del resultado viene de la [verificación](sdd-model.md), no de haber cargado una herramienta o seguido una fase.
3. **Conservar solo lo que corresponda.** El resultado vuelve a quien coordina o pidió el trabajo. Si hace falta continuidad, el tipo de información determina su destino: respaldo de perfil, contexto relacional, continuidad técnica de proyecto o canon curado para decisiones duraderas. Son capas con fines distintos, no pasos obligatorios ni copias automáticas. Véase [memoria por capas](operations-safeguards.md#3-memoria-por-capas).
4. **Observar por separado.** La consola sirve para consultar el estado; no dirige la delegación. Una vista de estado no demuestra que se haya atendido una petición concreta.

## Cómo revisar el mapa sin acceso privado

| Tipo de evidencia | Dónde mirar y qué permite concluir |
| --- | --- |
| **Implementado** | La [página del control plane](control-plane.md) documenta la consola como pieza software separada y distingue el código público del uso privado. Es una referencia sobre qué se ha construido, no una prueba de despliegue ni de disponibilidad actual. |
| **Modelo documentado** | El [roster](crew-roster.md) describe responsabilidades y el [estado documentado](deployment-status.md) distingue entre lo definido, lo configurado y lo observado. El modelo no acredita actividad actual. |
| **Histórico** | OpenCode es una influencia en la práctica de entrega software. El nombre `sdd-model.md` conserva esa historia; las fases formales son una opción, no un requisito del runtime ni de cada cambio. |
| **Ejemplo** | El ejemplo sintético [`public-demo-config.yaml`](../examples/public-demo-config.yaml) ilustra el reparto de roles y la política de publicación. No configura un despliegue de Hermes. |
| **Privado** | La configuración efectiva, los datos vivos, las fuentes operativas y el acceso al panel quedan fuera. Una captura, un ejemplo o un valor de fallback no sustituyen evidencia de ejecución. Véase [sistema frente a escaparate](system-vs-showcase.md). |
