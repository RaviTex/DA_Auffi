# Recherche: Definition „isometrische Ansicht in Videospielen“ (Kap. 9.1)

## 0. Kontext, Bestand, Prüfprotokoll

- Repo: `/home/shmaster/Documents/DA_Auffi`
- Kapitel 9: `Platzer/kapitel2.tex`, Z. 1 `\chapter{Isometrische Videospiele}`; TOC: `chapter.9`
- Abschnitt 9.1: `Platzer/kapitel2.tex`, Z. 11; Quelltext-Titel mit doppeltem Leerzeichen: `Definition einer  isometrischen Ansicht in Videospielen` (TOC zeigt einfaches Leerzeichen)
- Zu prüfende Behauptungen: (1) Kamera schräg von oben, „meist 30 bis 45 Grad“; (2) kein Fluchtpunkt, keine Verkleinerung/kein anderer Winkel; (3) Ziel gute Übersicht; (4) „isometrisch“ als Genre-Beisatz (Action-RPG, Strategie, Aufbausimulation)
- Prüfdatum: 2026-11-04
- Methoden: Crossref-API (`api.crossref.org/works/<DOI>`, DOI-Lookups + `query.bibliographic`), Google Books `SearchWithinVolume` (Snippets mit Seitenzahl), archive.org-Volltextscans (OCR, Seiten über Running Heads/Scandata zugeordnet), OpenAlex-API (Abstract-Rekonstruktion, Volltextsuche), Open-Library-Fulltextsuche, DiGRA-PDF (eigener Download + `pdftotext`), direkte HTTP-Abrufe
- Nicht benutzt: web_search (defekt); DuckDuckGo/Google-Web (blockiert/Challenge); Semantic Scholar (HTTP 429)
- Wikipedia-Sicherung `_recherche/wiki_iso.json` (Seite `Isometric video game graphics`): nur Fundstelle für Literatur, NICHT zitierwürdig; Kernaussage dort selbst mit `{{or}}` (Original Research) markiert: „isometric computer graphics are rarely truly isometric … dimetric projection or a 2:1 pixel ratio being the most common“; 29 `<ref>`-Einträge, u. a. Krikke 2000, Perron/Wolf 2008 S. 158, Collins (SIGGRAPH), usgamer, Kotaku
- `literatur.bib`: reine Vorlagen-Bib (Lamport, Kopka, Oetiker, Burger, …); keine Grafik-/Projektions-/Game-Design-Quelle; für alle Kandidaten unten: **nicht vorhanden**; kein Duplikat gefunden
- Zitierbefehle in `Platzer/`: nur `einleitung.tex:19` `\cite{Lamport94,Lamport95}`; `kapitel2.tex`–`kapitel4.tex` ohne `\cite`
- Weitere Bib-Dateien: `abgabe.bib` (nur Katze/Formel1, gehört `Latex_Abgabe.tex`), `DA_Auffi.bib` (leer) — für `literatur.bib` nicht relevant

---

## 1. Kandidaten

### [1] ISO 5456-3:1996 — Technische Zeichnungen — Projektionsmethoden — Teil 3: Axonometrische Darstellungen
- Autor/Herausgeber: ISO/TC 10 (UNSICHER: Komitee nicht selbst gesehen); deutsche Übernahme: DIN
- Jahr: ISO 1996; DIN-Ausgabe 1998-04
- Verlag: ISO; DIN Media GmbH (DE-Übernahme)
- DOI: `10.31030/7384269` (DIN ISO 5456-3:1998-04); URL: https://doi.org/10.31030/7384269
- ISBN: keine (Norm)
- Verifikation: Crossref-Record selbst abgefragt (Titel: „DIN ISO 5456-3:1998-04, Technische Zeichnungen_- Projektionsmethoden_- Teil_3: Axonometrische Darstellungen (ISO_5456-3:1996)“, Typ `standard`, Verlag DIN Media GmbH); ISO-Katalogseite `iso.org/standard/…` → HTTP 403 (Cloudflare), auch `standard/26094/26095/26096.html` getestet → 403; Volltext nicht geprüft
- Relevanz:
  - normativ für „axonometrische Darstellung“ = Oberbegriff, isometrisch/dimetrisch/trimmetrisch als Unterfälle
  - kein Videospielbezug; nur Geometrie-/Normbeleg für 9.1
  - Paywall → keine wörtliche Fundstelle behaupten
- Zitierwürdigkeit: Norm (nicht peer-reviewed) · primär (normativ) · kein Praxisbeleg
- Fundort im Kapitel: 9.1, Geometrie-Basis (ergänzend zu [4]/[3]); nicht für Games-Claims
- Volltext-Zugang: nein (Paywall/kein Zugriff); genaue Seiten: nicht prüfbar
- Status in `literatur.bib`: nicht vorhanden

### [2] Foley, James D.; van Dam, Andries; Feiner, Steven K.; Hughes, John F.: Computer Graphics: Principles and Practice (2. Aufl.)
- Jahr: 1990
- Verlag: Addison-Wesley
- ISBN: 0-201-12110-7 (Open Library: „Computer graphics“, 1990, Addison-Wesley, 1174 S.)
- DOI: keiner (Buch); URL: keine stabile Verlagsseite geprüft
- Verifikation: Volltext-Scan selbst gelesen (archive.org-Identifier `foley-james-d.-et-al.-computer-graphics-principles-and-practice-2nd-edition`, `_djvu.xml` + `_djvu.txt`); Seitenzahlen über die im OCR sichtbaren Running Heads („231“, „233“, „234“) verifiziert; ISBN über Open-Library-API
- Wörtliche Fundstellen (selbst gesehen):
  - S. 231, Abschnitt 6.1 „Projections“: „The size of the perspective projection of an object varies inversely with the distance of that object from the center of projection.“
  - S. 231: „The projection can be used for exact measurements and parallel lines do remain parallel.“
  - S. 233: „Axonometric orthographic projections use projection planes that are not normal to a principal axis and therefore show several faces of an object at once.“ / „the foreshortening is uniform rather than being related to the distance from the center of projection“
  - S. 234: „The isometric projection has the useful property that all three principal axes are equally foreshortened, allowing measurements along the axes to be made to the same scale (hence the name: iso for equal, metric for measure).“
  - S. 233/234: isometrische Projektion als Konstruktion entlang Richtung `(1,−1,−1)` (Fig. 6.7)
- Relevanz:
  - belegt „kein Fluchtpunkt“ / „keine Verkleinerung mit Entfernung“ = Parallelprojektion (S. 231)
  - belegt isometrisch = gleiche Verkürzung aller drei Hauptachsen (S. 234), Axonometrie = mehrere Flächen gleichzeitig (S. 233)
  - direkter Beleg für „Objekte nicht kleiner“; „nicht aus anderem Winkel sichtbar“ nur indirekt (fixe Projektionsrichtung), kein Satz dazu gefunden
- Zitierwürdigkeit: Lehrbuch, nicht peer-reviewed · sekundär · kein Praxisbeleg
- Fundort im Kapitel: 9.1, Punkt 1 (Geometrie) und Punkt 2 („Kein Fluchtpunkt“)
- Volltext-Zugang: ja (Scan der 2. Aufl. 1990); gedruckte Ausgabe käuflich
- Status in `literatur.bib`: nicht vorhanden
- Hinweis: 3. Aufl. (2013) nicht geprüft; 2. Aufl. inhaltlich verifiziert

### [3] Morling, Ken: Geometric and Engineering Drawing (3. Aufl.), Kap. 3 „Isometric Projection“, S. 31–42
- Autor: K. Morling (Crossref: „K. Morling“)
- Jahr: 2010
- Verlag: Elsevier (Routledge-Ausgabe separat: `10.4324/9780080967691-10`)
- Kapitel-DOI: `10.1016/B978-0-08-096768-4.00003-6`; Buch-ISBN: 9780080967684
- Verifikation: Crossref-DOI-Record (Titel, Autor, S. 31–42, ISBN); Volltext-Scan selbst gelesen (archive.org-Identifier `geometric.and.engineering.drawing`, Vollzugriff, `_djvu.xml`); Seitenzuordnung: Kapitelbeginn S. 31 = Leaf 47, S. 38 = Leaf 54 (Scandata/Printed-Page-Mapping)
- Wörtliche Fundstellen (selbst gesehen):
  - S. 31: „Isometric drawing ignores perspective altogether. Lines are drawn parallel to each other and drawings can be made using a T-square and a set square.“
  - S. 31: „three isometric axes. These are inclined at 120° to each other. One axis is vertical and the other two axes are therefore at 30° to the horizontal. Dimensions measured along these axes, or parallel to them, are true lengths.“
  - S. 31: „True isometric projection is an application of orthographic projection … The most common form of isometric projection is called ‚conventional isometric‘.“
  - S. 35: Abschnitt „True Isometric Projection“; S. 37: Fig. 3.8 „True length 30° 30°“
  - S. 38: „The ratio between the true length and the isometric length is isometric length = true length X 0.8165. This ratio is constant for all lines measured parallel to any of the isometric axes.“
- Relevanz:
  - belegt „kein Fluchtpunkt“ (S. 31) und 30°-Zeichenachsen (nicht Kameraneigung!)
  - belegt Unterscheidung „conventional isometric“ vs. „true isometric“ → Praxis vereinfacht „Isometrie“ (wichtig für Autor-These)
  - 0,8165 = cos 35,264° (eigene Rechnung, keine Quelle) → Brücke zum Winkel, aber im Text nicht als 35,264° ausgewiesen
- Zitierwürdigkeit: Lehrbuch, nicht peer-reviewed · sekundär · kein Praxisbeleg
- Fundort im Kapitel: 9.1, Punkt 1/2 (Geometrie, Winkel, Verkürzung)
- Volltext-Zugang: ja (archive.org-Vollzugriff); gedruckte Ausgabe käuflich
- Status in `literatur.bib`: nicht vorhanden

### [4] Salomon, David: Transformations and Projections in Computer Graphics, Kap. 2 „Parallel Projections“, S. 57–70
- Jahr: 2006
- Verlag: Springer London
- DOI: `10.1007/978-1-84628-620-9` (Buch); Kapitel: `10.1007/978-1-84628-620-9_3` („Parallel Projections“)
- ISBN: 978-1-84628-392-5 (print)
- Verifikation: Crossref-Buchrecord (Titel, Typ `book`, Verlag Springer London, 2006, ISBN); Google Books `SearchWithinVolume` (ID `6CzuydFlMpwC`) selbst abgefragt → Snippets mit Seitenzahlen; Seiten 62–66 mehrfach belegt
- Wörtliche Fundstellen (Snippets, selbst abgefragt; „…“ = Snippet-Lücke/OCR-Glättung):
  - S. 64: „isometric projection is the most useful but also the most restrictive of the three axonometric projections.“
  - S. 64: „we can measure distances on the diagram and divide them by 0.8165 to obtain actual dimensions“
  - S. 65: „after being rotated by ±45° about the y axis and by ±35.26° about the x axis. If these rotations result in obscuring important object features, a less restrictive projection, such as dimetric or trimetric, must be used.“
  - S. 65: „The standard specifies the ratio h/w = 1/√3, which results in α ≈ 30°. … a quantity that happens to be close to 35°. This projection is attributed by [Krikke 00] to William Farish, who developed it in 1822.“
  - S. 65/66: Fig. 2.8 „The 30° Standard for Isometric Projections“; Fig. 2.10 „The 27° Isometric Projection“
  - S. 66: „1:2 isometric projection because it is based on the ratio h/w = 1/2.“
  - S. 66: „A similar standard is based on the ratio h/w = 1, which leads to α = 45°. This case is also known as the military isometric projection.“
  - S. 66: weitere Standards: `h/w = 0.33` → „42°/7° standard“ (dimetric)
- Relevanz:
  - **Kernbeleg für „echte Isometrie“ vs. Spiele-Praxis**: echte Isometrie = ±45° Gier + ±35,26° Neigung, h/w = 1/√3, Zeichenachsen α ≈ 30° (S. 65)
  - 2:1-Spielstil = „1:2 isometric projection“, h/w = 1/2 → Zeichenachsen 27° (≈ arctan 0,5 = 26,565°, eigene Rechnung); Kameraneigung θ = arcsin(1/2) = 30° (eigene Rechnung auf Basis der Formel θ = arcsin(h/w), S. 65)
  - „military isometric“ h/w = 1 → 45° (S. 66) — belegt, dass 45° eine andere Konvention ist, nicht der isometrische Standard
  - zitiert Krikke 2000 → Brücke zu [5]
- Zitierwürdigkeit: Fachbuch (Springer), nicht peer-reviewed · sekundär · kein Praxisbeleg
- Fundort im Kapitel: 9.1, Punkt 1 (Winkel, 30° vs. 35,26°) und Differenzierung „echt vs. 2:1“
- Volltext-Zugang: kein Volltext (Paywall); Google-Books-Snippets mit Seitenzahlen; Seitenangaben aus Snippets, nicht aus Volltext
- Status in `literatur.bib`: nicht vorhanden
- **Korrektur zum Lead**: DOI `10.1007/978-1-84628-620-1` → HTTP 404 (Crossref geprüft); korrekt ist `10.1007/978-1-84628-620-9`

### [5] Krikke, Jan: „Axonometry: a matter of perspective“
- Jahr: 2000
- Venue: IEEE Computer Graphics and Applications, Jg. 20, Heft 4, S. 7–11
- DOI: `10.1109/38.851742`; URL: https://doi.org/10.1109/38.851742
- Verifikation: Crossref-Record (Titel, Autor „Krikke, J.“, IEEE, 20(4), S. 7–11); Abstract über OpenAlex-API (`abstract_inverted_index`) rekonstruiert; Volltext IEEE-Paywall, nicht gelesen
- Wörtliche Fundstellen (Abstract, rekonstruiert):
  - „Since the 1920s axonometry, or parallel perspective, has provided an important graphic technique for artists, architects, and engineers.“
  - „Axonometry, and the pictorial grammar that goes with it, has taken on a new significance with the advent of visual computing.“
  - „Most visual computing tools use a combination of axonometry and isometry with linear perspective to create anything from computer games to virtual reality worlds.“
- Relevanz:
  - belegt Axonometrie = Parallelperspektive (Abstract)
  - Bezug zu Computerspielen nur im Abstract-Satz, keine Definition/Gradangabe
  - von Salomon S. 65 als Quelle für Farish 1822 zitiert (Cross-Referenz)
- Zitierwürdigkeit: IEEE-Fachmagazin; **Peer-Review-Status UNSICHER** (Artikeltyp/Kolumne nicht verifiziert) · sekundär · kein Praxisbeleg
- Fundort im Kapitel: 9.1, Geometrie-Hintergrund; für „isometrisch“-Definition nur schwach
- Volltext-Zugang: nein (Paywall); Abstract: ja (OpenAlex)
- Status in `literatur.bib`: nicht vorhanden

### [6] Järvinen, Aki: „Gran Stylissimo: The Audiovisual Elements and Styles in Computer and Video Games“
- Jahr: 2002
- Venue: Computer Games and Digital Cultures Conference Proceedings (Hrsg. Frans Mäyrä), Tampere University Press, S. 113–128; ISSN 2342-9666
- DOI: `10.26503/dl.v2002i1.19`; URL: https://dl.digra.org/index.php/dl/article/view/19
- Verifikation: OJS-Metadaten (DC.Source = „Computer Games and Digital Cultures Conference Proceedings“, ISSN 2342-9666, Datum 2002); PDF selbst geladen und per `pdftotext` gelesen; Seitenzahlen aus PDF-Fußzeilen (113, 114, 117, 128)
- Wörtliche Fundstellen (selbst gesehen):
  - S. 114: „Then there are games where one sees characters, houses and other objects from above, from a tilted angle, but in such a way, that the horizon is not visible and the lines of perspective do not converge. This kind of view is called isometric. Well-known examples of games representing/simulating objects from isometric perspective include the popular Sim-games, many role-playing games (such as the Baldur’s Gate series) and the strategy game series Command & Conquer.“
  - S. 116, Abschnitt „Point of perception“: „if the game’s rules demand that the environment is made into a two-dimensional or isometric grid that governs the means of moving (like in many board games, or turn-based strategy games), then two dimensions or an isometric perspective might well be the appropriate solution regarding dimensionality.“
  - S. 117: „the isometric perspective employed by many ‚god games‘ is a means to lift the player above the ‚streets‘ to see the bigger picture, so to speak, and do omnipotent things.“
  - S. 117: „The Sims (Maxis Software, 1999) – isometric dimensionality with 3rd person PoP.“
- Relevanz:
  - **einzige gefundene akademische Spiele-Definition**: schräg von oben, kein Horizont, keine konvergierenden Linien (≈ „kein Fluchtpunkt“) (S. 114)
  - Genres: Sim-/Aufbauspiele, RPG (Baldur’s Gate), Strategie (Command & Conquer), God Games (S. 114/117) → stützt Genre-Beisatz (4)
  - Übersicht: „see the bigger picture“ (S. 117) → stützt Punkt 3
  - keine Gradzahl; keine Aussage zu „30–45°“; keine Aussage zu „nicht aus anderem Winkel“
- Zitierwürdigkeit: Konferenzbeitrag/Proceedings; **Peer-Review-Status UNSICHER** (DiGRA 2002, nicht belegt) · primär (Definition) · kein Praxisbeleg
- Fundort im Kapitel: 9.1 Punkte 1–3 + Genres; ggf. 9.2
- Volltext-Zugang: ja (Open-Access-PDF DiGRA Digital Library)
- Status in `literatur.bib`: nicht vorhanden

### [7] Pazera, Ernest: Isometric Game Programming with DirectX 7.0
- Jahr: 2001
- Verlag: Prima Tech / Prima Publishing (Rocklin, CA)
- ISBN: 0-7615-3089-4 (im Buchtext gelesen)
- DOI/URL: keiner/keine (Buch); archive.org-Identifier `isometric-game-programming-with-direct-x-7`
- Verifikation: Volltext-Scan selbst gelesen (`_djvu.xml`/`_djvu.txt`); Copyright-Seite (©2001 by Prima Publishing), ISBN im Text; Seitenzuordnung: Kap.-11-Titelblatt = Leaf 310 = S. 285 (TOC „Chapter 11 … 285“) → Leaf 312 = S. 287; Index bestätigt „isometric projection, 287“; Leaf 584 → S. 559 (Index „2:1 ratio, 561“ → UNSICHER ±2 S.)
- Wörtliche Fundstellen (selbst gesehen, OCR bereinigt):
  - S. 287, Kap. 11 „Introduction to IsoHex“: „An isometric projection is a 3D projection that does not correct for distance (in other words, something 30 tiles away is just as big as something 10 tiles away). The isometric projection is one of a family of axonometric projections. … Rhombuses, or diamond shapes, are usually used to represent an isometric tiled world.“ (OCR: „isomeric“, „ахопотвгіс“)
  - S. 559 (UNSICHER): „I’ve only really gotten tile slanting to work for isometric tiles that have an aspect ration of 2:1 (the width is 2 times the height).“ / „For a 64x32 isometric tile (which is my standard), you need a 16x16 square image.“
  - Kap. 9/10 (Seite UNSICHER): „Most real-time strategy games and turn-based strategy games are made using isometric tiles …“
- Relevanz:
  - Praxis-/Technikbeleg für „keine Entfernungsverkleinerung“ (S. 287) und 2:1-Tile-Standard (S. 559, UNSICHER)
  - Strategie-Genre als typischer Einsatz (Kap. 9/10, Seite UNSICHER)
  - keine Kamerawinkel-Gradangabe; keine akademische Definition
- Zitierwürdigkeit: Programmier-/Fachbuch, nicht peer-reviewed · sekundär (Praxis) · **Praxisbeleg ja**
- Fundort im Kapitel: 9.1 Punkt 2; Genres; 9.3 (Tile-/Bewegungslogik)
- Volltext-Zugang: ja (archive.org-Scan; Nutzung nur zur Verifikation)
- Status in `literatur.bib`: nicht vorhanden

### [8] Adams, Ernest: Fundamentals of Game Design
- Jahr: 2010 (Google-Books-Metadaten „New Riders, 2010“; Open Library ohne Datum)
- Verlag: New Riders (Pearson Education)
- ISBN: 978-0-13-210475-3 (ISBN-10: 013210475X; Open Library bestätigt Titel+Verlag)
- DOI: keiner; Google-Books-ID: `-BCrex2U1XMC`
- Verifikation: Google Books `SearchWithinVolume` selbst abgefragt (Snippets + Seitenzahlen); Buchseite: „New Riders, 2010“; Auflage nicht aus Metadaten gelesen → UNSICHER
- Wörtliche Fundstellen (Snippets, selbst abgefragt; „…“ = Snippet-Lücke):
  - S. 220: „ISOMETRIC PERSPECTIVE. The isometric perspective is normally used to display 2D outdoor scenes. While the top-down perspective looks straight down at the landscape from an elevated position, the isometric perspective looks across the …“
  - S. 220: „… 30 degrees from the horizontal. If the game world is rectilinear, as they usually are in games that use the isometric perspective, the camera is normally positioned at a 45-degree angle from the north-south axis of the landscape.“
  - S. 221: „… the isometric perspective distorts reality somewhat because objects that are farther from the [camera] … not smaller on the screen. However, the camera does not display much of the landscape at one time, so players don’t mind the slight distortion. The player can truck or dolly the camera above the landscape but cannot pan, tilt …“
  - S. 459: „isometric perspective so the player can see the whole party“ / „Baldur’s Gate II: Throne of Bhaal, which illustrates this isometric perspective“
  - S. 477: „isometric perspective was once the de facto standard for party-based play“
  - S. 242: „In a top-down or isometric perspective in which the player sees the avatar from above …“
  - Index S. 666: „isometric perspective, 220–221, 242“
- Relevanz:
  - **wichtig für Behauptung 1**: 30° = Neigung von der Horizontalen; 45° = Azimut um die Hochachse → Autor-Formulierung „meist 30 bis 45 Grad“ vermischt zwei verschiedene Winkel
  - **belegt Behauptung 2 wörtlich**: „objects … farther from the camera are not smaller on the screen“ (S. 221)
  - Übersicht/Party (S. 459), Genre RPG/party-based (S. 477) → stützt 3 und 4
- Zitierwürdigkeit: Game-Design-Lehrbuch, nicht peer-reviewed · sekundär · kein Praxisbeleg
- Fundort im Kapitel: 9.1 Punkte 1–3; Genres; 9.2
- Volltext-Zugang: nein (nur Google-Books-Snippets); Seitenangaben aus Snippets
- Status in `literatur.bib`: nicht vorhanden

### [9] Nitsche, Michael: Video Game Spaces: Image, Play, and Structure in 3D Worlds
- Jahr: 2008 (Crossref: 2008-12-05; Open Library: 2008)
- Verlag: The MIT Press
- DOI: `10.7551/mitpress/9780262141017.001.0001` (DOI-Resolver: 302 → Crossref iPage, geprüft)
- ISBN: 978-0-262-14101-7 (print, Open Library); 978-0-262-25511-0 (eISBN, Crossref); 305 S.
- Verifikation: Crossref-Record (Titel, Autor Michael Nitsche, Typ `monograph`, MIT Press); Google Books `SearchWithinVolume` (ID `2Adk9hp8nh8C`) selbst abgefragt → Snippets mit Seitenzahlen
- Wörtliche Fundstellen (Snippets, selbst abgefragt; „…“ = Snippet-Lücke):
  - S. 99: „Overhead View … The overhead view consists of a viewing position that hovers above the virtual playground. The player is looking down onto the events on the surface of the virtual world below.“
  - S. 99: „Isometric views eliminate any distortion of the depicted shape caused by the perspective. There is no single focal point that would help to concentrate the picture or fixate its orientation. True isometric views are an artistic construct and always include a level of abstraction, because the real world is not perceived in that way.“
  - S. 100: „isometric perspective can lead to awkward pixilation especially in older games and many have instead opted for a different angle. Any of these overhead views—isometric or not—exclude complete examination of the world because the player cannot get closer or change the basic setup.“
  - S. 93: „overhead view on the virtual world (and related views such as isometric style)—often incorporating varying viewing angles, found, e.g., in strategy games such as Age of Mythology“
  - Index S. 299: „Isometric, 93, 99–100, 122“
- Relevanz:
  - belegt „kein Fluchtpunkt“ („no single focal point“, S. 99) und isometrisch als Unterfall der Overhead-View
  - **differenziert Behauptung 3**: Overhead-Views „exclude complete examination of the world“ (S. 100) → „gute Übersicht“ nur eingeschränkt
  - Strategie-Genre (S. 93); „varying viewing angles“ (S. 93) → Widerspruch zu „nie aus anderem Winkel“
- Zitierwürdigkeit: wissenschaftliche Monografie (MIT Press), nicht klassisch peer-reviewed · sekundär/akademisch · kein Praxisbeleg
- Fundort im Kapitel: 9.1 Punkte 1–3; 9.2/9.4
- Volltext-Zugang: nein (nur Google-Books-Snippets); Seitenangaben aus Snippets
- Status in `literatur.bib`: nicht vorhanden

### [10] Bellanger, Clint: „Isometric Tiles Math“ (Entwickler-Tutorial)
- Jahr: UNSICHER (keine Datumsangabe auf der Seite gefunden)
- Venue: clintbellanger.net (Entwickler-Blog/Tutorial); URL: https://clintbellanger.net/articles/isometric_math/ (HTTP 200)
- Verifikation: Seite selbst geladen und gelesen (HTML), keine Metadaten-Datenbank
- Wörtliche Fundstellen (selbst gesehen):
  - „This tutorial is for beginner game programmers looking to wrap their heads around isometric math.“
  - „In this example our isometric tiles are 128x64 pixels.“
  - „Increasing map X by +1 tile … increases screen.x by 64 (half our tile’s width) and screen.y by 32 (half our tile’s height).“
  - Formeln: `screen.x = (map.x - map.y) * TILE_WIDTH_HALF; screen.y = (map.x + map.y) * TILE_HEIGHT_HALF;`
  - „It’s the way that isometry is handled in the Tiled map editor“
- Relevanz:
  - Praxisbeleg für 2:1-Tile-Geometrie (128×64; halbe Werte 64/32) und Map→Screen-Umrechnung
  - keine Gradangabe; keine akademische Definition
- Zitierwürdigkeit: nein · Praxisbeleg (Blog/Tutorial) · **Praxisbeleg ja**
- Fundort im Kapitel: 9.1/9.3 (Projektionsformel, Bewegung)
- Volltext-Zugang: ja (frei)
- Status in `literatur.bib`: nicht vorhanden

---

## 2. Abgleich mit den Behauptungen des Autors (9.1)

- **Behauptung 1 — „Kamera schaut schräg von oben, meist von 30 bis 45 Grad“**
  - belegt: „tilted angle“ ohne Grad (Järvinen S. 114); „hovers above“ (Nitsche S. 99); 30° Neigung von der Horizontalen + 45° Azimut (Adams S. 220); echte Isometrie: 45° Gier + 35,26° Neigung (Salomon S. 65); Zeichenachsen 30° (Morling S. 31; Salomon S. 65)
  - WIDERSPRUCH/Präzisierung: Adams' 30° und 45° sind verschiedene Winkel (Neigung vs. Azimut); als Bereich „30–45°“ für die Neigung in keiner geprüften Quelle; Neigung ist 30° (2:1-Spielstil, rechnerisch aus Salomon S. 65/66) bzw. 35,26° (echte Isometrie, Salomon S. 65)
  - Status: **teilweise belegt, Formulierung zu präzisieren**
- **Behauptung 2 — „Kein Fluchtpunkt; Objekte werden nicht kleiner noch aus anderem Winkel sichtbar“**
  - belegt: Foley S. 231/233/234 (Parallelprojektion, konstante Verkürzung); Morling S. 31 („ignores perspective altogether“); Adams S. 221 („farther from the camera are not smaller on the screen“); Nitsche S. 99 („no single focal point“); Järvinen S. 114 („lines of perspective do not converge“)
  - nicht belegt/widersprüchlich: „nicht aus einem anderen Winkel“ — Nitsche S. 93: Overhead-/Isometric-Style mit „varying viewing angles“; Nitsche S. 100: Spiele weichen auf „a different angle“ aus; Sprite-Praxis zeichnet Figuren aus mehreren Richtungen (Praxisbeobachtung, keine Quelle) → Satz so nicht haltbar, streichen oder auf Kamera fixieren
  - Status: **Teil 1 (kein Fluchtpunkt/keine Verkleinerung) gut belegbar; Teil 2 (anderer Winkel) unbelegt**
- **Behauptung 3 — „Ziel: gute Übersicht über das Spielfeld“**
  - belegt: Järvinen S. 117 („lift the player above the ‚streets‘ to see the bigger picture“); Adams S. 459 („see the whole party“)
  - Einschränkung: Nitsche S. 100 (Overhead-Views „exclude complete examination of the world“); Adams S. 221 („does not display much of the landscape at one time“)
  - Status: **belegt, aber mit Einschränkung (keine vollständige Übersicht)**
- **Behauptung 4 — „‚Isometrisch‘ als Genre-Beisatz (Action-RPG, Strategie, Aufbausimulation)“**
  - belegt/teilbelegt: Järvinen S. 114 (Sim-Spiele, RPG/Baldur’s Gate, Strategie/Command & Conquer), S. 117 (God Games); Nitsche S. 93 (Strategie, Age of Mythology); Adams S. 477 („de facto standard for party-based play“, RPG); Pazera S. 559/UNSICHER + Kap. 9/10 (RTS/TBS)
  - Lücke: „Action-RPG“ als Genre-Label nicht in den geprüften Quellen; Beispiele Diablo/Disco Elysium nicht belegt → als eigene Beobachtung kennzeichnen
  - Status: **teilweise belegt (Strategie, Aufbau/Sim, RPG); „Action-RPG“ unbelegt**

## 3. Echte Isometrie vs. Videospiel-Isometrie (Kernbefund)

- echte Isometrie: drei Hauptachsen gleich verkürzt (Foley S. 234); Rotation ±45° um y-Achse und ±35,26° um x-Achse (Salomon S. 65); Standard h/w = 1/√3 → Zeichenachsen α ≈ 30°, Neigung ≈ 35° (Salomon S. 65); Verkürzungsfaktor 0,8165 (Salomon S. 64; Morling S. 38)
- Videospiel-Praxis: 2:1-Tiles (Pazera S. 559/UNSICHER; Bellanger 128×64); 2:1 entspricht Salomons „1:2 isometric projection“ mit h/w = 1/2 und Zeichenachsen 27° (Salomon S. 66; arctan 0,5 = 26,565° = eigene Rechnung); Kameraneigung dabei rechnerisch 30° (θ = arcsin(h/w), Salomon S. 65 + h/w = 1/2, eigene Rechnung)
- 45°-Variante: „military isometric“, h/w = 1 → α = 45° (Salomon S. 66) — andere Konvention, nicht Standard-Isometrie
- exakte 35,264°: Salomon schreibt „±35.26°“ (S. 65), nicht 35,264°; Wikipedia nennt „≈35.264°“, ist aber nicht zitierfähig → **35,26° belegt, 35,264°-Präzision UNSICHER**
- Wikipedia-Artikel selbst markiert „rarely truly isometric / 2:1 most common“ als `{{or}}` → **kein zitierfähiger Beleg für diese Kernaussage gefunden** (nur technische Fachliteratur [4] und Praxis [7]/[10])

## 4. Geprüft und verworfen / nicht belegbar

- Dunn, Fletcher; Parberry, Ian: 3D Math Primer for Graphics and Game Development, 2. Aufl. 2011, A K Peters/CRC Press, DOI `10.1201/b11152`, ISBN 9780429190926 (Crossref verifiziert) — Google-Books-Suche (ID `02WMiiWKzZEC`): „isometric“ → 0 Treffer, „projection“ → 20 Treffer (nur orthographische Projektion/Kamera) → **für 9.1 nicht brauchbar**
- Haigh-Hutchinson, Mark: Real Time Cameras, 2009, CRC Press, DOI `10.1201/9780429258190`, ISBN 9780429258190; Print-Ausgabe Morgan Kaufmann/Elsevier ISBN 9780123116345 (Crossref-Kapitel-DOIs `10.1016/B978-0-12-311634-5.*`) — Metadaten verifiziert; **Inhalt zum Thema Isometrie nicht geprüft** (kein Volltext)
- Schell, Jesse: The Art of Game Design (10th Anniversary), 2019, A K Peters/CRC Press, DOI `10.1201/b22101`, ISBN 9781315208435 (Crossref) — Metadaten verifiziert; **kein Isometrie-Beleg gefunden**, nicht weiter verfolgt
- Foley et al. 3. Aufl. (2013): ISBN nicht sicher verifiziert (Google-Books-ISBN-Abruf → 404) — nicht geprüft; 2. Aufl. [2] stattdessen belegt
- Perron, Bernard; Wolf, Mark J. P. (Hrsg.): The Video Game Theory Reader 2, Routledge 2008, DOI `10.4324/9780203887660` (Crossref); Wikipedia zitiert S. 158 (Kapitel „Understanding Digital Playability“, S. 155–172) für Zaxxon/isometrisch — **Inhalt nicht selbst geprüft**, daher kein Kandidat
- Collins, Steven: „Game Graphics During the 8-bit Computer Era“, SIGGRAPH Computer Graphics Newsletter 32(2), 1998 (Wikipedia-Ref; Original über archive.today) — **nicht selbst geprüft**, kein Kandidat
- usgamer (Signor 2014), Kotaku (Vas 2013): journalistische Praxisbelege aus Wikipedia-Refs — **nicht selbst geprüft/abgerufen**, nicht zitierwürdig
- ISO-Katalogseite `iso.org/standard/26094.html`, `…/26095.html`, `…/26096.html`: HTTP 403 (Cloudflare) — ISO-Original nicht einsehbar; DIN-Übernahme via Crossref [1]
- Semantic Scholar API: HTTP 429 (Rate-Limit) → keine zusätzliche Literatur
- OpenAlex `fulltext.search:"isometric video game"`: nur 2 Treffer (Konferenzpapier Novi Sad 2025, DOI `10.24867/bsd-2024-1-021`; finnisches Theseus-Bachelor-Projekt) — keine verwertbare Definition
- Crossref ISSN-Suche (`query.bibliographic=isometric`) in Game Studies (1604-7982), Games and Culture (1555-4120), IEEE Transactions on Games (2475-1502), Entertainment Computing (1875-9521), Journal of Gaming & Virtual Worlds (1757-191X), Loading… (1923-2691): **total-results 0** in allen sechs → keine Treffer in bibliografischen Metadaten

## 5. Praxisbelege (separat, nicht zitierwürdig)

- GDC Vault `https://gdcvault.com/browse?keyword=isometric` (HTTP 200, Titel/Sprecher selbst gelesen; Videoinhalte Paywall/nicht geprüft):
  - „Gathering Your Party with Project Eternity (GDC Next 10)“, Josh Sawyer (Obsidian Entertainment), GDC Next 2013, `/play/1019680` — isometrisches Party-RPG
  - „Classic Game Postmortem – POPULOUS“, Peter Molyneux (Lionhead Studios), GDC 2011, `/play/1014633` — God Game
  - „The View from Above: Designing Compelling Quests for ‚Diablo IV‘“, Harrison Pink (Cyan Worlds), GDC 2024, `/play/1034226`
  - („‚TUNIC‘: This Was Here the Whole Time“, Andrew Shouldice, GDC 2023 — nur Studio-Name „ISOMETRICORP Games Ltd.“, kein Isometrie-Inhalt belegt)
- Godot Engine Docs „Using TileSets“: „rectangular, hexagonal, or isometric (pseudo-3D perspective)“ (HTTP 200, Text selbst gelesen) — Engine-Dokumentation, kein Grad/keine Definition
- Bellanger-Tutorial [10]: 2:1-Tile-Mathematik (Praxisbeleg)

## 6. Suchlücken (explizit)

- **Keine peer-reviewte Zeitschriftenquelle mit expliziter Spiele-Definition** von „isometric“ gefunden; Crossref-ISSN-Suche in 6 Game-Studies-/Games-Journals = 0 Treffer; beste Treffer: Järvinen (DiGRA-Proceedings, Review-Status unklar) und Nitsche (MIT-Press-Monografie) — keine „sichere“ Peer-Review-Quelle
- **„30 bis 45 Grad“ als Neigungsbereich** in keiner Quelle; belegt sind 30° Neigung (Adams; 2:1-Praxis, rechnerisch) und 35,26° (echte Isometrie); 45° ist bei Adams Azimut bzw. bei Salomon „military isometric“ → Autor-Formulierung vermischt Winkel
- **35,264° exakt**: nur „35.26°“ (Salomon S. 65) und „close to 35°“ (S. 65); 0,8165 = cos 35,264° eigene Rechnung → exakte Zahl nicht wörtlich belegt
- **2:1 ↔ 26,565°/27°**: Salomon S. 66 belegt „1:2 … h/w = 1/2“ und „27° Isometric Projection“; exakte 26,565° nicht wörtlich; Wikipedia-Artikel ist `{{or}}`-markiert → nicht zitierfähig
- **Kein Beleg für „Objekte nicht aus anderem Winkel sichtbar“**: Nitsche S. 93/100 nennt „varying viewing angles“ und „different angle“; Sprite-basierte Spiele (Praxis) rendern Figuren in mehreren Richtungen → Behauptung einschränken
- **Praxisbelege mit konkreten Entwickleraussagen zu Kamerawinkeln** (Diablo, Age of Empires, SimCity 2000) fehlen; GDC-Talks nur auf Titel-Ebene, Video Paywall
- **Keine Belege für „Action-RPG“** als Genre-Label in den geprüften Quellen; Beispiele Diablo/Disco Elysium/Baldur’s Gate III nicht in zitierfähiger Quelle

## 7. Top-3 für 9.1

1. **[4] Salomon 2006** — technische Kernquelle: echte Isometrie 45°/35,26°, h/w = 1/√3, 2:1-Standard 27°, 45°-Militär-Isometrie; Crossref + Google-Books-Seiten belegt; DOI-Korrektur beachten
2. **[6] Järvinen 2002** — einzige Spiele-Definition (schräg von oben, kein Horizont, keine konvergierenden Linien) + Genres + „bigger picture“; Open-Access-PDF, Seiten belegt; Review-Status UNSICHER kennzeichnen
3. **[8] Adams 2010** — Game-Design-Lehrbuch: 30° Neigung/45° Azimut, „nicht kleiner auf dem Screen“, RPG/Party; Google-Books-Seiten 220–221, 459, 477; Jahr/Auflage UNSICHER

Ergänzend: [2] Foley (Parallelprojektion/kein Fluchtpunkt, S. 231–234) und [3] Morling (30°-Zeichenachsen, 0,8165, S. 31/38) als Geometrie-Belege; [9] Nitsche als akademische Differenzierung der Übersicht.
