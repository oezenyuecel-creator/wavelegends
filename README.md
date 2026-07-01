# WAVE LEGENDS 🌊

Ein **Surf-Endless-Adventure** im Stil von *Alto's Odyssey × Fortnite-Farben × Disney-Licht*.
Eigenständiger One-File-Prototyp — `index.html` öffnen, surfen. Keine Build-Tools, keine Dependencies, keine Assets (alles prozedural gezeichnet & vertont).

> Status: **v0.1 – spielbarer Vertical-Slice.** Der Kern (Surf-Feeling, Tricks, Wetter-Biome, Boss, Progression) steht und macht Spaß. Die große Vision (3D, echtes Live-Ops, Multiplayer) ist bewusst **nicht** enthalten — siehe [Roadmap](#roadmap-zur-vollen-vision).

---

## Vision
Der Spieler ist ein Surfer, der ein **lebendiges Meer** abreitet. Das Meer ist der Hauptcharakter: es
verändert Wellenhöhe, Licht, Wetter und Tageszeit. Keine Runde fühlt sich gleich an. Leicht zu lernen,
schwer zu meistern — die klassische „nur-noch-ein-Run"-Schleife.

## Steuerung (One-Button, mobile-first)
- **HALTEN** = die Wellenflanke *anpumpen* → Speed aufbauen; am Kamm abheben (loslassen = Absprung-Pop für höhere Airs)
- **In der Luft HALTEN** = **Flip/Rotation** (Trickpunkte) → rechtzeitig loslassen, um sauber & gerade zu landen
- **In der Luft kurz TIPPEN** = **Grab** (Style-Punkte ohne Rotationsrisiko)
- **Sauber landen** = Combo läuft weiter + kleiner Speed-Boost. Schief landen = **Wipeout** (Combo weg, Speed bricht ein)
- Desktop-Test: `Leertaste` / `Pfeil-runter` = Halten, `P` = Pause, `M` = Ton

## Der Clou: die Monsterwelle 🌊
Statt „einmal berührt = tot" jagt dich eine **riesige Monsterwelle** von hinten. Hindernisse killen dich
nicht sofort — sie verursachen **Wipeouts**, die dich verlangsamen, sodass die Welle aufholt. **Speed &
saubere Tricks = Überleben.** Fair, spannend und thematisch perfekt fürs Surfen.

**Ausnahme: der Hai. 🦈** Er ist selten, kündigt sich mit pulsierender roter Warn-Aura an — und frisst
dich bei Berührung sofort (drüberspringen = sicher, Schild frisst stattdessen den Hai).

## Was schon drin ist (v0.1)
- **Surf-Physik**: prozedurale Wellen-Oberfläche (mehrschichtige Sinus-Swells), Anpumpen der Flanke, Absprung am Kamm, Flugphase, Landungs-Bewertung
- **Trick- & Combo-System**: AIR · BACKFLIP · 360°/720° SPIN · **GRAB** (Tippen in der Luft) · SUPER AIR — Kombis wie „BACKFLIP + GRAB"; je länger die Combo, desto höher der Multiplikator (`x1.5`, `x2.0` …)
- **Game Feel**: Surfer-Posen (Hocken beim Pumpen, Tuck im Flip, Grab-Pose, Jubel nach Trick-Landung), **Zeitlupe + Kamera-Zoom** bei großen Airs und beim knappen Hai-Überspringen („KNAPP! +10"), Vibration auf dem Handy
- **5 Wetter-Biome** mit weichem Übergang & eigenem Look/Licht/Sound:
  - 🏝️ **Tropische Bucht** — Sonne, volumetrische Strahlen, Palmeninseln, Möwen
  - 🌅 **Goldener Sonnenuntergang** — warme Farben, tiefe Sonne
  - ⛈️ **Sturmsee** — Regen, Blitze, Nebel, höhere Wellen
  - 🌌 **Biolumineszente Nacht** — Sterne, Mond-Glow, leuchtendes Wasser
  - 🌈 **Polarlichter** — wogende Aurora-Bänder, eisige Palette
- **Boss-Setpiece**: ⚠ **KRAKEN** — Tentakel-Walls, über die du springen musst (+Perlen-Belohnung)
- **Sammeln**: Perlen (Währung, teils knapp über dem Wasser sammelbar, teils als Air-Bögen) & Goldmünzen
- **Power-Ups**: 🧲 Magnet · 🛡 Schild · ⚡ Turbo · ★ Unbesiegbar (mit HUD-Anzeige + Timer)
- **Missionen & Daily Challenge** 🎯: 3 aktive Missionen (Pool von 18: Distanz, Perlen, Tricks, Flips, Grabs, Combos, Hai-Near-Miss, Boss, „ohne Wipeout" …) — erfüllte werden nach dem Run automatisch ersetzt; dazu täglich 1 ★ Tages-Challenge mit großem Perlen-Bonus. Fortschritt zählt live im Run, Belohnung kommt sofort mit Banner.
- **Progression**: Perlen fließen in ein dauerhaftes Konto (localStorage), Highscore, Run-Zähler
- **Shop** (fair, **kein Pay-to-Win**): 6 Boards & 5 Surfer — nur leichte Gameplay-Tweaks + kleine Perks
- **Juice**: Gischt/Foam/Partikel, Screenshake, schwebende Score-Popups, Biom-Banner, Barrel/Tube-Effekt beim schnellen Abtauchen, Turbo-Flammen-Trail
- **Prozeduraler Sound** (Web Audio, keine Dateien): Wellen-Bett + Ambient-Pad, das den Akkord pro Biom wechselt, plus SFX für Sprung/Landung/Sammeln/Trick/Crash. Ton per `M` oder Menü an/aus
- **Mobile-first**: Fullscreen-Canvas, DPR-scharf, Touch-Steuerung, 60-FPS-Ziel

## Boards & Surfer
| Boards | Surfer (Perks) |
|---|---|
| Holz · Retro · Carbon · Feuer · Kristall · Drachen | Kai · Luna (Startschild-Chance) · Reef (Magnet länger) · Storm (vergebendere Landung) · Aya (+10 % Perlen) |

Alle per Perlen freischaltbar. Tweaks sind bewusst klein — Skill schlägt Ausrüstung.

## Starten
```bash
# einfach die Datei öffnen …
open index.html
# … oder lokal serven:
npx serve .
```

## Roadmap zur vollen Vision
Der ausführliche Ziel-Prompt beschreibt ein AAA-Studioprojekt (mehrere Mannjahre). Nächste sinnvolle Schritte auf diesem Fundament:
- [ ] Mehr Bosse mit echten Phasen (Riesenkalmar, Weißer Hai, Poseidon)
- [ ] Gegner-KI-Varianten (jagende Haie, Barrakuda-Schwärme, Geisterschiffe)
- [ ] Geheimnisse & Zufalls-Events (Höhlen, Wracks, seltene Tiere, Delfin-Begleiter)
- [ ] Missionen (täglich/wöchentlich), Achievements, Ränge, Fähigkeitenbaum
- [ ] Ghost-Rennen & Bestenlisten (async Multiplayer), Saison-Events, Battle Pass (kosmetisch)
- [ ] Cloud-Save, Lokalisierung, Barrierefreiheit, Haptik
- [ ] Portierung auf eine 3D-Engine (Unity/Unreal) oder WebGL für das spektakuläre Wasser

## Tech
Reines HTML5 + Canvas 2D + Web Audio API. Eine Datei, ~1.400 Zeilen, keine externen Libraries.
Komponentenartig strukturiert (Biome · Ocean · Player-Physik · Entities · Boss · Partikel · Audio · UI-Screens).

---
*Prototyp — Feedback & Balance-Tuning willkommen.*
