=== Card Forms - Mobile First Form ===
Contributors: wpmfs
Tags: forms, card, mobile-first, gutenberg, responsive
Requires at least: 6.5
Tested up to: 7.0
Requires PHP: 7.4
Stable tag: 1.1.0
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Modernes, card-basiertes Formularsystem mit Gutenberg-Integration. Mobile First Design für WordPress.

== Description ==

**Card Forms** ist ein innovatives Formularsystem für WordPress, das speziell für mobile Geräte entwickelt wurde. Mit einer modernen Card-basierten Benutzeroberfläche bietet es eine optimale User Experience auf allen Bildschirmgrößen.

= Features =

* 🎴 **Card-basiertes Design** - Eine Frage pro Ansicht für bessere Fokussierung
* 📱 **Mobile First** - Optimiert für Smartphones und Tablets
* 🎨 **Theme-Integration** - Übernimmt automatisch Farben und Schriften aus Ihrem Theme
* 📐 **Responsive Controls** - Separate Einstellungen für Desktop, Tablet und Mobile
* 🔀 **Conditional Logic** - Fragen basierend auf Antworten anzeigen/verstecken
* ⚡ **Performance** - Lädt CSS/JS nur wenn benötigt
* ♿ **Accessibility** - WCAG 2.1 AA konform
* 🌍 **Übersetzbar** - I18n ready

= Fragetypen =

* Single Choice (Radio Buttons als Cards)
* Such-Auswahl (Suchfeld über einer langen Optionsliste, z. B. Straßen)
* Multiple Choice (Checkboxen als Cards)
* Datenschutz-Zustimmung (Checkbox mit verlinktem Hinweistext)
* Textfeld (einzeilig)
* Textarea (mehrzeilig)
* Bewertungsskala (1-5 oder 1-10)

= Gutenberg Editor =

Vollständig in den Gutenberg-Editor integriert mit intuitiven Einstellungen:

* Live-Vorschau im Editor
* Drag & Drop für Fragenreihenfolge
* Responsive Einstellungen mit Device-Switcher
* Farbauswahl mit Theme-Integration

= Pro Version =

Erweitern Sie Card Forms mit zusätzlichen Features:

* Modal-Darstellung (Fullscreen)
* Zusätzliche Templates
* Erweiterte Conditional Logic
* Date Picker & File Upload
* CSV/JSON Export

[Mehr erfahren über Card Forms Pro](https://wpmfs.de/mm-wpmfs-card-forms-pro)

== Installation ==

= Automatische Installation =

1. Gehen Sie zu Plugins > Installieren in Ihrem WordPress-Dashboard
2. Suchen Sie nach "Card Forms"
3. Klicken Sie auf "Jetzt installieren"
4. Aktivieren Sie das Plugin

= Manuelle Installation =

1. Laden Sie die Plugin-Dateien in `/wp-content/plugins/mm-wpmfs-card-forms/` hoch
2. Aktivieren Sie das Plugin über das 'Plugins'-Menü in WordPress
3. Nutzen Sie den Card Forms Block in Ihrem Gutenberg-Editor

== Frequently Asked Questions ==

= Ist Card Forms DSGVO-konform? =

Ja, Card Forms speichert nur die eingegebenen Formulardaten. IP-Adressen und User-Agents können optional in den Einstellungen deaktiviert werden.

= Funktioniert Card Forms mit meinem Theme? =

Ja, Card Forms ist mit allen modernen WordPress-Themes kompatibel und übernimmt automatisch die Theme-Farben und Schriften.

= Kann ich die Farben anpassen? =

Ja, Sie können alle Farben über die Gutenberg-Einstellungen anpassen oder die Theme-Farben verwenden.

= Unterstützt Card Forms Conditional Logic? =

Ja, Sie können Fragen basierend auf vorherigen Antworten ein- oder ausblenden.

== Screenshots ==

1. Card-basiertes Formular auf Mobile
2. Gutenberg Editor mit Responsive Controls
3. Farbauswahl mit Theme-Integration
4. Conditional Logic Einstellungen
5. Formulare-Übersicht im Admin
6. Submissions-Ansicht

== Changelog ==

= 1.1.0 =
* Neuer Fragetyp „Such-Auswahl": über einer langen Optionsliste steht ein
  Suchfeld, das ab dem ersten Zeichen filtert. Vor der Eingabe sind nur die
  ersten Einträge sichtbar — gedacht für Listen wie Straße und Hausnummer, die
  als Radio-Liste unbrauchbar wären.
* Die Optionen dieses Typs lassen sich als Liste einfügen, getrennt durch
  Zeilenumbruch, Semikolon oder Komma. Bereits vergebene Werte bleiben beim
  Bearbeiten erhalten, damit gespeicherte Antworten weiter zugeordnet werden.
* Die Suche ignoriert Groß- und Kleinschreibung, Umlaute und die Schreibweise
  von „Straße": „hauptstr 12" findet die „Hauptstraße 12", und jede
  Zwischenstufe der Eingabe filtert mit.
* Neuer Fragetyp „Datenschutz": eine Pflicht-Checkbox mit formatiertem
  Hinweistext, in dem ein Link auf die Datenschutzerklärung stehen darf. Die
  Schriftgröße lässt sich getrennt einstellen. Erlaubt sind nur die Auszeichnungen
  a, strong, em, b, i, br und span; alles andere wird vor der Ausgabe entfernt.
* Nach dem Absenden lässt sich eine Weiterleitung einstellen, samt Verzögerung,
  damit die Dankesmeldung noch lesbar bleibt. Angenommen werden nur http und https.
* Die Zahl der sichtbaren Optionen der Such-Auswahl lässt sich getrennt für
  Desktop, Tablet und Mobil einstellen (Standard 8/6/4). Acht Karten plus
  Suchfeld schoben die Navigation auf dem Handy unter den Bildschirmrand.
  Eine bereits gespeicherte Einzelzahl gilt weiterhin, auf kleineren Geräten
  als Obergrenze.
* Fortschrittsleiste und „Frage x von y" stehen jetzt in einer Zeile statt
  übereinander und brauchen damit etwa halb so viel Höhe. Der Balken hat eine
  sichtbare Spur bekommen.
* Neue Einstellung „Eckenrundung" unter Layout: eine Zahl für das ganze
  Formular. Die inneren Ecken — Optionen, Felder, Buttons — folgen mit zwei
  Dritteln, die Fehlermeldung mit einem Drittel. Bisher hing nur die Karte an
  einem Wert, alles andere stand fest auf 8 bzw. 4 Pixeln. Fortschrittsbalken
  und das Häkchen der Danke-Seite bleiben rund, die sind formgebend.
* Das Suchfeld hatte 4 px Eckenrundung neben 8 px an den Optionen und war
  40 px hoch neben 56 px — Astra setzt für Eingabefelder eigene Höhe, Rahmen
  und Rundung. Es hat jetzt dieselben Maße wie die Optionsreihen.
* Rahmen setzen sich jetzt relativ zu der Fläche ab, die sie umschließen, statt
  die Rahmenfarbe des Themes zu übernehmen. Astra teilt sich dort einen
  Palettenplatz mit „Subtle Background"; in einer dunklen Palette steht darin
  oft ein Fast-Schwarz, und die Felder bekamen damit schwarze Kästen statt einer
  Kante. Auch die inaktive Spur des Fortschrittsbalkens ist jetzt eine Fläche
  und nicht mehr die Rahmenfarbe.
* Dunkelmodus: Karte, Optionen, Eingabefelder und gedämpfte Texte werden jetzt
  relativ zur Schriftfarbe abgesetzt statt fest auf Weiß bzw. `#666` zu stehen.
  Auf hellem Grund werden sie dunkler, auf dunklem heller — die Karte hebt sich
  in beiden Fällen vom Seitenhintergrund ab, und Felder und Optionen bleiben
  von der Karte unterscheidbar. Die Karte hat dafür zusätzlich eine Haarlinie
  bekommen: ihr Schatten ist reines Schwarz und auf dunklem Grund unsichtbar.
  Nachgemessen bleiben alle Texte über 4,5:1, hell wie dunkel.
* Der Absenden-Button trägt jetzt die Akzentfarbe statt eines fest verdrahteten
  Grüns. Das war als Erfolgsfarbe gemeint, stand neben einem andersfarbigen
  Theme aber wie ein Fremdkörper.
* Die Schriftfarbe der Buttons richtet sich nach dem Kontrast: Schwarz oder
  Weiß, je nachdem was auf der Buttonfläche besser lesbar ist. Gerechnet wird
  nach WCAG 2.1 (relative Leuchtdichte, Kontrastverhältnis) statt mit der alten
  YIQ-Faustformel — die wählte etwa auf `#7f7f7f` Weiß mit 4,00:1, wo Schwarz
  5,24:1 erreicht. Kommt die Akzentfarbe aus dem Theme, steht sie nur als
  CSS-Variable fest und lässt sich vorher nicht ausrechnen; dort entscheidet
  `contrast-color()` im Stylesheet, und wo der Browser das nicht kennt, springt
  eine Berechnung auf der gerenderten Fläche ein — im Frontend wie im Editor.
* Fragen ließen sich über die Oberfläche nicht löschen. Beide Papierkörbe
  hingen an `window.confirm()`, das in eingebetteten Ansichten unterdrückt wird
  und dann sofort „abgebrochen" meldet — der Klick tat schlicht nichts. Die
  Rückfrage ist entfernt; zurückgenommen wird wie bei Gutenberg-Blöcken mit ⌘Z.
* Schriftart und Textgröße kommen jetzt aus dem Theme. Die Größen für Text,
  Buttons und Beschreibung haben keinen eigenen Standard mehr; erst ein
  gesetzter Wert überschreibt das Theme, und der Regler lässt sich auf
  „Theme-Standard" zurücksetzen. Bisher erzwang der Block 18/16/14 px.
  **Hinweis:** Formulare, die diese Größen nie angefasst haben, übernehmen damit
  die Schriftgrößen des Themes.
* Die Optionen einer Auswahl sind `<label>`-Elemente, und Themes geben
  Formular-Labels gern eine eigene, kleinere Größe. Sie stehen jetzt wieder auf
  der normalen Textgröße, weil dort Inhalt steht und kein Feld-Titel.
* Das Suchfeld folgt derselben Textgrößen-Einstellung wie die übrigen Eingaben.
* Texte werden jetzt direkt auf der Leinwand bearbeitet statt über Felder in der
  Seitenleiste: der Platzhalter des Suchfeldes, die Beschriftungen von „Weiter",
  „Zurück" und „Absenden" sowie der Datenschutz-Hinweis samt Link. In der
  Seitenleiste bleiben nur die Texte, die auf der Leinwand nicht zu sehen sind
  (Danke-Nachricht, Text ohne Treffer, Fehlermeldung) — und alle Zahlen.
  Geblättert wird über die Pfeile in der Block-Werkzeugleiste; die Buttons auf
  der Leinwand sind jetzt Beschriftungen, keine Navigation.
* Editor und Frontend teilen sich ein Stylesheet. Das Aussehen der Komponenten
  stand bisher doppelt im Code — einmal in `assets/css/frontend.css`, die nur
  vorn eingereiht wurde, und in Teilen nachgebaut in `editor.scss`. Beide
  Fassungen liefen auseinander, die Vorschau zeigte etwas anderes als die Seite.
  Alles liegt jetzt in `src/style.scss`, die WordPress über `block.json` in der
  Leinwand **und** vorn lädt; in `editor.scss` bleibt nur noch Editor-Eigenes.
  Unterschiede laufen ausschließlich über die Tokens `--mmwpmfs-cf-*`.
* Die Fortschrittsleiste hält jetzt auch im Editor die eingestellte Kartenbreite
  und steht bündig über der Karte. Vorn tat sie das schon, in der Vorschau lief
  sie über die ganze Leinwand.
* Karte, Optionen und Buttons erklären ihr `box-sizing` selbst, statt sich auf
  den Reset des Themes zu verlassen. In der Editor-Leinwand fehlt der, wodurch
  die Karte ihre Max-Breite ohne das Padding rechnete und 64 px breiter wurde
  als eingestellt.
* Dabei behoben: die Fragen-Beschreibung war vorn ungestylt und übernahm die
  Absatzregeln des Themes, während der Editor sie formatierte. Sie sieht jetzt
  an beiden Stellen gleich aus.
* Die Editor-Vorschau folgt jetzt dem Geräteschalter. Bisher blieb sie für alle
  responsiven Einstellungen auf Desktop stehen, auch wenn oben Mobil gewählt war.
* „Card Max-Breite" ist mobil ein Prozentwert, sonst eine Pixelbreite. Der
  Editor rechnete überall mit Pixeln, wodurch die Karte in der Mobil-Vorschau
  auf 100 px zusammenfiel; der Schieberegler konnte den mobilen Standard von 100
  zudem gar nicht darstellen. Beide Stellen kennen die Einheit jetzt, und sie
  steht am Feld.
* Farben orientieren sich jetzt am Theme: Akzent, Text, Hintergrund und Rahmen
  kommen aus dessen Palette, und die Highlights — Auswahl, Fokus-Ring,
  Button-Hover — werden daraus abgeleitet statt fest verdrahtet zu sein. Im Block
  gesetzte Farben haben weiterhin Vorrang.

= 1.0.2 =
* Plugin-Symbol und -Banner werden jetzt an WordPress gemeldet und erscheinen in der Plugin-Liste und im „Details ansehen"-Dialog. Vorläufige Grafiken, bis endgültiges Material vorliegt.
* Der geteilte Update-Code trägt eine neue Versionsnummer. Ohne sie hätte die älteste installierte Kopie das Verhalten aller Plugins der Familie bestimmt.

= 1.0.1 =
* Beim Löschen des Plugins werden jetzt die eigenen Tabellen und Einstellungen entfernt. Bisher blieben Formulare, Einsendungen und Optionen dauerhaft in der Datenbank zurück.
* Im Netzwerkbetrieb wird pro Site aufgeräumt, nicht nur auf der aktuellen.

= 1.0.0 - 2025-11-21 =
* Umbenannt auf das Präfix der WPMFS-Familie: Plugin-Slug, Text Domain, Block
  (`mm-wpmfs/card-form`), REST-Namespace (`mm-wpmfs-card-forms/v1`), Optionen
  und Datenbanktabellen. Bestehende Entwicklungsdaten werden nicht migriert.
* Editor-Übersetzungen greifen wieder: sie hingen an einem Script-Handle, das
  nie eingereiht wurde.
* Blöcke ohne gesetzte Block-ID bekommen wieder eine gültige Wrapper-Klasse.
* Block-Kategorie „Mobile First" wird nicht mehr doppelt registriert.
* Initial Release
* Card-basiertes Formular-System
* 5 Basis-Fragetypen
* Responsive Controls
* Theme-Integration
* Conditional Logic
* Gutenberg Block

== Upgrade Notice ==

= 1.0.2 =
Bringt Symbole und Banner mit. Damit sie überall greifen, sollten alle Plugins der Familie aktualisiert werden.

= 1.0.1 =
Beim **Löschen** des Plugins werden Formulare und Einsendungen jetzt mit entfernt. Wer die Daten behalten will, deaktiviert das Plugin, statt es zu löschen.

= 1.0.0 =
Initial release of Card Forms.


