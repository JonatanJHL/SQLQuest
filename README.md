# SQL Quest — Aprende SQL Jugando

Un juego RPG educativo donde aprendes SQL/MySQL mientras exploras un dungeon, combates enemigos y resuelves puzzles usando comandos SQL reales.

> ⚠️ **Uso educativo exclusivamente** — Para escuelas, universidades y aprendizaje personal. Sin fines de lucro.

## 🎮 Cómo Jugar

1. Abre `sql_quest_rpg_v2.html` en tu navegador
2. Usa comandos SQL para moverte, investigar y combatir:

```sql
SELECT * FROM mapa;                    -- Ver posición y caminos
UPDATE heroes SET position = 'north'; -- Moverse al norte
SELECT hp FROM heroes;                 -- Ver vida actual
INSERT INTO attack;                  -- Atacar enemigo
SELECT * FROM inventory;             -- Ver objetos
UPDATE heroes SET hp = hp + 30;       -- Curarse (con poción)
DELETE FROM combate;                -- Huir del combate
```

## 📚 Plan de Estudios (10 Niveles)

| Nivel | Tema SQL | Desafío |
|-------|---------|---------|
| 1 | `SELECT *`, `FROM`, `UPDATE` | Exploración básica — llegar a la salida |
| 2 | `SELECT columna` | Buscar objeto específico con columna |
| 3 | `WHERE`, `>`, `<`, `=`, `!=` | Filtrar enemigos por estadísticas |
| 4 | `ORDER BY`, `LIMIT` | Encontrar mejor loot |
| 5 | `AND`, `OR`, `NOT` | Lógicas complejas |
| 6 | `COUNT`, `SUM`, `AVG` |统计分析 |
| 7 | `GROUP BY`, `HAVING` | Agrupar por tipo |
| 8 | `JOIN`, `INNER`, `LEFT` |Combinar tablas |
| 9 | Subqueries | Consultas anidadas |
| 10 | `CASE`, `INDEX` | Nivel avanzado |

## 🛠️ Requisitos

- Navegador moderno (Chrome, Firefox, Edge, Safari)
- **NO requiere servidor** — funciona offline

## 📁 Estructura del Proyecto

```
sqlQuest/
├── sql_quest_rpg_v2.html   (Juego completo)
├── README.md              (Este archivo)
└── LICENSE             (Licencia)
```

## 📜 Licencia

**Uso educativo no lucrativo** — Ver archivo `LICENSE`.

---

## 🤝 Cómo Contribuir

1. Fork el repositorio
2. Crea una rama (`git checkout -b feature/nueva`)
3. Commit tus cambios
4. Push a GitHub
5. Abre un Pull Request

## ⭐ Créditos

- **Desarrollador**: JonatanJHL
- **Inspiración**: SQL RPG Mystery, Select Star SQL

---

*SQL Quest — Aprende SQL jugando, explora el dungeon, conviértete en maestro SQL.*
