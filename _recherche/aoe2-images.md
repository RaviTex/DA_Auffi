# AoE2-Bildkandidaten für Kapitel 9.1 („Definition einer isometrischen Ansicht in Videospielen")

- Zugriffsdatum aller Abrufe: **2026-11-04**
- Zielstelle im Repo: `Platzer/kapitel2.tex`, Z. 11 `\section{Definition einer isometrischen Ansicht in Videospielen}` (im Gesamtdokument Kap. 9.1)
- Bewertungsraster = die drei Kriterien des Autors (`Platzer/kapitel2.tex` Z. 16–18): (1) gedrehte Ansicht 30–45°, (2) kein Fluchtpunkt, (3) gute Übersicht
- Arbeitsweise: nur lesend im Repo; keine `.tex`/`literatur.bib` geändert; geschrieben nur `_recherche/aoe2-images.md` + `_recherche/images/`
- Rohbelege (JSON/HTML) in `_recherche/images/_meta/` bzw. `_recherche/images/_meta/src/`

## Kurzfazit

- **3 Empfehlungen** = die drei DE-Screenshots ohne HUD: `aoe2_kandidat1.jpg`, `aoe2_kandidat2.jpg`, `aoe2_kandidat4.jpg` (alle 1920×1080, kein Text-Overlay, keine UI-Leisten)
- Alle 6 Steam-Kandidaten heruntergeladen und mit `read_image` selbst angesehen → Bildinhalte unten sind eigene Sichtprüfung, nicht Seitenbeschreibung
- **Keine freie Lizenz** auf der Steam-Store-Seite angegeben; dort nur Copyright-/Trademark-Hinweis
- Wikimedia Commons: **kein echter AoE2-Gameplay-Screenshot**; einziger „gameplay"-Treffer ist eine selbstgezeichnete HUD-Skizze (nicht brauchbar)
- Frei lizenzierte isometrische **Alternativbilder** existieren (Commons, GPL/CC BY-SA), visuell aber **nicht** geprüft → UNSICHER
- Rechtliche Bewertung ausdrücklich **nicht** hier, sondern bei Teammitglied `copyright-at`

---

## Kandidat A (Empfehlung 1) — `aoe2_kandidat1.jpg`

- **Lokaler Pfad:** `_recherche/images/aoe2_kandidat1.jpg`
- **Datei:** JPEG, 1.447.598 B, 1920×1080 (per `file` geprüft), sha256 `20c1bd45a8bf1851f2a9c267bb2b15ccdd98db3e7022b4dc9509c0a0c914d0bf`
- **Direkt-URL (vollauflösend):** https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/813780/ss_83253675c7af3ad5f3f2c1dc2c43c667000e0c4a.1920x1080.jpg?t=1790623375
- **Maschinenlesbare Quelle:** https://store.steampowered.com/api/appdetails?appids=813780&filters=screenshots,basic → `data.screenshots[2]` (= Anzeige-Position 3 von 12)
- **Fundseite:** https://store.steampowered.com/app/813780/Age_of_Empires_II_Definitive_Edition/ (HTTP 200, `<title>Age of Empires II: Definitive Edition on Steam</title>`)
- **Bildinhalt (Sichtprüfung):**
  - Europäisch anmutende Stadt mit roten Ziegeldächern, goldene Kuppel (Kirche/Kathedrale), Steintürme, Zelte
  - Herbstlaub, Fluss mit Wasserfall und steinerne Brücke, ein Segelschiff, dicht stehende Reiter-/Fußeinheiten in Blau/Grün
  - **Kein HUD**, keine UI-Leisten, kein eingebranntes Text-Overlay, kein Logo
- **Warum isometrisch gut sichtbar:**
  - Gebäude alle aus gleichem schrägem Blick von oben (Kriterium 1)
  - Dachkanten/Mauerfluchten bleiben parallel, keine Fluchtpunkte (Kriterium 2)
  - große Spielfeldfläche gleichzeitig lesbar, Einheiten + Gebäude + Gelände in einem Bild (Kriterium 3)
- **Rechteinhaber laut Seite:** Publisher `Xbox Game Studios`; Store-Hinweis im Wortlaut: „© 2024 Microsoft. Microsoft, World's Edge, Age of Empires, and the Age of Empires logo are trademarks of the Microsoft group of companies. All rights reserved."
- **Nutzungsbedingungen der Fundstelle (Kurzzitat):** keine Reuse-/Bildlizenz auf der Store-Seite angegeben; nur o. g. Copyright-Zeile + Steam-Footer „© Valve Corporation. All rights reserved. All trademarks are property of their respective owners in the US and other countries." (Steam-SSA-Zitat siehe Abschnitt „Nutzungsbedingungen")
- **Lizenzstatus:** frei lizenziert **nein** (keine Lizenz/Erlaubnis auf der Fundstelle angegeben)
- **Login nötig:** **nein** (Bild-URL per `curl` ohne Cookie/Login mit HTTP 200 geladen)

## Kandidat B (Empfehlung 2) — `aoe2_kandidat2.jpg`

- **Lokaler Pfad:** `_recherche/images/aoe2_kandidat2.jpg`
- **Datei:** JPEG, 1.537.346 B, 1920×1080, sha256 `05927fd4540339bd442b693f8feb55944bd43f7d716f6cc1eb9b6bbc88b14529`
- **Direkt-URL (vollauflösend):** https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/813780/ss_77792f8c4a7b375fc7c749b6336e61d61830920b.1920x1080.jpg?t=1790623375
- **Maschinenlesbare Quelle:** Steam-Appdetails 813780 → `data.screenshots[6]` (= Position 7 von 12)
- **Fundseite:** https://store.steampowered.com/app/813780/Age_of_Empires_II_Definitive_Edition/
- **Bildinhalt (Sichtprüfung):**
  - Dichte, komplett ummauerte Stadt (Kathedrale/Duomo mit Kuppel, Glockenturm, Tortürme, Marktplätze)
  - gepflasterter Platz mit klar erkennbarem **diagonalem Kachelraster**, viele Figuren, Pferde, Karren
  - Meer/Fluss im linken oberen Eck; **kein HUD**, kein Overlay, kein Logo
- **Warum isometrisch gut sichtbar:**
  - gleichbleibender schräger Blickwinkel über die ganze Stadt (Kriterium 1)
  - Bodenkacheln laufen als 2:1-Rauten/Diagonalen weiter, parallele Kanten, kein Fluchtpunkt (Kriterium 2)
  - maximale Gebäudedichte bei gleichzeitig guter Lesbarkeit = Musterbeispiel für „gute Übersicht" (Kriterium 3)
- **Rechteinhaber laut Seite:** s. Kandidat A (`Xbox Game Studios` / „© 2024 Microsoft …")
- **Nutzungsbedingungen der Fundstelle (Kurzzitat):** wie Kandidat A — keine Bildlizenz auf der Store-Seite angegeben
- **Lizenzstatus:** frei lizenziert **nein**
- **Login nötig:** **nein**

## Kandidat C (Empfehlung 3) — `aoe2_kandidat4.jpg`

- **Lokaler Pfad:** `_recherche/images/aoe2_kandidat4.jpg`
- **Datei:** JPEG, 1.286.925 B, 1920×1080, sha256 `17ad1b8df0d0bbc92c776e6f4cd5a07a764c694a84cda6ee15bea6a305f224d5`
- **Direkt-URL (vollauflösend):** https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/813780/ss_b42dec99b197fea9882abc333e2cfb0a77dd3ed2.1920x1080.jpg?t=1790623375
- **Maschinenlesbare Quelle:** Steam-Appdetails 813780 → `data.screenshots[8]` (= Position 9 von 12)
- **Fundseite:** https://store.steampowered.com/app/813780/Age_of_Empires_II_Definitive_Edition/
- **Bildinhalt (Sichtprüfung):**
  - belagerte Stadtmauer mit Torturm/Wehrgang, dahinter Burg- und Wohngebäude; zwei steinerne Brücken über einen Fluss
  - Belagerungswaffen und Infanterie/Kavallerie beider Seiten am Ufer, Wasser + Sandstrand
  - **kein HUD**, kein Overlay, kein Logo
- **Warum isometrisch gut sichtbar:**
  - Uferlinien/Flusslauf und Mauern in derselben schrägen Draufsicht (Kriterium 1)
  - Brücken und Wasserflächen zeigen die typische Rauten-/Diagonalgeometrie ohne Fluchtpunkt (Kriterium 2)
  - Übersicht über zwei Uferseiten + Gebäude + Einheiten in einem Bild (Kriterium 3)
- **Rechteinhaber laut Seite:** s. Kandidat A (`Xbox Game Studios` / „© 2024 Microsoft …")
- **Nutzungsbedingungen der Fundstelle (Kurzzitat):** wie Kandidat A — keine Bildlizenz auf der Store-Seite angegeben
- **Lizenzstatus:** frei lizenziert **nein**
- **Login nötig:** **nein**

---

## Reserve-Kandidaten (selbst geprüft, nicht empfohlen)

| # | Datei | Auflösung | Inhalt (Sichtprüfung) | Warum nicht empfohlen |
|---|-------|-----------|------------------------|----------------------|
| D | `aoe2_kandidat3.jpg` | 1920×1080 | Nahaufnahme Felder/Windmühlen, Dorf, Stadtmauer rechts; kein HUD | Motiv zeigt kaum Gebäude/Einheiten → Isometrie weniger anschaulich |
| E | `aoe2_kandidat5.jpg` | 1920×1080 | HD Edition, echte Spielansicht **mit vollem HUD**: Ressourcenleiste oben (1000/1000/1200/200, Pop 7/75), „Castle Age", Minimap, „Age of Empires HD Edition"-Logo; Kartenburg, Moschee mit Kuppel, Hafen | HUD + eingebranntes Spiel-Logo; nur als Alternative, wenn bewusst eine echte Spielansicht mit UI gewünscht ist |
| F | `aoe2_kandidat6.jpg` | 1920×1080 | HD Edition, **HUD** („Feudal Age", Minimap, Logo); Burg auf Inseln zwischen Brücken, Wasser, Stadtmauer | wie E (HUD/Logo) |
| G | `aoe2_kandidat7_commons.png` | 1316×1024 | **kein Screenshot**: selbstgezeichnete HUD-Skizze (grüne Fläche, norwegische Labels „VED MAT GULL STEIN POPULASJON", „TIDSALDER", Kästchen 1–5, Raute „MINIKART"); Lizenz auf Commons: CC BY-SA 3.0, Artist „Arntor", Credit „Own work" | zeigt **keine** isometrische Ansicht → für 9.1 unbrauchbar |
| H | `aoe2_kandidat8_commons_gui.png` | 1920×1080 | echter Screenshot des DE-Szenario-Editors: Menüleiste oben, isometrisches Gelände, Start-TC, Einheiten, unten Kartengenerator-Panel, rautenförmige Minimap; Lizenz auf Commons: CC BY 3.0, Artist „Age of Empires", Credit: YouTube „Age of Empires II: DE – September Update Preview", Minute 1:02 | Motiv = leeres Gelände, keine Stadt; Lizenzlage des Spielinhalts unklar (UNSICHER) |

- Reserve-Direkt-URLs (Steam, AppID 813780, `?t=1790623375`):
  - kandidat3 (Position 12/12): https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/813780/ss_f270aa4e146459dc8b75a69bfecf23d13b0e8df6.1920x1080.jpg?t=1790623375 — sha256 `d4e91813a42b0b62f26b47a3ae2f2a6e91ae5fae622aac11cb15f94064b75f05`
- Reserve-Direkt-URLs (Steam, AppID 221380, `?t=1705596928`, Fundseite https://store.steampowered.com/app/221380/):
  - kandidat5 (Position 3/6): https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/221380/ss_9ccf9acb373b3e26f9e42a053147845561b2c224.1920x1080.jpg?t=1705596928 — sha256 `e741674e0234071896f082c32ee945c04dc2db13d1226e999187cdf34e673ebc`
  - kandidat6 (Position 4/6): https://shared.akamai.steamstatic.com/store_item_assets/steam/apps/221380/ss_5723ddcec6da4d9697f73882fab90e6cec99a8ad.1920x1080.jpg?t=1705596928 — sha256 `ae3b394a202915612cb210a46d1025f6e51dd14b728ed2e57e94e6196b8dfde1`
- Commons-Dateien/Belege:
  - kandidat7: https://upload.wikimedia.org/wikipedia/commons/2/26/Age_of_Empires_II_in_gameplay.png (Dateiseite: https://commons.wikimedia.org/wiki/File:Age_of_Empires_II_in_gameplay.png)
  - kandidat8: https://upload.wikimedia.org/wikipedia/commons/1/13/GUI_Editor_Age_of_Empires_II_Definitive_Edition.png (Dateiseite: https://commons.wikimedia.org/wiki/File:GUI_Editor_Age_of_Empires_II_Definitive_Edition.png)
- Ausgeschlossen (nicht heruntergeladen, nur Thumbnail geprüft): DE-Screenshots Position 1 und 2 (Motiv „East Asian/Japanese city" bzw. „Middle Eastern city") tragen ein eingebranntes Werbe-Overlay „NEW CO-OP MODE!" → für eine Abbildung ungeeignet
- Thumbnails aller 18 Store-Screenshots (12× AppID 813780, 6× AppID 221380) liegen in `_recherche/images/_meta/thumbs/`

## Steam-Metadaten der Fundstelle (verifiziert 2026-11-04)

- AppID 813780 (DE): Store-Seite HTTP 200; Publisher `Xbox Game Studios`; Developer `World's Edge, Forgotten Empires, …`; Released `14 Nov, 2019`; 12 Screenshots im `screenshots`-Array
- AppID 221380 (HD): Store-Seite HTTP 200, `<title>Age of Empires II (Retired) on Steam</title>`; Publisher `Xbox Game Studios`; Developer `Skybox Labs, Hidden Path Entertainment, Ensemble Studios, Forgotten Empires`; 6 Screenshots
- Hinweis: `filters=screenshots,basic` liefert `developers`/`publishers`/`release_date` = `null` → diese Felder wurden aus dem Store-Seiten-HTML gelesen
- Auf der HD-Store-Seite (221380) **kein** Microsoft-©-Hinweis im HTML gefunden, nur der Valve-Footer → UNSICHER, welche Copyright-Zeile für die HD-Bilder maßgeblich ist
- Bild-URLs funktionieren auch ohne den `?t=…`-Parameter (verifiziert: Download mit abgeschnittenem Query-String, HTTP 200, identische Dateigröße)
- Kein Wasserzeichen in den Bildern; die HD-Bilder (kandidat5/6) enthalten jedoch das „Age of Empires HD Edition"-Logo im HUD-Bereich

---

## Geprüfte weitere Quellen (Ergebnis)

- **ageofempires.com/games/aoeiide/**: HTTP 200; `<title>` = „Age of Empires II: Definitive Edition – Play with Game Pass for PC – Age of Empires – World's Edge Studio"; Footer „© 2026 Microsoft. All rights reserved."; 72 Bild-URLs auf `cdn.ageofempires.com` (webp, Update-/News-Grafiken, keine Screenshot-Galerie)
- **ageofempires.com/games/aoeiide/media/**: **HTTP 404** („Page Not Found") → kein offizielles Media-/Press-Kit auf diesem Pfad gefunden
- **Xbox Wire** (`news.xbox.com/en-us/?s=age+of+empires`): Suchseite HTTP 200; Artikel u. a. „Age of Empires II: Definitive Edition – The Viking Sagas Available Now" (2026-09-23); im geprüften Artikel **0 extrahierbare Bild-URLs** (`wp-content/uploads`) → UNSICHER, ob dort Pressebilder nutzbar sind; Footer „© Microsoft 2026"
- **GOG**: `gog.com/en/game/age_of_empires_ii_definitive_edition` leitet auf die GOG-Startseite (0 Treffer für „age of empires" im HTML); Catalog-API-Abfrage `like:age of empires` liefert 10 fremde Titel → **AoE2 nicht auf GOG** (Stand 2026-11-04) → keine GOG-Quelle
- **Microsoft Store / Xbox-Presseseite**: nicht geprüft → UNSICHER (Lücke)

## Wikimedia Commons (Commons-API, namespace 6)

- Suche „Age of Empires II": 138.583 Treffer; die ersten 20 sind überwiegend `.webm`-Trailer, Logos und Event-Grafiken — **kein freier Gameplay-Screenshot**
- `File:Age of Empires II in gameplay.png`: CC BY-SA 3.0, Artist „Arntor", Credit „Own work", 1316×1024, Datum 2012-08-10 → Sichtprüfung: **schematische HUD-Zeichnung, kein Screenshot** (Details oben, Kandidat G)
- `File:Age of Empires 2 Logo.svg`: „Public domain", 422×291, Artist „Ensemble Studios" → Logo, kein Gameplay
- `File:GUI Editor Age of Empires II Definitive Edition.png`: CC BY 3.0, 1920×1080, Artist „Age of Empires", Credit YouTube „Age of Empires II: DE – September Update Preview", Minute 1:02 → echter Editor-Screenshot (Kandidat H)
- `File:Age of Empires II- DE - …webm` (mehrere): Trailer, für Standbild nicht verwertet

## Frei lizenzierte isometrische Alternative (Fallback, Lizenz verifiziert, Motiv NICHT visuell geprüft)

| Spiel | Commons-Datei | Auflösung | Lizenz laut Commons-Metadaten | Artist/Credit |
|-------|---------------|-----------|-------------------------------|---------------|
| OpenTTD | `File:OpenTTD-15.3-en.png` | 1600×860 | GPLv2 (`gnu.org/licenses/old-licenses/gpl-2.0.html`) | „Screenshot: theki / Game: OpenTTD ; uses the OpenGFX graphics set", Credit „Own work" |
| 0 A.D. | `File:0 A.D. Alpha 23.jpg` | 1750×979 | CC BY-SA 3.0 | „0 A.D. Developers", Credit „Screenshot" |
| Unknown Horizons | `File:Unknown horizons 3176.PNG` | 1024×768 | CC BY-SA 3.0 | „The Unknown Horizons Team", Credit „Unknown Horizons homepage: screenshots" |
| The Battle for Wesnoth | `File:Battle for wesnoth version 1.12.0 screenshot.jpg` | 1280×768 | GPL (`gnu.org/licenses/gpl.html`) | „Battle for Wesnoth developers.", Credit „Battle for Wesnoth website" |
| (AoE2) | `File:Age of Empires II in gameplay.png` | 1316×1024 | CC BY-SA 3.0 | „Arntor", Credit „Own work" — **kein Screenshot**, s. o. |

- Dateiseiten (jeweils mit Lizenzbaustein): `https://commons.wikimedia.org/wiki/<Dateiname>`
- AttributionRequired laut Commons-Metadaten: bei allen fünf `true`
- **UNSICHER:** ob die Motive die isometrische Ansicht gut zeigen (OpenTTD/Unknown Horizons gelten als isometrisch, 0 A.D. = freie 3D-Kamera, Wesnoth = Hexfeld-2D) → nicht per `read_image` geprüft, da Auftrag auf AoE2 fokussiert war
- **UNSICHER:** Eignung von GPL-lizenzierten Screenshots für den Nachdruck in einer Diplomarbeit — Bewertung bei `copyright-at`

## Nutzungsbedingungen — Zitate (Wortlaut, ohne Interpretation)

- **Steam Store-Seite 813780**, Copyright-Hinweis (Element `game_area_legal`): „© 2024 Microsoft. Microsoft, World's Edge, Age of Empires, and the Age of Empires logo are trademarks of the Microsoft group of companies. All rights reserved. Acceptance of Microsoft Services Agreement and Privacy Statement required to play."
- **Steam Store-Seite**, Footer: „© Valve Corporation. All rights reserved. All trademarks are property of their respective owners in the US and other countries."
- **Steam Subscriber Agreement** (https://store.steampowered.com/subscriber_agreement/english/, HTTP 200), Abschnitt „2. LICENSES – A. General Content and Services License": „Valve hereby grants, and you accept, a non-exclusive license and right, to use the Content and Services for your personal, non-commercial use (except where commercial use is expressly allowed herein or in the applicable Subscription Terms). … The Content and Services are licensed, not sold. Your license confers no title or ownership in the Content and Services."
- **Steam SSA**: enthält **kein** Vorkommen des Wortes „screenshot" (Volltextsuche im abgerufenen HTML, 2026-11-04) → SSA regelt Bildverwendung nicht ausdrücklich; kein „Last Updated"/„Effective"-Datum im abgerufenen Text gefunden → UNSICHER
- **Microsoft Game Content Usage Rules** (https://www.xbox.com/en-US/developers/rules, HTTP 200): „Last Updated: January 2015"; Grant: „Microsoft grants you a personal, non-exclusive, non-sublicenseable, non-transferable, revocable, limited license for you to use and display Game Content and to create derivative works based upon Game Content, strictly for your personal, noncommercial (except as specifically provided below) use."
- **Game Content Usage Rules**, Pflichthinweis bei Weitergabe: „[Name of the Microsoft Game] © Microsoft Corporation. [The title of your Item] was created under Microsoft's 'Game Content Usage Rules' using assets from [Name of the Microsoft Game], and it is not endorsed by or affiliated with Microsoft." + Link auf die Rules verpflichtend
- **Game Content Usage Rules**, Anwendungsbereich: „These Rules apply to all games and Game Content published and owned by Microsoft Studios and for which Microsoft owns the copyright, trademark or other intellectual property." → **UNSICHER**, ob AoE2 DE (Publisher Xbox Game Studios / © Microsoft laut Store-Seite) darunter fällt; Bewertung: `copyright-at`
- **Commons-Dateiseite** `File:Age of Empires II in gameplay.png`: „I, the copyright holder of this work, hereby publish it under the following license: This file is licensed under the Creative Commons Attribution-Share Alike 3.0 Unported license." (Bedingungen: attribution, share alike, kein Endorsement)

## Rechtliche/technische Hürden & Lücken (Fakten, keine Bewertung)

- **Keine freie Lizenz** für die Steam-Bilder: Store-Seite nennt nur Copyright/Trademark, keine Erlaubnis zur Weiterverwendung; Steam-SSA enthält kein „screenshot"
- Lizenzlage der **Commons-Dateien** widersprüchlich zuordenbar: CC-/GPL-Angaben beziehen sich auf Uploader-Leistung (Screenshot-Aufnahme), die Spielinhalte selbst sind kommerziell → **UNSICHER**, ob die Commons-Lizenz die Microsoft-Rechte abdeckt (bei `File:GUI Editor …` stammt das Bild nachweislich aus einem offiziellen Age-of-Empires-YouTube-Video)
- **Kein offizielles Presse-/Media-Kit** mit Nutzungserlaubnis gefunden (`…/games/aoeiide/media/` = HTTP 404); Microsoft Store/Xbox-Presseseite ungeprüft → Lücke
- **Technisch unproblematisch:** alle 8 Dateien ohne Login/Cookie per HTTPS abrufbar (HTTP 200, `curl`); 1920×1080 reicht für Abdruck bis ca. 16 cm Breite bei 300 dpi
- **Technische Stolperstelle:** `upload.wikimedia.org` lieferte 2× HTTP 429 (Rate-Limit); Retry mit Pause + eigenem User-Agent erfolgreich
- **Kein frei lizenzierter echter AoE2-Gameplay-Screenshot** gefunden → falls eine freie Lizenz zwingend ist, bleibt nur (a) Erlaubnisanfrage bei Microsoft/World's Edge, (b) Fallback auf OpenTTD/0 A.D./Unknown Horizons (Lizenz ja, Motiv ungeprüft, Isometrie-Eignung UNSICHER), oder (c) Bewertung durch `copyright-at` (GCUR / Bildzitat § 42f UrhG)
- **Empfehlung für die Abbildung:** Kandidat A/B/C als Bilddatei verwenden, Bildnachweis „Age of Empires II: Definitive Edition, © Microsoft / Xbox Game Studios, Screenshot: Steam-Store-Seite (AppID 813780), abgerufen 2026-11-04" — endgültige Formulierung und Zulässigkeit: `copyright-at`
