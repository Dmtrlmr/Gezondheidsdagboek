# 🍽 Voedingsdagboek — PWA

Persoonlijke app om maaltijden en klachten bij te houden. AI detecteert patronen tussen voeding en spijsverteringsklachten.

## Bestanden

```
voedingsdagboek/
├── index.html      ← de volledige app
├── manifest.json   ← PWA-configuratie
├── sw.js           ← service worker (offline werking)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## Installeren via GitHub Pages

### Stap 1 — GitHub repository aanmaken
1. Ga naar [github.com](https://github.com) en log in (of maak een gratis account)
2. Klik op **New repository**
3. Naam: `voedingsdagboek` (of een andere naam naar keuze)
4. Zet op **Public**
5. Klik **Create repository**

### Stap 2 — Bestanden uploaden
1. Klik op **uploading an existing file**
2. Sleep alle bestanden én de `icons/`-map naar het uploadvenster
3. Klik **Commit changes**

### Stap 3 — GitHub Pages activeren
1. Ga naar **Settings** → **Pages**
2. Onder *Source*: kies **Deploy from a branch**
3. Branch: **main**, map: **/ (root)**
4. Klik **Save**
5. Na ~1 minuut is de app beschikbaar op:
   `https://JOUWGEBRUIKERSNAAM.github.io/voedingsdagboek/`

### Stap 4 — Toevoegen aan iPhone-startscherm
1. Open de URL hierboven in **Safari** op je iPhone
2. Tik op het **Deel-icoon** (vakje met pijltje omhoog)
3. Scroll naar beneden → **Zet op beginscherm**
4. Naam: "Dagboek" → **Voeg toe**

De app verschijnt nu als icoon op je startscherm en opent fullscreen, zonder adresbalk.

## Gegevens

Alle data wordt lokaal opgeslagen op je apparaat (localStorage). Er worden geen gegevens naar een server gestuurd, behalve bij de AI-analyse (anoniem naar Anthropic API).

## Aanpassen

De volledige app staat in `index.html` — één bestand, geen build-stap nodig.
