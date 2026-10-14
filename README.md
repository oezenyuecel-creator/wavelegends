# WAVE LEGENDS 🌊

Ein **Surf-Endless-Adventure** im Stil von *Alto's Odyssey × Fortnite-Farben × Disney-Licht*.
Eigenständiger One-File-Prototyp — `index.html` öffnen, surfen. Keine Build-Tools, keine Dependencies, keine Assets (alles prozedural gezeichnet & vertont).

> Status: **v0.1 – spielbarer Vertical-Slice.** Der Kern (Surf-Feeling, Tricks, Wetter-Biome, Boss, Progression) steht und macht Spaß. Die große Vision (3D, echtes Live-Ops, Multiplayer) ist bewusst **nicht** enthalten — siehe [Roadmap](#roadmap-zur-vollen-vision).

---

## Vision
Der Spieler ist ein Surfer, der ein **lebendiges Meer** abreitet. Das Meer ist der Hauptcharakter: es
verändert Wellenhöhe, Licht, Wetter und Tageszeit. Keine Runde fühlt sich gleich an. Leicht zu lernen,
schwer zu meistern — die klassische „nur-noch-ein-Run"-Schleife.

## Langzeit-Motivation
Ein Tester hatte nach ~26 Läufen (~19 min) alles gekauft. Deshalb gibt es jetzt:
- **Surfer-Rang**: Jeder Lauf gibt XP (Distanz, Tricks, Flips, Kraken, Events, Missionen) → Level mit Titeln (Anfänger → Wasserratte → … → Wave Legend bei Lv 50, danach endlos weiter). Jeder Aufstieg: Perlen; Lv 10/25/40: exklusive Trails.
- **Erfolge** 🏆: 12 Disziplinen × Bronze/Silber/Gold (36 Medaillen), z. B. Flip-Meister, Kraken-Jäger, Hai-Flüsterer, Dauersurfer. Belohnung: 100/300/750 Perlen; Gold-Stufen schalten Trails frei, die man nicht kaufen kann. Neue Erfolge erscheinen sofort im Lauf (Banner-Warteschlange) und in der Auswertung.
- **Trails**: 8 Spuren hinter dem Board (Gischt, Sternenstaub, Feuer, Regenbogen, Leuchtspur, Kraken-Tinte, Perlenkette, Goldspur) – nur erspielbar.
- **Power-Up-Upgrades**: Magnet/Turbo/Stern länger, Schild öfter schon beim Start – je 5 Stufen (500 → 8.000 Perlen), nur für Perlen, nie für Echtgeld.
- **Tägliche Belohnung**: 7-Tage-Serie (100 → 1.000 Perlen, Tag 7 zusätzlich +5 💎), verpasster Tag = von vorn.
- **Sammel-Kollektion mit Effekten** 💎: 6 Boards (Prisma, Frost, Blitz, Königs-Board, Phönix mit Flammen, Galaxie) und 6 Surfer (Jack der Pirat, Shadow der Ninja, Robo, Merlin der Zauberer, Blaze mit Heldenumhang, Coral mit Krone & Aura) in den Stufen Selten/Episch/Legendär. Seltene für Perlen, Epische (💎 20–25) und Legendäre (💎 50–60) nur für **Kristalle** — selten hoch in der Luft (guter Sprung nötig), +1 pro Kraken, +2/+5 für Silber/Gold-Erfolge, +3 alle 5 Level, +5 an Tag 7. Alles reine Optik (Werte wie das Holzboard). Shop mit Live-Vorschau, Seltenheits-Leiste und Sammlungs-Zähler; dein aktueller Surfer steht als Schaustück im Menü.
- Bestehende Spielstände bekommen Start-XP fürs bisherige Spielen, schon erreichte Rekorde zählen sofort als Erfolge. Shop und Erfolge sind scrollbar (Knöpfe lösen erst beim Loslassen ohne Wischen aus).

## Bonus-Level (eigener Modus, Hauptspiel unverändert)
Über „🧜 Bonus" im Menü. **Tickets**: täglich 1× gratis, +1 für jeden Lauf, in dem der Kraken besiegt wird (max. 5).
- **🧜 Meerjungfrauen-Lagune** (spielbar): Unterwasser-Höhlen mit Lichtstrahlen und Leuchtpflanzen. Eine Meerjungfrau schwimmt voraus, ihre Perlenspur ist der Weg. Steuerung: HALTEN = abtauchen, LOSLASSEN = aufsteigen. **Kein Game Over**: Luft (40 s, Luftblasen +2,5 s) läuft ab, Quallen kosten nur Perlen. Perlen zählen doppelt, dazu ein Kristall (mit 💎-Vorankündigung am Rand) und eine **goldene Muschel** – die Meerjungfrau taucht zu ihr hinab. 5 Muscheln = exklusives **Schuppen-Board**.
- **🦈 Hai-Jagd**: Korallenschlucht im Sonnenuntergang, ein Riesenhai jagt dich 35 s lang. Er wechselt Takt und Richtung (schnappt von hinten, doppelt, oder taucht ab und kommt von vorn), aber jeder Angriff wird gleich angekündigt: Ein **Ring um den Surfer** füllt sich – wird er **grün**, tippen = springen (◀/▶ zeigt die Richtung, von vorn zusätzlich 🦈 am Rand). Perlenbögen liegen genau auf der idealen Sprungbahn, „PERFEKT!" gibt +5. **Kein Game Over**: ein Biss kostet 15 Perlen, nach 3 Bissen endet die Flucht früher, die Beute bleibt. Durchhalten = Jackpot (+60) und ein **Haizahn** 🦷 → 5 Haizähne = exklusives **Haizahn-Board**.
- **🐉 Leviathan-Ritt**: Nachts im Sturm (Regen, Blitze) surfst du auf dem Rücken eines Seeungeheuers. Steuerung wie im Hauptspiel: **HALTEN = Schwung holen, LOSLASSEN = springen** – zwischen den Buckeln liegt Wasser, das bremst (reinfallen kostet ⅓ Tempo, kurze Gnadenfrist am Rand). Landung auf dem Abhang = „Sauber!" (+Tempo). Ab und zu schüttelt er sich und Schätze schweben herab. **Finale**: Er hebt den Kopf und schleudert dich hoch – mit genug **Schwung** (Marke 💎 in der Anzeige) fliegst du durch den Kristallring (💎 +1, ◐ +40). Jeder Ritt bringt eine **Sturmperle** ⚡ → 5 = exklusive **Sturmblitz-Spur**.
Fairness auf Handy-Breite (375 px) mit Bots gemessen:
- Lagune: Muschel 16/16, Kristall 12/16 (0,3 s Reaktion).
- Hai-Jagd: Wer auf „Ring wird grün" mit 0,22–0,38 s reagiert, übersteht 30/30 Fluchten, mit 0,45 s noch 27/30; Nicht-Tippen oder Wild-Tippen endet nach ~10–15 s. Gute Spieler ~340–355 Perlen, langsame ~195.
- Leviathan: Loslassen irgendwo zwischen 0,7 s vor dem Wasser und dem Wasserrand trifft den Ring in 7–8 von 8 Ritten; Dauer-Halten oder Nichtstun schafft den Ring nie. Perlen je nach Präzision ~195–390.
Die exklusiven Teile sind reine Optik; das Hauptspiel (Physik, Spawns, Balance, HUD) ist unverändert.

## Surf-Schule (Tutorial)
Beim ersten Start führt eine Mitmach-Schule in 5 Schritten durch das Spiel — jeder Schritt wartet, bis man ihn
geschafft hat: ① Halten = Speed (⚡-Balken leuchtet) · ② Loslassen = Springen · ③ echter Fels mit ⚠-Warnung
(„gleich …" → „JETZT!") · ④ Flip in drei geführten Teilschritten mit Zeitlupe · ⑤ die Monsterwelle. Ein
Daumen-Hinweis unten zeigt immer, was zu tun ist. Währenddessen keine Haie/Bosse, die Welle frisst nicht;
danach geht es nahtlos in den echten Lauf („LOS GEHT'S!"). Überspringbar, im Menü über „❓ Surf-Schule"
jederzeit wiederholbar.

## So wirst du gut
- **Speed aufbauen**: auf der Welle **gedrückt halten** — du pumpst die Abwärts-Flanke runter (fast doppelt so schnell wie ohne) und verlierst bergauf kaum Tempo. Der ⚡-Balken oben links zeigt es. Nur zum **Springen** loslassen, am besten oben am Wellenkamm.
- **Perfekter Flip**: abspringen → in der Luft **neu drücken und halten** → das Board dreht mit festem Tempo (ein Flip ≈ ½ Sekunde) → **loslassen, sobald der Ring um den Surfer GRÜN ist**. Loslassen stoppt die Drehung sofort, ein Lande-Assistent richtet das Board auf die Welle aus. Bei Mini-Hüpfern (Ring bleibt rot) lieber nicht flippen.
- **Tricks geben Speed**: jeder gelandete Flip beschleunigt dich zusätzlich (+6 % pro Flip).

## Gratis & Vollversion (keine Werbung, nie)
Modell „kostenlos starten, einmal zahlen":
- **Gratis**: Tropenbucht, Sonnenuntergang, Sturmsee mit Kraken, Missionen und Daily Challenge. Kein harter Stopp: Nach der Sturmsee surft man ein paar Sekunden **echt in die biolumineszente Nacht** (Banner „🌙 Vorgeschmack"), dann wird es wieder Tag in der Tropenbucht — Gratis-Spieler surfen endlos um den Highscore. Kein Fenster mitten im Lauf, nichts zum Anklicken.
- **Vollversion (Einmalkauf, Platzhalter 3,99 €)**: 🌙 Biolumineszente Nacht + Polarlichter, 🌠 Sternschnuppen-Events, Nachtsurfer-Paket (Surferin **Nova** mit leuchtendem Anzug + **Polarlicht-Board**, reine Optik, gleiche Werte wie das Holzboard: Echtgeld kauft nie Vorteile).
- **Kaufseite** im Hoch-Moment: Hinweis in der Auswertung nach dem ersten Kraken bzw. am Ende der Gratis-Strecke, dazu „🌙 Vollversion" im Menü und bei den Premium-Artikeln im Shop. Im Prototyp ist der Kauf ein klar markierter **Test-Kauf** (es wird nichts abgebucht); „Käufe wiederherstellen" und echte Zahlung kommen mit der App-Store-Version. Zum Testen lässt sich die Vollversion auf der Kaufseite zurücksetzen.
- **📤 Rekord teilen**: Nach jedem Run erzeugt das Spiel ein Rekord-Bild (Distanz, Combo, Perlen, „Schaffst du das?" + Link) und öffnet auf dem Handy das Teilen-Menü (WhatsApp & Co.); am Desktop wird es heruntergeladen.

## Fair & lernbar: Können statt Glück
Gemessen auf iPhone-Breite: vorher war ein Hindernis bei Vollgas nur 0,2–0,4 s sichtbar (unter der
Reaktionszeit), und 43 % aller Hindernis-Paare lagen zu weit für einen Sprung, aber zu nah zum Landen und
neu Abspringen. Ein reagierender Spieler kam dadurch nicht weiter als einer, der nie springt. Jetzt:
- **⚠-Vorwarnung** am rechten Rand ~1,2 s vor jedem Hindernis (🦈 rot für Haie), mit Countdown-Ring — unabhängig von Bildschirmbreite und Tempo
- **Faire Abstände**: Hindernisse kommen entweder als Gruppe, die ein Sprung nimmt, oder mit genug Zeit zum Landen (Haie mit extra Abstand, nie in Gruppen); die ersten ~3 s sind frei
- **Run-Analyse** nach jedem Lauf: Todesursache in Klartext, dein Wert vs. Rekord pro Disziplin (🏆 bei neuem Bestwert), Trend der letzten 10 Runs (▲ +X %) und ein gezielter Tipp
- **Rekord-Boje** 🏁: deine Bestweite steht als Fahne im Wasser
Ergebnis (Bot mit 0,3 s Reaktionszeit, 14 Läufe): Median 6.256 m statt 3.479 m — Können zahlt sich jetzt aus.

## Steuerung (One-Button, mobile-first)
- **HALTEN** = die Wellenflanke *anpumpen* → Speed aufbauen; am Kamm abheben (loslassen = Absprung-Pop für höhere Airs)
- **In der Luft HALTEN** = **Flip/Rotation** (Trickpunkte) → rechtzeitig loslassen, um sauber & gerade zu landen
- **In der Luft kurz TIPPEN** = **Grab** (Style-Punkte ohne Rotationsrisiko)
- **Sauber landen** = Combo läuft weiter + kleiner Speed-Boost. Schief landen = **Wipeout** (Combo weg, Speed bricht ein)
- Desktop-Test: `Leertaste` / `Pfeil-runter` = Halten, `P` = Pause, `M` = Ton

## Der Clou: die Monsterwelle 🌊
Statt „einmal berührt = tot" jagt dich eine **riesige Monsterwelle** von hinten. Ihr Abstand funktioniert
wie ein Lebensbalken (🌊-Anzeige oben links): sauber surfen schiebt sie zurück — je schneller, desto mehr —,
jeder **Wipeout** lässt sie um einen festen Betrag heranrollen. **1 Fehler = spürbar, 2 kurz nacheinander =
Gefahr, 3 in Folge = gefressen.** Immer gleich, unabhängig von Glück mit der Wellenform. Auf schmalen
Handys kündigt Gischt am linken Rand sie an, bevor sie ins Bild rollt.

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
- **Lebendiges Meer** 🐬: ein Event-Director streut alle 10–15 s eine Überraschung ein (erste nach ~5 s):
  🐬 **Delfin** schwimmt mit und legt bei jedem Sprung eine Perlenspur auf deinen Weg · 🐋 **Wal-Sprung** bricht vor dir durch die Oberfläche (+15 Perlen) · 💰 **Schatzspur**: hindernisfreie Münzspur bis zu einer Truhe (40–70 Perlen) · 🌠 **Sternschnuppen** (nachts): Sternsplitter in Sprunghöhe fangen · 🌈 **Sonnenregen → Regenbogen**: solange er steht, zählen Perlen doppelt. Dazu 4 neue Missionen.
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
