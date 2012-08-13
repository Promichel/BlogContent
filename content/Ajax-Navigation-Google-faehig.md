# Eine Ajax Navigation Google fähig machen #
**Montag, 13. August 2012**  

Während der Programmierung dieses Blogs hier ist mir ein großer Stolperstein in den Weg gelegt worden. Der Google Crawler... Obwohl ich versuche kein Backend für diesen Blog zu verwenden, blieb mir nun nichts anderes als für das Feed System und den Google Bot eine Ausnahme zu machen.  
In diesem Beitrag möchte ich die Funktionsweise des Google Ajax crawlen ein bisschen erläutern und eine mögliche Vorgehensweise beschreiben.  

Eine Zeit lang bestand keine Möglichkeit Content, der über Javascript geladen wird, in den Google Suchmaschinen-Index zu bekommen. Im Jahr 2009 machte Google seinen Crawler Ajax fähig und somit Javascript Content indexierbar. Hierfür gibt es allerdings eine Beschränkung. Man muss sich an ein festes [Schema] halten.

**Die Links**  
Wenn man einen solchen Ajax Content-Load auf seiner Webseite realisiert, dann sind das in der Regel Relative Links, welche die aktuell aufgerufene Seite und einen Hash enthalten. (**Beispiel:** index.html#tollercontent)  

Während der Browser des Benutzers damit keinerlei Probleme hat und den Aufruf erfolgreich verarbeiten kann, wird der Google Crawler hier den Ajax Content nicht laden und anzeigen können.   

Die Spezifikation erfordert, dass der Link (**Beispiel:** index.html**#!tollercontent**) heißen muss.  

Doch damit ist es leider noch nicht getan, denn Google wird an der Stelle anschließend einfach nur das **#!** mit einem **?_escaped_fragment_=** ersetzen.  

**Was bedeutet das für mich?**  
Für euch bedeutet das, dass ihr sofern der Aufruf mit einem **escapedFragment** erfolgt, der Content der jeweiligen Seite direkt vom Webserver zurückgeliefert werden muss.  

Ihr müsst somit also eine Alternativ Abrufmöglichkeit für den Crawler schaffen. Je nachdem was für eine Sprache ihr also im Backend verwendet, müsst ihr schauen ob die jeweile Seite mit dem GET Parameter **escapedFragment** aufgerufen wurde. Im Falle des Beispiels müsste man das auf der Seite **index.html** kontrollieren. (Würde im Falle einer statischen HTML Seite nun schwierig werden ;D)  

Die Rückgabe des Webservers bei einem solchen Aufruf muss so aussehen, wie sie beim User **nach** dem Laden des Javascript Contents aussieht.  

Lest euch in Ruhe die [Schema] Beschreibung von Google durch und nutzt die Webmaster-Tools um zu prüfen, ob die Implementation funktioniert.  

**Und wie habe ich das gemacht?**  
Da ich für meinen Blog kein Backend verwende, war das ganze für mich natürlich ein bisschen schwieriger.  
Ich habe es gelöst in dem ich mit einer .htaccess auf den Parameter prüfe und bei einem Match auf eine PHP Seite weiterleite. Diese liefert den Content dann so zurück, wie es der Browser des Nutzers auch darstellen würde.  

**PS:** Diese Google Ajax-Richtlinien treffen auch auf Bing zu. Vermutlich auch auf Yahoo und co.

[schema]:https://developers.google.com/webmasters/ajax-crawling/docs/getting-started