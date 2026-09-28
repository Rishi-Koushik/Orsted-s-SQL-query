# Orsted's SQL Journey

A browser RPG that teaches SQL, set in the world of *Mushoku Tensei*. You play as Orsted, the Dragon God. You walk a tile-based world, solve rune stones by writing real SQL queries, and fight bosses whose seals only break when your queries are correct.

It's a single HTML file with no install, no server and no build step. Open it in a browser and play, even offline.

## How it plays

- **43 rune stones across 6 regions.** Each stone gives you a short lesson, a task and a live query editor. Your query runs against a real SQLite database in the browser and is graded on the rows it returns.
- **5 Dragon Vaults.** Clearing a region's vault opens the road to the next region.
- **6 side bosses.** These are optional bullet-dodging fights with spells. Each boss is guarded by 2 SQL seals that test harder mixes of what its region taught. Beating one gives you a permanent blessing for later fights.
- **Final boss: Hitogami.** Three seals, three SQL challenges.
- **Theory panel.** A toggle next to Hint. It explains how each concept works, how the database runs it, the syntax and common mistakes, and has a separate explanation and example for each function. There are 38 topics, and you can browse them all from the Codex.
- **3 save slots.** Continue, Load game and a pause menu (save, copy to another slot, quit to title). Transfer codes move a save between devices.
- **Phone support.** An on-screen D-pad and a SQL keyword bar above the keyboard.

## What it covers

| Region | SQL topics |
|---|---|
| Fittoa | `SELECT`, `WHERE`, `ORDER BY`, `DISTINCT`, `LIMIT` |
| Sharia | `LIKE`, `IN`, `BETWEEN`, `IS NULL`, `CASE`, string, number and date functions |
| Begaritt | `COUNT`/`SUM`/`AVG`/`MIN`/`MAX`, `GROUP BY`, `HAVING` |
| Rikarisu | `INNER`/`LEFT`/self joins, `UNION`, `INTERSECT`, `EXCEPT` |
| Chaos Breaker | Subqueries, `EXISTS`, CTEs, recursive CTEs, window functions |
| The Void | `INSERT`, `UPDATE`, `DELETE`, `CREATE TABLE`, indexes, views, transactions |

## Play

Download `orsteds-sql-journey.html` and open it in any modern browser.

## Controls

| Key | Action |
|---|---|
| W A S D / arrows | Move (Shift to run) |
| E | Read a stone, enter a lair |
| Enter | Run your query (Shift + Enter for a new line) |
| 1 2 3 4 | Spells in boss fights |
| C | Codex |
| Esc | Pause menu, or retreat from a fight |

## Built with

- HTML5 Canvas and vanilla JavaScript, with no frameworks
- [sql.js](https://github.com/sql-js/sql.js), which is SQLite compiled to JavaScript and bundled inside the file
- `localStorage` for save slots

## Disclaimer

This is a non-commercial fan project made for learning. *Mushoku Tensei* and its characters belong to Rifujin na Magonote and their respective rights holders. All art in the game is drawn in code and is original.
