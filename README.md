# Wo & Wann? — Geschichte entdecken, statt Jahreszahlen auswendig zu lernen

<p align="center">
  <img src="public/assets/logo-wo-und-wann.png" alt="Wo & Wann? – Logo" width="520">
</p>

**Wo auf der Welt bist du – und in welchem Jahr?** In *Wo & Wann?* erkundest du historische Schauplätze als drehbare 360°-Szenen. Du suchst Hinweise in Architektur, Maschinen, Kleidung und Umgebung, setzt deinen Tipp auf eine Weltkarte und wählst ein Jahr auf der Zeitleiste. Erst danach erfährst du, was an diesem Ort passiert ist – und warum es für die Geschichte der Weltwirtschaft wichtig war.

**[▶ Im Browser spielen](https://wo-wann.vercel.app/)** · [So funktioniert es](#so-funktioniert-das-spiel) · [Lokal starten](#lokal-starten)

> **Projektstatus:** Spielbarer Web-Prototyp mit historisch inspirierten **KI-Rekonstruktionen**. Die Bilder sind keine Originalfotografien; ihre historische und geometrische Endprüfung ist noch nicht abgeschlossen.

## Ein Blick ins Spiel

Die folgenden Bilder sind **echte Szenenbilder aus dem Repository**, keine nachträglich angefertigten Werbegrafiken. Im Spiel kannst du dich innerhalb dieser Panoramen umsehen.

| Früher globaler Handel | Industrielle Massenproduktion | Moderne Lieferketten |
| :---: | :---: | :---: |
| <img src="public/assets/orte/amsterdam-voc-werft.jpg" alt="KI-Rekonstruktion der VOC-Werft in Amsterdam" width="310"> | <img src="public/assets/orte/automobilfabrik.jpg" alt="KI-Rekonstruktion einer frühen Automobil-Montagehalle" width="310"> | <img src="public/assets/orte/taiwan-chips.jpg" alt="KI-Rekonstruktion einer modernen Halbleiterfertigung" width="310"> |
| VOC-Werft in Amsterdam, um 1670 | Ford-Produktion in Highland Park, 1913 | Halbleiterfertigung in Taiwan, 2023 |

*Alle drei Motive sind KI-generierte historische bzw. zeitgenössische Rekonstruktionen. Sie illustrieren die Lerninhalte, sind aber keine fotografischen Belege.*

## Warum wir das gebaut haben

Das Projekt entstand als **Creative Assignment** in der WU-Lehrveranstaltung *ZuWi – Von Handelskompanien zu Multinational Corporations* (Matteo Winter und Niklas Meller; Betreuung: Wolfgang Gruber).

Die Leitfrage dahinter: **Wie lässt sich die Entstehung der globalisierten Wirtschaft unmittelbar erfahrbar machen?** Zwischen einer Werft der Niederländischen Ostindien-Kompanie, einer industriellen Fließbandfertigung und einer heutigen Chipfabrik liegen Jahrhunderte – aber auch Verbindungen über Handel, Rohstoffe, Arbeit, Kapital und Macht.

Anstatt diese Entwicklung ausschließlich über Texte und Jahreszahlen zu vermitteln, macht das Spiel daraus eine Entdeckungsaufgabe. Wer einen Ort und eine Zeit schätzen muss, achtet auf konkrete Spuren. Die Auflösung verknüpft das Gesehene anschließend mit dem historischen Hintergrund. Das Spiel soll **Neugier auslösen**, nicht den Besuch eines Geschichtsarchivs oder sorgfältige Quellenarbeit ersetzen.

## So funktioniert das Spiel

1. **Themen auswählen:** *Produktion*, *Handel & Macht* und/oder *Wendepunkte*. Die Länge einer Runde lässt sich von **1 bis 9 Szenen** einstellen.
2. **Umsehen:** Ein 360°-Panorama aus einem festen Kamerastandpunkt erkunden. Du kannst die Ansicht drehen; es gibt keine frei begehbare 3D-Welt.
3. **Wo und wann raten:** Auf der zoombaren Weltkarte einen Ort markieren und auf der Zeitleiste ein Jahr auswählen (**1600–2025**).
4. **Auflösen:** Bis zu **10.000 Punkte je Szene** sammeln – bis zu 5.000 für die räumliche Einschätzung und 5.000 für die zeitliche. Ein richtiges Land erhält die vollen Ortspunkte; sonst fließt die Entfernung zur tatsächlichen Position ein. Bei der Jahreswertung zählt die Abweichung.
5. **Etwas lernen:** Die Auflösung zeigt den richtigen Ort und das Jahr, die Abweichung deiner Tipps, historische Erklärungen und visuelle Hinweise. Nach der Runde erscheint eine Gesamtübersicht.

Die Auswahl berücksichtigt bereits gespielte Orte im Browser, damit sich neue Szenen möglichst vor Wiederholungen zeigen. Die letzte Rundenpunktzahl wird lokal gespeichert. **Es gibt aktuell keine öffentliche Online-Bestenliste.**

### Inhaltlicher Schwerpunkt

Die Orte reichen von der frühen Neuzeit bis ins 21. Jahrhundert und verknüpfen drei Perspektiven:

- **Produktion:** Technischer Wandel, Arbeitsbedingungen, Industrialisierung und Ressourcen.
- **Handel & Macht:** Handelskompanien, Kolonialismus, Transport und internationale wirtschaftliche Verflechtungen.
- **Wendepunkte:** Ereignisse, an denen sich politische und wirtschaftliche Strukturen sichtbar verändert haben.

## Aktueller Stand und Grenzen

Der Datenbestand unter [`public/data/orte.json`](public/data/orte.json) enthält derzeit **29 konfigurierte Szeneneinträge** mit zugehörigen Bilddateien; daneben existieren [drei frühe technische Testpanoramen](public/data/scenes.json). Einige Pilotmotive überschneiden sich inhaltlich mit dem Hauptkatalog.

Das getrennte [Produktionsziel umfasst 30 kuratierte historische Schauplätze](docs/SCENE_MASTERPLAN_30.md). **Spielbar / eingebunden** bedeutet dabei ausdrücklich **nicht** historisch und geometrisch endgültig freigegeben: Für den verbindlichen 30er-Plan sind noch **0 von 30** Panoramen formal vollständig abgenommen. Details zu Bildauswahl, offenen Remakes und Qualitätskriterien stehen im [Bildproduktionsstatus](docs/IMAGE_PRODUCTION_STATUS_30.md).

Besonders wichtig:

- KI-Rekonstruktionen zeigen plausible zusammengesetzte Szenen, keine authentischen Fotoaufnahmen der Vergangenheit.
- Bilddetails und historische Aussagen müssen getrennt überprüft werden; ein überzeugend aussehendes Bild ist kein Beleg.
- Ein 2:1-Bild ist nicht automatisch ein korrektes, nahtloses Kugelpanorama. Die technische Qualität wird eigens geprüft.
- Die Kartenabfrage nutzt **heutige Ländergrenzen**, auch wenn die Szene aus einer früheren Epoche stammt.

## Lokal starten

Voraussetzung ist nur **Python 3** oder ein anderer statischer Webserver; es gibt keinen Build-Schritt und keine Datenbank.

```bash
git clone https://github.com/Matteo-Winter/Wo-Wann-Spiel.git
cd Wo-Wann-Spiel
python3 -m http.server 8000 --directory public
```

Öffne anschließend **http://localhost:8000**. Der 360°-Viewer lädt [Pannellum](https://pannellum.org/) über ein CDN; dafür wird eine Internetverbindung benötigt.

### Technischer Aufbau

| Bereich | Umsetzung |
| --- | --- |
| Weboberfläche und Spiellogik | HTML, CSS und JavaScript in [`public/index.html`](public/index.html) |
| 360°-Ansichten | Pannellum mit equirectangularen Panoramabildern |
| Spielinhalte | JSON mit Ort, Land, Jahr, Auflösung, Hinweisen und Bildpfad |
| Weltkarte | SVG auf Basis von Natural Earth; Zoom, Verschieben und Positions-Pin |
| Speicherung | Browser-`localStorage` für Einstellungen, Szenenwiederholungen und letzte Runde |
| Hosting | Statische Website aus `public/` über Vercel |

### Tests und Bildprüfung

```bash
python3 -m pip install -r requirements-qa.txt
python3 -m unittest discover -s tests -p 'test_*.py' -v
python3 scripts/check_panorama.py public/assets/panoramas/*.jpg
```

Die Bild-QA liefert Diagnosewerte, **keine automatische historische oder visuelle Freigabe**. Zusätzlich gibt es Werkzeuge für perspektivische Prüfseiten und die lokale Einzelbildansicht.

## Projektdokumentation

- [Szenen-Masterplan: alle 30 geplanten Schauplätze](docs/SCENE_MASTERPLAN_30.md)
- [Aktueller Bild- und Freigabestatus](docs/IMAGE_PRODUCTION_STATUS_30.md)
- [Lokale 360°-Tests und Bedienung](docs/LOCAL_360_TEST.md)
- [Panorama-Pipeline und Qualitätsanforderungen](docs/PANORAMA_PIPELINE.md)
- [Technische Panorama-QA](docs/PANORAMA_QA_PROBES.md)
- [Quellen und Lizenzen der historischen Startseitenbilder sowie Kartendaten](docs/START_SCREEN_IMAGES.md)

## Mitwirkende und Hinweise zur Nutzung

**Konzept und Umsetzung:** Matteo Winter & Niklas Meller im Rahmen des genannten WU-Kurses. Historische Inhalte und Szenen werden weiter recherchiert und geprüft.

Das Repository ist öffentlich einsehbar, enthält derzeit aber **keine explizite Software-Lizenz**. Eine öffentliche Bereitstellung ist nicht gleichbedeutend mit einer Freigabe zur beliebigen Weiterverwendung. Bildmaterial und historische Quellen sind gesondert zu betrachten.
