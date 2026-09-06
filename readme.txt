=== Card Forms - Mobile First Form ===
Contributors: wpmfs
Tags: forms, card, mobile-first, gutenberg, responsive
Requires at least: 6.5
Tested up to: 7.0
Requires PHP: 7.4
Stable tag: 1.0.1
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
* Multiple Choice (Checkboxen als Cards)
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

= 1.0.1 =
Beim **Löschen** des Plugins werden Formulare und Einsendungen jetzt mit entfernt. Wer die Daten behalten will, deaktiviert das Plugin, statt es zu löschen.

= 1.0.0 =
Initial release of Card Forms.


