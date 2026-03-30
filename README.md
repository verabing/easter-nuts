# Påskekalender light

Dette er en forenklet påskekalender laget for GitHub Pages.

## Struktur

- `index.html` – hovedfilen
- `lang/` – språkfiler (`no.json`, `en.json`, `de.json`)
- `bilder/` – legg bilder her hvis du vil bruke egne illustrasjoner
- `flags/` – flaggikoner til språkvalg hvis du vil bygge det ut visuelt
- `reminders/` – korte innholdsnotater og publiseringshjelp
- `bakgrunn.jpg` – bakgrunnsbilde brukt av siden
- `favicon.ico` – ikon i nettleseren

## Light-versjonen

Denne versjonen har 5 dører:

1. Skjærtorsdag
2. Langfredag
3. Påskeaften
4. 1. påskedag
5. 2. påskedag

Datoene ligger i `index.html` i `calendarConfig`.

## Slik tilpasser du innholdet

### 1. Endre tekstene i dørene

Åpne språkfilene i `lang/` og rediger tittelen og teksten for hver dør.

### 2. Endre datoene

I `index.html` finner du dette feltet:

```js
const calendarConfig = [
  { id: 1, key: 'maundyThursday', date: '2026-04-02' },
  { id: 2, key: 'goodFriday', date: '2026-04-03' },
  { id: 3, key: 'holySaturday', date: '2026-04-04' },
  { id: 4, key: 'easterSunday', date: '2026-04-05' },
  { id: 5, key: 'easterMonday', date: '2026-04-06' }
];
```

Bytt til årets påskedatoer ved behov.

### 3. Endre utseende

- bytt `bakgrunn.jpg`
- juster farger i `<style>` i `index.html`
- legg inn egne bilder eller lenker i dørteksten

## GitHub Pages

1. Lag et nytt repository, for eksempel `paaskekalender-light`
2. Last opp alle filene i denne mappen
3. Gå til **Settings > Pages**
4. Velg branch `main` og root `/`
5. Lagre

Da publiseres siden som en statisk nettside.

## Neste steg

Hvis du vil bygge videre fra denne light-versjonen, er de mest naturlige retningene:

a) bare bytte tekst og bilder
b) gjøre dørene mer visuelle med illustrasjoner
c) legge inn lyd, dikt eller små oppgaver i hver dør


## Ny UI-retning

Denne versjonen bruker en kurv med fem mønstrede egg. Når et egg åpnes, blir det liggende som sprukket skall i kurven, og dagens bilde samles separat i galleriet. Standard plassholderbilder ligger i `bilder/egg-1.svg` til `bilder/egg-5.svg` og kan erstattes med egne bilder med samme filnavn.
