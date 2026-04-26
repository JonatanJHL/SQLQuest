# ⚔ SQL Quest

> Aprende SQL jugando un RPG de mazmorras. Escribe queries reales para moverte, atacar, curar y conquistar zonas.

<p align="center">
  <a href="https://play.google.com/store/apps/details?id=com.joatnjhl.sqlquest.app&hl=es">
    <img src="https://play.google.com/intl/en_us/badges/static/images/badges/es_badge_web_generic.png" alt="Disponible en Google Play" height="80"/>
  </a>
</p>

---

## ¿Qué es SQL Quest?

SQL Quest es un juego educativo de tipo RPG donde el jugador aprende SQL de forma progresiva mientras explora mazmorras generadas proceduralmente, combate enemigos y desbloquea nuevas zonas. Cada acción del juego se ejecuta mediante un comando SQL real.

```sql
-- Para moverte
UPDATE héroe SET posición = 'norte';

-- Para atacar
INSERT INTO ataque VALUES ('espada');

-- Para analizar el mapa
SELECT * FROM enemigos WHERE atk > 5;
```

---

## Modos de juego

### 📚 Modo Aprendizaje
- 13 lecciones progresivas con narrativa integrada
- Feedback inteligente: detecta el error exacto en tu query
- Scaffolding adaptativo: más ayuda cuando la necesitas, menos cuando dominas
- Retrieval Rooms entre zonas para consolidar lo aprendido
- Mini-quiz automático cada 3 lecciones

### ⚔ Modo Campaña
- Se desbloquea al completar todas las lecciones
- Sin chips, sin hints — SQL puro
- Enemigos más poderosos que exigen queries complejos
- Zonas exclusivas: Torre del SQL Maestro y Abismo del Caos

---

## Comandos SQL que aprenderás

| Comando | Zona | Uso en el juego |
|---|---|---|
| `SELECT *` | Caverna Inicial | Explorar el mapa |
| `UPDATE SET` | Caverna Inicial | Moverte por el mapa |
| `SELECT columna` | Pasillos del Conocimiento | Consultar tus stats |
| `WHERE` | Pasillos del Conocimiento | Filtrar enemigos |
| `INSERT` | Arena de Consultas | Atacar |
| `DELETE` | Arena de Consultas | Huir del combate |
| `COUNT` | Laboratorio de Análisis | Contar enemigos |
| `ORDER BY` | Laboratorio de Análisis | Ordenar inventario |
| `GROUP BY` | Laboratorio de Análisis | Agrupar items |
| `JOIN` | Torre del SQL Maestro | Cruzar la torre |
| `Subconsultas` | Torre del SQL Maestro | Derrotar al jefe |
| `HAVING` | Abismo del Caos | Modo campaña |
| `TRANSACTION` | Abismo del Caos | Modo campaña |

---

## Modelo pedagógico

El juego aplica 4 capas de aprendizaje basadas en la Taxonomía de Bloom y el modelo de Vygotsky:

1. **Exposición contextual** — El NPC introduce el comando dentro de la narrativa
2. **Práctica guiada** — Chips y hints visibles, feedback inmediato
3. **Práctica libre** — Sin chips, el jugador escribe solo
4. **Retrieval challenge** — Sin ninguna ayuda, memoria pura

El sistema adaptativo ajusta el nivel de scaffolding automáticamente: 3 errores consecutivos activan la ayuda, 3 aciertos consecutivos la desactivan.

---

## Características técnicas

- **Mapas procedurales** generados con algoritmo BSP por semilla
- **Pixel art** dibujado en Canvas nativo de Android (sin librerías externas)
- **Fog of war** con revelado progresivo por celda
- **Sistema de mastery** por comando: Visto → Practicado → Dominado → Retenido
- **Feedback inteligente** — detecta typos, falta de `;`, tablas incorrectas, orden de cláusulas
- **Sin internet requerido** — funciona 100% offline
- **Sin publicidad** — sin SDKs de terceros

---

## Stack

```
Kotlin 1.9
Android SDK 35 (minSdk 24)
AndroidX / Material Components 1.13.0
Canvas 2D API (pixel art nativo)
SharedPreferences (guardado local)
```

---

## Estructura del proyecto

```
app/src/main/java/com/joatnjhl/sqlquest/app/
├── GameData.kt        — Tipos, zonas, lecciones, quiz bank, sistema de mastery
├── GameEngine.kt      — Lógica del juego, SQL parser, feedback inteligente
├── MapGenerator.kt    — Generación BSP de mazmorras
├── MapView.kt         — Pixel art en Canvas nativo
└── MainActivity.kt    — UI programática, dos modos de juego
```

---

## Privacidad

SQL Quest no recopila ningún dato personal. Todo el progreso se guarda localmente en el dispositivo.

👉 [Política de Privacidad](https://TU_USUARIO.github.io/sqlquest-privacy/)

---

## Descarga

<a href="https://play.google.com/store/apps/details?id=com.joatnjhl.sqlquest.app&hl=es">
  <strong>Google Play Store →</strong>
</a>

---

## o miralo en tu equipo(versión no actualizda)

Abre index.html en tu navegador

Usa comandos SQL para moverte, investigar y combatir:

---

## Licencia

Este proyecto fue desarrollado como herramienta educativa.  
© 2026 Jonatan Hidalgo — Todos los derechos reservados.
