# 🎱 Bingo Costa Rica

Tablero de bingo interactivo diseñado para proyectarse en televisores durante partidas en vivo. Desarrollado con HTML, CSS y JavaScript puro — sin dependencias externas.

## ¿Qué hace?

- Tablero de 75 números organizados en filas B-I-N-G-O
- Múltiples **modos de juego** seleccionables antes de cada partida (4 esquinas, La T, La X, El marco, Cartón lleno, etc.)
- Marca el **último número cantado** en grande debajo del tablero
- **Narrador de voz** opcional con 4 personajes (Diego, Juana, Esteban, Gladis), cada uno con sus propios dichos clásicos de bingo
- Los modos jugados se marcan y se mueven al fondo del panel lateral
- Botones de **Reiniciar** (con confirmación) y **Deshacer**

## Tecnologías

- HTML / CSS / JavaScript vanilla
- Audios generados con [ElevenLabs](https://elevenlabs.io) e integrados en base64 dentro de `script.js`
- Desplegado en [Vercel](https://vercel.com)

## Estructura

```
index.html   → estructura de la app
styles.css   → estilos (tema navy oscuro optimizado para TV)
script.js    → lógica del juego + audios de los narradores en base64
```

## Narradores

Los audios se generaron con ElevenLabs usando voces creadas en Voice Design. Para regenerarlos o agregar más narradores, usar el script `generar_4_narradores.py` de la carpeta `archivos/` (no incluida en el repo).

Los créditos de ElevenLabs se renuevan mensualmente. Los dichos y textos de cada narrador están en el mismo script.

## Modos de juego disponibles

| Modo | Descripción |
|---|---|
| 4 esquinas | Las 4 celdas de las esquinas |
| La T | Fila superior + columna central |
| Línea horizontal | Cualquier fila completa |
| Línea vertical | Cualquier columna completa |
| Línea diagonal | Cualquiera de las dos diagonales |
| La X | Ambas diagonales cruzadas |
| La H | Dos columnas laterales + fila central |
| La L | Columna izquierda + fila inferior |
| La M | Columnas externas y diagonales superiores |
| La C | Fila superior, inferior y columna izquierda |
| El marco | Todo el borde del cartón |
| Cartón lleno | Todas las celdas |
| Libre | Figura acordada entre los jugadores |