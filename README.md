# code-along-css-grid-260923

Repetition av Grid innan vi går vidare till typsnitt, färger och variabler.
Samma layout byggd två gånger: en gång med linjer, en gång med areas.

HTML:en är identisk i båda mapparna. Det är bara CSS:en som skiljer.

## 1-grid-lines

Placera med `grid-column` och `grid-row`.

1. Öppna `1-grid-lines/index.html` i Live Server.
2. Titta på `grid-template-columns: 20rem 1fr 1fr`. Tre kolumner ger fyra linjer.
3. Läs `grid-column: 1 / 4` på header. Det är linje 1 till linje 4, inte tre kolumner.
4. Byt `1 / 4` mot `1 / -1`. Samma resultat, men nu behöver du inte räkna om när du lägger till en kolumn.
5. Jämför `grid-column: 2 / span 2` på main med `2 / 4`. `span` räknar spår, siffran räknar linjer.
6. KOMMENTERA BORT `grid-template-rows`. Nu ser du den implicita raden som aside skapar.

## 2-grid-areas

Samma layout, utan ett enda linjenummer.

1. Öppna `2-grid-areas/index.html`.
2. Läs `grid-template-areas`. Varje rad i citattecken är en rad i gridet, så CSS-koden blir en karta över sidan.
3. Byt `"nav aside aside"` mot `"nav . aside"`. Punkten är en tom ruta.
4. Dra ihop fönstret till under 600px. Kartan ritas om i media queryn.
5. Flytta `"nav"` över `"main"` i media queryn. Ordningen i HTML:en rörs inte.

## När väljer man vad?

Linjer när du placerar enstaka items i ett grid du redan har, som i bloggen vi gjorde igår.
Areas när du bygger en sidlayout med namngivna delar och vill kunna rita om den för mobil.

## Vidare

Övningarna efter passet ligger i [css-grid-fundamentals](https://github.com/chasacademy-sandra-larsson/css-grid-fundamentals) — gör övning 1 (grid-lines) och 2 (grid-area).

Fråga i kanalen om något krånglar!
