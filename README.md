# Trix Card Tracker

Spåra och bocka av spelade kort i **Trix** under pågående spel – med ett enda klick. Inga data skickas någonstans; allt sparas lokalt i webbläsaren.

![Trix Card Tracker](icon.svg)

## Funktioner

- **52 kort i 4 färggrupper** – Hjärter, Ruter, Spader och Klöver (2 till Ess) i pokerstil
- **Ett-klicksavbockning** – spelat kort blir nedtonat och överstruket direkt
- **Live-räknare** – hur många kort som återstår totalt och per färg, med progressbar
- **Varningar & färgstatus** – pulserande röd varning när en färg har ≤3 kort kvar, grön bock när en färg är avklarad
- **Autosave** – leken sparas automatiskt och finns kvar efter stängning
- **Ångra** – knapp eller `Ctrl+Z`
- **Rike-filter** – kombinera fokus på Hjärter Kung, Damer, Ruter eller Spader
- **Highlights** – guldmarkering av Damer, röd markering av Hjärter Kung och Ruter-kort
- **Ljud & animationer** – klickljud och flipp-animation (avstängningsbart)
- **Installeras som app (PWA)** – egen ikon och offline-stöd

## Kom igång

Öppna `index.html` direkt i din webbläsare – allt fungerar utan installation.

### Installera som Windows-app (PWA)

1. Starta en lokal server i mappen:

   ```
   python -m http.server 8080
   ```

2. Öppna [http://localhost:8080](http://localhost:8080) i Chrome eller Edge.
3. Klicka på *installera*-ikonen i adressfältet (eller `Installera app`-knappen när den visas).

## Genvägar

| Tangent | Funktion |
| --- | --- |
| `Ctrl+Z` | Ångra senaste klick |
| `R` | Återställ alla kort |

## Filstruktur

```
index.html            Appen (HTML + CSS + JavaScript)
manifest.webmanifest  PWA-manifest
sw.js                 Service worker (offline-stöd)
icon.svg              App-ikon
```