# 🧱 Architecture

## Vista de alto nivel

La nave pública se entiende mejor si separas sus grandes piezas. No hace falta ver cada remache del casco para entender por qué flota.

### 1. Hermes runtime
La capa de ejecución: perfiles, herramientas, automatización y superficie operativa donde viven los agentes.

### 2. Tripulación Mugiwara
Los agentes especializados no son “skins” del mismo bot con distinto peinado. Cada uno tiene alcance, criterios y contrato operativo propios.

Ejemplos del núcleo actual:

- **Luffy** → coordinación, priorización y cierre ejecutivo
- **Zoro** → software, arquitectura, implementación y verify técnico
- **Franky** → infraestructura, automatización y sistemas

### 3. Canon compartido
El vault curado actúa como historia oficial del barco: decisiones estables, summaries y conocimiento reutilizable.

### 4. Memoria por capas
No toda memoria merece el mismo destino. El modelo separa:

- memoria compacta de perfil
- memoria relacional compartida
- memoria técnica viva por proyecto
- canon duradero en vault

### 5. Capa de escaparate público
Este repositorio vive por encima del sistema real como una capa editorial filtrada.
No es un espejo; es una versión gobernada, segura y pensada para enseñar sin regalar munición.

## ⚙️ Principios de diseño

- **especialización sobre generalismo**
- **delegación explícita sobre improvisación borrosa**
- **verify sobre storytelling vacío**
- **canon curado sobre dump bruto**
- **publicación segura sobre exhibicionismo técnico**

## 🧭 Regla de lectura

Si una pieza parece demasiado abstracta, piensa esto:

- el sistema real es más rico que este repo
- este repo es más seguro que el sistema real
- y esa diferencia es intencional, no una carencia

En Grand Line no enseñas el mapa completo si quieres seguir flotando. 🗺️
