# Das Mysterium TrueCrypt
Der ein oder andere wird es schon gehört haben: Die Entwicklung der OpenSource Verschlüsselungssoftware "TrueCrypt" ist plötzlich eingestellt worden.

### Keine alten Versionen mehr
Die unbekannten Entwickler gehen sogar noch einen Schritt weiter und verkünden nicht nur das Ende ihrer Entwicklung, sondern nehmen alle alten Versionen des Krytoprogrammes offline. Stattdessen wird eine neue Version 7.2. veröffentlicht, welche Daten nicht mehr verschlüsseln kann und ausschließlich dazu dienen soll vorhandene verschlüsselte Daten zu portieren.

### Angebliche Sicherheitslücken
Auf der [TrueCrypt Webseite](http://truecrypt.sourceforge.net/) bekommen Besucher den Text **"WARNING: Using TrueCrypt is not secure as it may contain unfixed security issues"** angezeigt.

Die plötzliche Einstellung des Projektes und der Hinweis auf mögliche Sicherheitsprobleme sind äußerst merkwürdig. Erst vor wenigen Wochen wurde die Erste Phase eines [Code-Audits](http://de.wikipedia.org/wiki/Audit#Software) erfolgreich durchgeführt. Das [Ergebnis]() brachte keine außergewöhnlichen Fehler oder Sicherheitslücken zu Tage. Eine weitere Phase des Audits sollte ursprünglich in Kürze beginnen.

### Verschwörungstheorie: NSA hat Finger im Spiel
Kurz nach der Einstellung des Projektes sind bereits erste Verschwörungstheorien im Internet aufgetaucht. Viele Personen aus der Internet-Gemeinde sind fest davon überzeugt, dass hinter der Aktion die NSA steht.

So leiten einige bereits aus der von den vermutlichen TrueCrypt Entwicklern hinterlassenen Warnung einen Hinweis auf den US-Geheimdienst ab. Die Anfangsbuchstaben der Wörter in der Formulierung **"not secure as"** ergeben die Abkürzung *NSA*.

[Vergleicht](https://github.com/warewolf/truecrypt/compare/master...7.2) man die Vorgängerversion mit der Endgültigen TrueCrypt Version, so entdeckt man, dass z.B. plötzlich nach vielen Jahren ohne eine Änderung, nun die Sprachenhinweise von *"English (U.S.)"* auf *English (United States)* geändert wurde. (**UPDATE: Seit Visual Studio 2013 werden diese Strings wohl automatisch umbenannt.**) Solche Theorien sind natürlich sehr gewagt und auch mit großer Vorsicht zu beachten.

Es gibt allerdings auch andere Mysterien rund um das Thema TrueCrypt, welche Verschwörungstheorien momentan helfen einen festen Sockel zu geben. [Sucht](https://web.archive.org/web/*/http://www.truecrypt.org) man bei der WayBackMachine nach der TrueCrypt Homepage, bekommt man nur den Hinweis **"Der Zugriff auf den Inhalt ist gesperrt. Blocked Site Error"**.

Die WayBackMachine ist hier auch nicht der einzige Ort, an dem sämtliche Links gesperrt oder gelöscht wurden. Auch bei den Suchmaschinen der [PRISM](http://de.wikipedia.org/wiki/PRISM) Unternehmen Google, Mircrosoft (Bing) und Yahoo sind alle zwischengespeicherten (Cache) Seiten die auf die TrueCrypt Seite verwiesen haben verschwunden oder gelöscht worden.

Seit dem der eMail-Provider LavaBit bereits seine Pforten geschlossen hatte, weil der US-Geheimdienst die Privaten Sicherheitsschlüssel der Benutzer haben wollte. Vermuten zunehmend Leute, dass auch im Fall TrueCrypt die Entwickler die Reisleine gezogen haben, um z.B. den zwanghaften Einbau einer Sicherheitslücke zu verhindern.

### TrueCrypt Zukunft ungewiss
Während die TrueCrypt Webseite empfiehlt auf Produkte wie Bitlocker von Microsoft umzusteigen und hierfür sogar Migrationshilfen anbietet, ist die Netzgemeinde derzeit ratlos und hat noch keine sicheren OpenSource Alternativen zu bieten. Schaut man sich die Migrationshilfen für Macintosh Nutzer an, entdeckt man erneut etwas seltsames. So wird Schritt für Schritt erklärt wie man ein verschlüsseltes Laufwerk unter Macintosh erstellt, allerdings wird beim Feld "Encryption" also Verschlüsselung der Wert auf "none" gelassen. Sprich es würde gar keine Verschlüsselung erfolgen, sollte man der Anleitung folgen.

Einige Entwickler untersuchen momentan die Lizenz des TrueCrypt Quellcodes, um so eventuell einen Ableger des Projektes zu erstellen und weiterzuentwickeln.

Viele Fragen bleiben offen. Hatten die Entwickler keine Motivation mehr und wollten das Projekt einfach einstellen? Wurden die Entwickler zu etwas durch Behörden oder Geheimdienste gezwungen? Sehen wir hier einen typischen [*Warrant canary*](https://en.wikipedia.org/wiki/Warrant_canary)?

> Dieser Artikel befindet sich momentan in Entwicklung. Neuigkeiten werden oft ergänzt und Änderungen vorgenommen.
> Einige Informationen müssen noch durch seriöse Quellen belegt werden.
> Sollten weitere Infos bekannt werden, wird dieser Artikel aktualisiert.

Patrick Trautmann - 29.05.2014 Update: 30.05.2014

