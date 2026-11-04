# Spiel-Links zu Platzer/kapitel2.tex

- Spieleliste exakt aus `Platzer/kapitel2.tex` Zeilen 25–27 (9 Titel, Schreibweisen inkl. Tippfehler übernommen: `Baldur's Gate lll`, `Age of Empires ll`).
- Prüfmethode: `curl -L` (HTTP-Status nach Redirects, finale URL, HTML-`<title>`), `https://store.steampowered.com/api/appdetails?appids=<ID>` (JSON: developers, publishers, release_date, website), Wikipedia-API nur als Sekundärquelle. Kein `web_search` benutzt.
- Zugriffsdatum überall: 2026-11-04.
- `literatur.bib` (427 Zeilen) gegengeprüft: **kein Eintrag zu einem der 9 Spiele vorhanden** (kein Duplikat, kein passender Key). Einziges Spiel-Vorbild im Bestand: `@software{LegendOfZelda98}`.
- `kapitel2.tex` enthält **keine** `\cite`-Befehle zu den Spielen (nur `\emph{}` in Zeilen 25–27).
- Statusformat: `HTTP-Code · finaler Redirect · Seitentitel`.

## 1. Diablo

- **Titel in Datei:** `\emph{Diablo}` (kapitel2.tex:25) – mehrdeutig: Reihe vs. Diablo (1996/97) vs. Diablo II (2000) vs. Diablo IV (2023).
- **Offizieller Titel (empfohlen):** Diablo (1996/97)
- **Entwickler:** Blizzard North (Wikipedia, sekundär)
- **Publisher:** Blizzard Entertainment (Wikipedia, sekundär)
- **Release-Jahr:** 1997 (NA 1997-01-03; GOG: "released in 1997") – **UNSICHER:** Wikipedia-Sammelartikel "Isometric video game graphics" nennt 1996.
- **Offizielle URL:** `https://diablo.blizzard.com/` · HTTP 200 · Redirect → `https://diablo4.blizzard.com/en-us/` · Titel "Diablo IV" → führt **nicht** zu Diablo (1996/97). Offizielle Produktseite für Diablo (1996/97): **nicht verifizierbar** – Spieleübersicht verlinkt nur `https://shop.battle.net/product/diablo` (HTTP 401) → UNSICHER.
- **Offizielle Spieleübersicht:** `https://www.blizzard.com/en-us/games/` · HTTP 200 · Titel "Blizzard Entertainment - All Games" · verlinkt `https://shop.battle.net/product/diablo` · HTTP 401 (Login-Wall, kein 404).
- **Store-URL:** `https://www.gog.com/en/game/diablo` · HTTP 200 · final identisch · Titel "Diablo + Hellfire | GOG.com".
- **Steam:** kein Eintrag (Steam-Suche "Diablo" liefert nur Diablo IV App 2344520, Diablo II: Resurrected App 2536520, Diablo IV DLC).
- **Quellentyp:** primär = GOG-Store-Seite (Brand Blizzard Entertainment); sekundär = Wikipedia (Entwickler, Publisher, Release, Perspektive).
- **isometrisch:** ja
  - Beleg 1: Wikipedia "Diablo (video game)" – "3D isometric style" (Entwicklung).
  - Beleg 2: Wikipedia "Isometric video game graphics" – Diablo in Liste "fixed isometric perspective".
  - Beleg 3: Wikipedia-Kategorie "Video games with isometric graphics".
- **UNSICHER / fehlt:** offizielle Blizzard-Produktseite für Diablo (1996/97); Widerspruch Release 1996 vs. 1997.
- **BibTeX:**
```bibtex
@software{Diablo97,
   author={{Blizzard North}},
   title={{Diablo}},
   publisher={{Blizzard Entertainment}},
   year={1997},
   url={https://www.gog.com/en/game/diablo},
   urldate={2026-11-04},
   note={Store-Seite GOG; offizielle Blizzard-Produktseite für Diablo (1996/97) nicht mehr verfügbar},
   hyphenation={english}
}
```
- **Alternative – Diablo II (2000):** Blizzard North / Blizzard Entertainment · NA 2000-06-28 (Wikipedia) · offizielle Remaster-Seite `https://diablo2.blizzard.com/` HTTP 200 · Redirect → `/en-us/` · Titel "Diablo II: Resurrected" · Store: Battle.net (HTTP 401) und Steam App 2536520 (HTTP 200, "Diablo II: Resurrected – Infernal Edition", Steam-Release 2026-02-11) · isometrisch: ja (Wikipedia "Isometric video game graphics": "fixed-perspective 2D perspective like its predecessor").
```bibtex
@software{DiabloII00,
   author={{Blizzard North}},
   title={{Diablo II}},
   publisher={{Blizzard Entertainment}},
   year={2000},
   url={https://diablo2.blizzard.com/},
   urldate={2026-11-04},
   note={offizielle Remaster-Seite Diablo II: Resurrected; Steam App 2536520},
   hyphenation={english}
}
```
- **Alternative – Diablo IV (2023):** Blizzard Entertainment (Dev+Pub, Steam-Appdetails) · 2023-06-05 (Wikipedia; Steam-Release 2023-10-17) · offiziell `https://diablo4.blizzard.com/` HTTP 200 · Titel "Diablo IV" · Store Steam App 2344520 HTTP 200 "Diablo® IV on Steam" · isometrisch: ja – Wikipedia: "overhead isometric view"; Steam-Community-Tag "Isometric".
```bibtex
@software{DiabloIV23,
   author={{Blizzard Entertainment}},
   title={{Diablo IV}},
   publisher={{Blizzard Entertainment}},
   year={2023},
   url={https://diablo4.blizzard.com/},
   urldate={2026-11-04},
   note={Steam-Release 2023-10-17; Steam App 2344520},
   hyphenation={english}
}
```
- **Empfehlung:** Diablo (1996/97) zitieren (klassischer isometrischer 2D-Vertreter); Diablo IV nur als modernes Beispiel, Diablo II als Zwischenschritt.

## 2. Baldur's Gate lll

- **Titel in Datei:** `\emph{Baldur's Gate lll}` (kapitel2.tex:25) – Tippfehler: drei kleine "l" statt römischer Ziffer III; offizieller Titel: **Baldur's Gate 3**.
- **Entwickler:** Larian Studios (Steam-Appdetails 1086940; Wikipedia)
- **Publisher:** Larian Studios (Steam-Appdetails 1086940; Wikipedia)
- **Release-Jahr:** 2023 (Windows 2023-08-03; Steam-Appdetails + Wikipedia)
- **Offizielle URL:** `https://baldursgate3.game/` · HTTP 200 · final identisch · Titel "Baldur's Gate 3".
- **Store-URL:** `https://store.steampowered.com/app/1086940/` · HTTP 200 · final identisch · Titel "Baldur's Gate 3 on Steam".
- **Quellentyp:** primär = Larian-Website + Steam-Store/Appdetails; sekundär = Wikipedia.
- **isometrisch:** isometrie-ähnlich / **UNSICHER**
  - Wikipedia: "free-floating camera, with players able to adjust the perspective from top-down isometric to third person".
  - Kein Isometric-Tag auf der Steam-Store-Seite; kein streng isometrisches Projektionsverfahren belegt.
- **UNSICHER / fehlt:** offizielle Entwickler-/Publisher-Aussage zur Projektionsart; keine strikte Isometrie nachgewiesen.
- **BibTeX:**
```bibtex
@software{BaldursGateIII23,
   author={{Larian Studios}},
   title={{Baldur's Gate 3}},
   publisher={{Larian Studios}},
   year={2023},
   url={https://baldursgate3.game/},
   urldate={2026-11-04},
   note={Steam App 1086940; Windows-Release 2023-08-03},
   hyphenation={english}
}
```

## 3. Disco Elysium

- **Titel in Datei:** `\emph{Disco Elysium}` (kapitel2.tex:25)
- **Entwickler:** ZA/UM (Steam-Appdetails 632470; Wikipedia)
- **Publisher:** ZA/UM (Steam-Appdetails 632470; Wikipedia)
- **Release-Jahr:** 2019 (Windows 2019-10-15; Steam-Appdetails + Wikipedia)
- **Offizielle URL:** `https://discoelysium.com/` · HTTP 200 · final identisch · Titel "Disco Elysium".
- **Offizielle Studio-URL (Zusatz):** `https://zaumstudio.com/` · HTTP 200 · final identisch · Titel "ZA/UM".
- **Store-URL:** `https://store.steampowered.com/app/632470/` · HTTP 200 · final identisch · Titel "Disco Elysium - The Final Cut on Steam".
- **Quellentyp:** primär = Publisher-Seite + Steam; sekundär = Wikipedia.
- **isometrisch:** ja
  - Wikipedia: "The game is presented in an isometric perspective in which the player character is controlled."
  - Steam-Community-Tag "Isometric" (kein offizieller Beleg).
- **UNSICHER / fehlt:** — (Beleg ausreichend über Wikipedia + Store-Tag).
- **BibTeX:**
```bibtex
@software{DiscoElysium19,
   author={{ZA/UM}},
   title={{Disco Elysium}},
   publisher={{ZA/UM}},
   year={2019},
   url={https://discoelysium.com/},
   urldate={2026-11-04},
   note={Steam App 632470 (Disco Elysium - The Final Cut); Release 2019-10-15},
   hyphenation={english}
}
```

## 4. Age of Empires ll

- **Titel in Datei:** `\emph{Age of Empires ll}` (kapitel2.tex:26) – Tippfehler: zwei kleine "l" statt römischer Ziffer II; mehrdeutig: Original (1999) vs. Definitive Edition (2019).
- **Offizieller Titel (empfohlen):** Age of Empires II: Definitive Edition (2019)
- **Entwickler:** World's Edge, Forgotten Empires u. a. (Steam-Appdetails 813780); Original 1999: Ensemble Studios (Wikipedia)
- **Publisher:** Xbox Game Studios (Steam-Appdetails 813780); Original 1999: Microsoft (Wikipedia)
- **Release-Jahr:** 2019 (Definitive Edition, 2019-11-14; Steam-Appdetails + Wikipedia) / 1999 (Original, 1999-09-27; Wikipedia)
- **Offizielle URL:** `https://www.ageofempires.com/games/aoeiide/` · HTTP 200 · final identisch · Titel "Age of Empires II: Definitive Edition - Play with Game Pass for PC - Age of Empires - World's Edge Studio".
- **Store-URL:** `https://store.steampowered.com/app/813780/` · HTTP 200 · final identisch · Titel "Age of Empires II: Definitive Edition on Steam".
- **Quellentyp:** primär = Xbox-Game-Studios-Website + Steam-Store/Appdetails; sekundär = Wikipedia.
- **isometrisch:** ja
  - Wikipedia "Age of Empires II: Definitive Edition": "The game is presented in an isometric format."
  - Wikipedia-Kategorie "Video games with isometric graphics"; Steam-Community-Tag "Isometric".
- **UNSICHER / fehlt:** —
- **BibTeX:**
```bibtex
@software{AgeOfEmpiresIIDE19,
   author={{World's Edge} and {Forgotten Empires}},
   title={{Age of Empires II: Definitive Edition}},
   publisher={{Xbox Game Studios}},
   year={2019},
   url={https://www.ageofempires.com/games/aoeiide/},
   urldate={2026-11-04},
   note={Steam App 813780; Original Age of Empires II 1999 (Ensemble Studios/Microsoft)},
   hyphenation={english}
}
```
- **Empfehlung:** Definitive Edition zitieren (offizielle Seite + Store belegbar); Original 1999 nur über Wikipedia belegbar.

## 5. Warcraft

- **Titel in Datei:** `\emph{Warcraft}` (kapitel2.tex:26) – mehrdeutig: Reihe vs. Warcraft: Orcs & Humans (1994) vs. Warcraft II (1995) vs. Warcraft III (2002/Reforged).
- **Offizieller Titel (empfohlen):** Warcraft: Orcs & Humans (1994) – nur mit Beleg-Einschränkung (siehe isometrisch)
- **Entwickler:** Blizzard Entertainment (Wikipedia)
- **Publisher:** Blizzard Entertainment (NA; EU 1995 Interplay, Wikipedia)
- **Release-Jahr:** 1994 (NA 1994-11-15; Wikipedia)
- **Offizielle URL:** `https://warcraft.blizzard.com/` · **HTTP 000 · DNS nicht auflösbar** (`getent hosts`: kein Ergebnis) → **UNSICHER/tot**. `https://warcraft.com/` und `https://www.warcraft.com/` · HTTP 200 · Redirect → `https://worldofwarcraft.blizzard.com/en-us/` · Titel "World of Warcraft" (falsche Marke).
- **Offizielle Produktseite:** `https://shop.battle.net/product/warcraft-orcs-and-humans` · HTTP 401 (Login-Wall; verlinkt von `https://www.blizzard.com/en-us/games/` HTTP 200 "Blizzard Entertainment - All Games").
- **Weitere offizielle Produktlinks (von Blizzard-Spieleübersicht):** `https://shop.battle.net/product/warcraft-1-remastered` · HTTP 401; `https://shop.battle.net/product/warcraft-2-remastered` · HTTP 401; `https://shop.battle.net/product/warcraft-2-battle-net-edition` · HTTP 401.
- **Store-URL:** Battle.net (HTTP 401, Login-Wall) → **UNSICHER**; kein Steam-/GOG-Eintrag gefunden (Steam-Suche "Warcraft": keine offiziellen Treffer; GOG-Katalogsuche "warcraft": kein Blizzard-Titel).
- **Warcraft III: Reforged (Alternative):** `https://warcraft3.blizzard.com/` · HTTP 200 · Redirect → `/en-us/` · Titel "Warcraft III: Reforged"; Store `https://shop.battle.net/product/warcraft-iii-reforged` · HTTP 302 → Login (kein 404); Wikipedia: NA 2002-07-03.
- **Quellentyp:** primär = Blizzard-Produktseiten (nur Login-Wall); sekundär = Wikipedia (Entwickler, Publisher, Release, Perspektive).
- **isometrisch:** **UNSICHER**
  - Warcraft III: Wikipedia – "classical top-down perspective with a slight angle that can only be zoomed and rotated slightly" → nicht streng isometrisch, nur isometrie-ähnlich.
  - Warcraft: Orcs & Humans / Warcraft II: keine explizite Perspektiv-Angabe in Wikipedia-Text, offizieller Store-Beschreibung oder Steam/GOG gefunden → Beleg fehlt.
- **UNSICHER / fehlt:** DNS-Ausfall `warcraft.blizzard.com`; Battle.net-Shop nur mit Login; kein Beleg für "isometrisch" bei Warcraft I/II.
- **BibTeX (Warcraft: Orcs & Humans):**
```bibtex
@software{Warcraft94,
   author={{Blizzard Entertainment}},
   title={{Warcraft: Orcs \& Humans}},
   publisher={{Blizzard Entertainment}},
   year={1994},
   url={https://shop.battle.net/product/warcraft-orcs-and-humans},
   urldate={2026-11-04},
   note={Battle.net-Produktseite nur mit Login erreichbar (HTTP 401); kein Steam-/GOG-Eintrag gefunden},
   hyphenation={english}
}
```
- **BibTeX (Alternative Warcraft III: Reign of Chaos, belegbar):**
```bibtex
@software{WarcraftIII02,
   author={{Blizzard Entertainment}},
   title={{Warcraft III: Reign of Chaos}},
   publisher={{Blizzard Entertainment}},
   year={2002},
   url={https://warcraft3.blizzard.com/},
   urldate={2026-11-04},
   note={offizielle Seite Warcraft III: Reforged; Store Battle.net (Login); Perspektive nur top-down mit leichtem Winkel},
   hyphenation={english}
}
```
- **Empfehlung:** für strikt isometrische Argumentation Warcraft: Orcs & Humans (1994) oder Warcraft II (1995) – Beleg nachziehen (Handbuch/Review), sonst UNSICHER; Warcraft III nur als isometrie-ähnlich zitieren.

## 6. Gears Tactics

- **Titel in Datei:** `\emph{Gears Tactics}` (kapitel2.tex:26)
- **Entwickler:** Splash Damage, The Coalition (Steam-Appdetails 1184050; Wikipedia)
- **Publisher:** Xbox Game Studios (Steam-Appdetails 1184050; Wikipedia)
- **Release-Jahr:** 2020 (Windows 2020-04-28; Steam-Appdetails + Wikipedia)
- **Offizielle URL:** `https://www.gearstactics.com/` · HTTP 200 · Redirect → `https://www.gearsofwar.com/en-us/games/gears-tactics/` · Titel "Gears of War | Gears Tactics".
- **Store-URL:** `https://store.steampowered.com/app/1184050/` · HTTP 200 · final identisch · Titel "Gears Tactics on Steam".
- **Quellentyp:** primär = Xbox-/Gears-of-War-Website + Steam-Store/Appdetails; sekundär = Wikipedia.
- **isometrisch:** isometrie-ähnlich / **UNSICHER**
  - Wikipedia: "The game is played from a top-down perspective" (kein "isometrisch").
  - Steam-Community-Tag "Isometric" (kein offizieller Beleg); Unreal Engine 4, 3D (Wikipedia).
  - Kein offizielles Statement "isometrisch" auf Store-Seite/Entwicklerseite gefunden.
- **UNSICHER / fehlt:** offizieller Beleg für isometrische Projektion.
- **BibTeX:**
```bibtex
@software{GearsTactics20,
   author={{Splash Damage} and {The Coalition}},
   title={{Gears Tactics}},
   publisher={{Xbox Game Studios}},
   year={2020},
   url={https://www.gearsofwar.com/en-us/games/gears-tactics/},
   urldate={2026-11-04},
   note={Steam App 1184050; gearstactics.com leitet auf gearsofwar.com weiter},
   hyphenation={english}
}
```

## 7. Die Siedler

- **Titel in Datei:** `\emph{Die Siedler}` (kapitel2.tex:27) – mehrdeutig: Reihe, Die Siedler (1993) oder Die Siedler: Neue Allianzen (2023).
- **Offizieller Titel (empfohlen):** Die Siedler (1993) – für isometrische Argumentation; Quelle dünn (nur sekundär).
- **Entwickler:** Blue Byte (Wikipedia)
- **Publisher:** Blue Byte (MS-DOS NA: Strategic Simulations/SSI, Wikipedia)
- **Release-Jahr:** 1993 (Amiga DE 1993-06-30; Wikipedia)
- **Offizielle URL:** **nicht auffindbar** → `https://www.ubisoft.com/en-us/game/the-settlers` · HTTP 404 · Redirect → `https://www.ubisoft.com/en-us/404` · Titel "Not Found"; `https://www.ubisoft.com/de-de/games/the-settlers` · HTTP 404 · Titel "Nicht gefunden".
- **Store-URL:** **keine** – kein GOG-/Steam-Eintrag für Die Siedler (1993); GOG-Katalogsuche "settlers" liefert nur Settlers 2/3/4, Rise of an Empire, Settlers Bundle (Inhalt: Settlers 2 Gold, Settlers 2 10th Anniversary, Settlers 3, Settlers 4, Rise of an Empire – **ohne** 1993er-Teil).
- **Quellentyp:** ausschließlich sekundär = Wikipedia (kein Primärbeleg verfügbar).
- **isometrisch:** ja (Beleg dünn)
  - Wikipedia-Kategorie "Video games with isometric graphics".
  - Kein In-Text-Beleg in Wikipedia (en/de) und keine offizielle Quelle gefunden.
- **UNSICHER / fehlt:** offizielle Produkt-/Store-Seite; In-Text-Beleg für isometrische Perspektive.
- **Alternative – Die Siedler: Neue Allianzen (2023):** Ubisoft Düsseldorf / Ubisoft (Steam-Appdetails 2750080) · 2023-02-17 (Wikipedia; Steam-Release 2024-03-26) · offiziell `https://www.ubisoft.com/en-us/games/the-settlers-new-allies` · HTTP 200 · Redirect → `https://www.ubisoft.com/de-de/games/the-settlers-new-allies` · Titel "Die Siedler: Neue Allianzen für PC und mehr" · Store Steam App 2750080 HTTP 200 "The Settlers: New Allies on Steam" · isometrisch: **nein/UNSICHER** (kein Isometric-Tag, 3D).
- **BibTeX (Die Siedler 1993):**
```bibtex
@software{DieSiedler93,
   author={{Blue Byte}},
   title={{Die Siedler}},
   publisher={{Blue Byte}},
   year={1993},
   url={https://en.wikipedia.org/wiki/The_Settlers_(1993_video_game)},
   urldate={2026-11-04},
   note={keine offizielle Produkt-/Store-Seite auffindbar; Beleg nur sekundär (Wikipedia)},
   hyphenation={german}
}
```
- **BibTeX (Alternative Neue Allianzen):**
```bibtex
@software{SiedlerNeueAllianzen23,
   author={{Ubisoft Düsseldorf}},
   title={{Die Siedler: Neue Allianzen}},
   publisher={{Ubisoft}},
   year={2023},
   url={https://www.ubisoft.com/en-us/games/the-settlers-new-allies},
   urldate={2026-11-04},
   note={Steam App 2750080; Steam-Release 2024-03-26; offizielle Seite leitet auf de-de um},
   hyphenation={german}
}
```
- **Empfehlung:** Die Siedler (1993) für die isometrische Argumentation, aber Beleg nachziehen (Handbuch/Screenshot-Quelle); Neue Allianzen passt nicht (3D, nicht isometrisch).

## 8. RimWorld

- **Titel in Datei:** `\emph{RimWorld}` (kapitel2.tex:27)
- **Entwickler:** Ludeon Studios (Steam-Appdetails 294100; Wikipedia)
- **Publisher:** Ludeon Studios (Steam-Appdetails 294100; Wikipedia)
- **Release-Jahr:** 2018 (1.0 am 2018-10-17; Steam-Appdetails + Wikipedia; Early Access ab November 2013)
- **Offizielle URL:** `https://rimworldgame.com/` · HTTP 200 · final identisch · Titel "RimWorld - Sci-Fi Colony Sim".
- **Offizielle Studio-URL (Zusatz):** `https://ludeon.com/` · HTTP 200 · Redirect → `https://ludeon.com/blog/` · Titel "Ludeon Studios".
- **Store-URL:** `https://store.steampowered.com/app/294100/` · HTTP 200 · final identisch · Titel "RimWorld on Steam".
- **Quellentyp:** primär = Ludeon-Website + Steam-Store/Appdetails; sekundär = Wikipedia.
- **isometrisch:** **nein**
  - Wikipedia: "The game is two-dimensional, viewed from a top down perspective."
  - Kein Isometric-Tag auf der Steam-Store-Seite.
  - → **Widerspruch zu kapitel2.tex:27** (RimWorld dort als isometrisches Beispiel gelistet).
- **UNSICHER / fehlt:** — (Befund eindeutig: top-down, nicht isometrisch).
- **BibTeX:**
```bibtex
@software{RimWorld18,
   author={{Ludeon Studios}},
   title={{RimWorld}},
   publisher={{Ludeon Studios}},
   year={2018},
   url={https://rimworldgame.com/},
   urldate={2026-11-04},
   note={Steam App 294100; Early Access 2013, Release 2018-10-17; Perspektive top-down, nicht isometrisch},
   hyphenation={english}
}
```

## 9. SimCity 2000

- **Titel in Datei:** `\emph{SimCity 2000}` (kapitel2.tex:27)
- **Entwickler:** Maxis (Wikipedia; EA-Produktseite: `"developer":"Maxis"`)
- **Publisher:** Maxis (Original); Electronic Arts (EA-Produktseite: `"publisher":"Electronic Arts"`)
- **Release-Jahr:** 1994 (MS-DOS 1994-02; Wikipedia) – Macintosh 1993-12; **UNSICHER:** EA-Store nennt "Release Date Feb 8, 1995".
- **Offizielle URL:** `https://www.ea.com/games/simcity/simcity-2000` · HTTP 200 · final identisch · Titel "Buy SimCity 2000™ - Electronic Arts".
- **Offizielle Serien-URL (Zusatz):** `https://www.ea.com/games/simcity` · HTTP 200 · final identisch · Titel "SimCity™ Video Games - Official EA Site".
- **Store-URL:** `https://www.gog.com/en/game/simcity_2000_special_edition` · HTTP 200 · final identisch · Titel "SimCity™ 2000 Special Edition 60% off | GOG.COM".
- **Steam:** kein Eintrag (Steam-Suche "SimCity" liefert nur SimCity 4 Deluxe, SimCity 3000 Unlimited).
- **Quellentyp:** primär = EA-Produktseite + GOG-Store; sekundär = Wikipedia.
- **isometrisch:** ja
  - Wikipedia: "SimCity 2000 is played from an isometric perspective as opposed to the previous title, which was played from a top-down perspective."
  - Wikipedia: "near-isometric dimetric view".
  - Wikipedia "Isometric video game graphics": SimCity 2000 (1994) in Liste "fixed isometric perspective".
- **UNSICHER / fehlt:** Release-Datum (1993 Mac / 1994 DOS / 1995 EA-Store).
- **BibTeX:**
```bibtex
@software{SimCity2000_94,
   author={{Maxis}},
   title={{SimCity 2000}},
   publisher={{Maxis}},
   year={1994},
   url={https://www.ea.com/games/simcity/simcity-2000},
   urldate={2026-11-04},
   note={Macintosh 1993-12, MS-DOS 1994-02; EA-Store nennt Release Date 1995-02-08; GOG: SimCity 2000 Special Edition},
   hyphenation={english}
}
```

## Mehrdeutigkeiten und Lücken

- **Reihentitel (Diablo / Warcraft / Die Siedler):** Datei nennt nur die Reihe, konkreter Teil muss gewählt werden. Empfehlung: Diablo (1996/97) bzw. Diablo II (2000) für isometrisch; Warcraft: Orcs & Humans (1994) bzw. Warcraft II (NA 1995-12-05, Wikipedia) für isometrisch, Warcraft III (2002) nur isometrie-ähnlich; Die Siedler (1993) für isometrisch, Neue Allianzen (2023) nicht (3D). Belege: Diablo, Diablo II, Disco Elysium, AoE II, SimCity 2000 belegt; Warcraft I/II und Die Siedler (1993) nur über Wikipedia-Kategorie, Beleg nachziehen.
- **RimWorld ist kein isometrisches Spiel** (Wikipedia: "two-dimensional, viewed from a top down perspective") – Widerspruch zu kapitel2.tex:27, dort als isometrisches Beispiel gelistet; Titel ersetzen oder Aussage abschwächen (Hinweis, keine .tex-Änderung ausgeführt).
- **Nur isometrie-ähnlich:** Baldur's Gate 3 (freie Kamera: top-down isometrisch bis third person) und Gears Tactics (Wikipedia "top-down perspective", 3D) → als "isometrisch" nur mit Einschränkung haltbar (UNSICHER).
- **Formfehler und fehlende Primärbelege:** kapitel2.tex:25–27 Tippfehler `Baldur's Gate lll` (drei kleine L) und `Age of Empires ll` (zwei kleine L); keine `\cite`-Befehle und literatur.bib ohne diese 9 Titel → alle BibTeX-Vorschläge sind neu; offizielle Produktseiten fehlen für Diablo (1996/97) und Die Siedler (1993), `warcraft.blizzard.com` ist DNS-tot, Battle.net-Shop nur mit Login (HTTP 401).
