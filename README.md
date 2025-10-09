## 🏛️ Richtstätten Oberösterreichs
**Ein historisches Kartenprojekt von Wolfram**

Diese interaktive Karte zeigt die ehemaligen **Richtstätten, Galgenhäuser, Abdeckerhäuser, Pranger, Kleindenkmäler** und **Flurnamen** mit Bezug zur Rechtspflege in Oberösterreich.  
Ziel ist es, bekannte und vergessene Orte der Rechtsprechung, der Schande und der Hinrichtung vom Mittelalter bis ins 19. Jahrhundert zu dokumentieren und sichtbar zu machen.

🌐 **Website:** [https://wolfundrabe.github.io/richtstaetten-ooe/](https://wolfundrabe.github.io/richtstaetten-ooe/)

---

### 🗺️ Karteninhalte
Auf der Karte sind verschiedene Kategorien durch farbige Marker gekennzeichnet:

| Farbe | Kategorie | Beschreibung |
|-------|------------|--------------|
| 🔴 Rot | Richtstätten | Hochgerichte, Galgen, Blutgerüste |
| 🟡 Gold | Galgenhäuser / Abdecker | Wohnorte von Henkern oder Schindern |
| 🔵 Blau | Kleindenkmäler | Armesünderkapellen, Kreuze, Gedächtnismale |
| 🟢 Grün | Flurnamen | Historische Flurbezeichnungen (z. B. Galgenfeld) |
| ⚫ Schwarz | Pranger | Orte öffentlicher Strafe und Schande |

---

### 📄 CSV-Struktur (`daten/richtstaetten.csv`)

Die Karte liest ihre Daten automatisch aus dieser Datei.  
Verwendet wird das **UTF-8-Format** mit **Kommas** als Trennzeichen.  

Spaltenüberschriften:

```
name,kategorie,lat,lng,beschreibung,link
```

Beispiel:

```csv
Hochgericht der Stadt Wels,Richtstätten,48.157892,13.991535,"Dreischläfriger Galgen, zahlreiche Skelettfunde",orte/hochgerichtwels.html
Schandkreuz,Pranger,48.1566,14.0285,"auf dem Stich von Merian aus dem Jahr 1640 rechts neben der kayserl. Burg zu sehen",bilder/schandkreuz.png
```

#### Hinweise:
- **Koordinaten:** Dezimalgrad (WGS84), kein „°“-Zeichen  
- **Kategorien:** müssen exakt heißen:  
  `Richtstätten`, `Galgenhäuser`, `Abdecker`, `Kleindenkmäler`, `Pranger`, `Flurnamen`  
- **Link:** optional – führt zu einer Detailseite oder zu einer externen Quelle (z. B. DORIS, ANNO)

---

### 🧭 Neue Orte hinzufügen
1. Öffne die Datei `daten/richtstaetten.csv` in Excel oder einem Texteditor.  
2. Ergänze neue Zeilen mit Kommas als Trenner.  
3. Speichere im **UTF-8-Format**.  
4. Lade die geänderte Datei auf GitHub hoch → „Commit changes“.  
5. Die Marker erscheinen automatisch auf der Karte.

---

### 📷 Hinweise zu Bildern
Bilder gehören in den Ordner `/bilder/`.  
Bitte achte auf eigene Aufnahmen oder gemeinfreie Quellen.  
Beispiel für eine Verlinkung in der CSV:
```
Schandkreuz,Pranger,48.1566,14.0285,"auf Merian-Stich 1640 abgebildet",bilder/schandkreuz.png
```

---

### 📚 Quellenkürzel

In der Spalte *Beschreibung* der CSV-Datei werden für Karten- und Archivquellen folgende Kürzel verwendet:

| Kürzel | Quelle | Zeitraum | Beschreibung |
|:-------|:--------|:----------|:--------------|
| **FK** | Franziszeischer Kataster | ca. 1820 – 1830 | Urmappe und Steuerkataster des 19. Jh. |
| **JL** | Josephinische Landesaufnahme | 1775 – 1777 | Erste militärische Landesaufnahme Österreichs |
| **FL** | Franziszeische Landesaufnahme | 1809 – 1818 | Zweite militärische Landesaufnahme (unter Kaiser Franz I.) |
| **LH** | Lambacher Hausmappe | ca. 1723 | Früheste bekannte Haus- und Grundkarte der Region Wels |

---

### 📬 Kontakt
Fragen, Anmerkungen oder neue Hinweise bitte an:  
📧 **[richtstaette-ooe@gmx.net](mailto:richtstaette-ooe@gmx.net)**
