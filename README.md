# W.O.P.R. · War Operation Plan Response

Homenaje a **WarGames / Juegos de guerra (1983)**: la terminal de WOPR, el superordenador del NORAD, en el navegador.
Tiene pantalla de fósforo CRT, módem, voz sintetizada y los juegos de la película.

**Jugar:** https://pedritogrillo.github.io/wopr-1983/

## Cómo se juega

1. Pulsa una tecla para conectar: suenan los tonos de marcado y el módem.
2. En `LOGON:` puedes probar `HELP GAMES` o `LIST GAMES`… pero para entrar de verdad hace falta la puerta trasera del
   profesor Falken. *Pista: la contraseña es el nombre de su hijo.*
3. Contesta a Joshua como en la película y… *SHALL WE PLAY A GAME?*

## Juegos

| Juego | Qué hace |
|---|---|
| **GLOBAL THERMONUCLEAR WAR** | Eliges bando y objetivos. Las trayectorias rojas caen sobre los mapas ASCII de EE. UU. y de la URSS, y luego se pasa al mapa mundial del NORAD: DEFCON bajando, cientos de misiles en arco, impactos que se funden en destellos blancos y escenarios cada vez más rápidos con «WINNER: NONE»… hasta la frase final. |
| **TIC-TAC-TOE** | Tres en raya contra un WOPR que no pierde nunca. Con `LEARN` juega contra sí mismo, como en la película. |
| **FALKEN'S MAZE** | Laberinto aleatorio: muévete con las flechas o con W A S D. |
| **BLACK JACK** | Contra WOPR como crupier. |
| Juegos tácticos | Fighter Combat, Desert Warfare, etc. lanzan simulaciones con barras de progreso. |
| Juegos de mesa | Chess, Poker, Checkers… WOPR responde con ironía. |

## Comandos

`HELP` · `LIST GAMES` · `PLAY <juego>` o su número · `DEFCON` · `COLOR CYAN|GREEN|AMBER` · `SOUND ON|OFF` ·
`VOICE ON|OFF` · `CLS` · `LOGOFF`

## Técnica

Es un solo `index.html`, sin compilación. Usa la fuente VT323 (Google Fonts). Los mapas salen de
[world-atlas](https://github.com/topojson/world-atlas) a través de jsDelivr y se dibujan en un canvas. La voz es la
síntesis de voz del navegador y el sonido se genera con Web Audio.

Proyecto hecho por fans, sin relación con MGM ni con los autores de la película.
