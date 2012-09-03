#Gedanken zur Levelgenerierung#
**Montag, 3. September 2012**  

Wie ich bereits das ein oder andere Mal erwähnt habe, entwickeln wir seit knapp 3 Monaten ein eigenes Spiel. Uns ist wichtig, dass die Welt in diesem Multiplayer Spiel stark dynamisch ist.  

Leider haben wir bisher immernoch keinen idealen Ansatz dafür gefunden. Der erste Ansatz war ein Pattern Ansatz mit Prozeduraler Generierung. Das ganze funktioniert so, dass wir den 4 Kanten eines Quadrats eindeutige IDs geben, und dann diese Kanten passende Quadrate kleben. Hätte ein Quadrat dann z.B. an der Rechten Kante eine 1 (z.B. Sand), dann müsste das nächste Quadrat auf der Linken Seite auch eine 1 haben.  

Theoretisch klappt das so auch ganz gut, aber es ist zum Designen einfach nur grausam. Weiche Übergänge sind nahezu unmöglich und möchte man dann etwas wie Flüsse, Seen oder Meer mit Küste darstellen, gelangt man sehr schnell an seine Grenzen, oder aber an sehr Eckige, Unschöne, Karten.  

Es muss also irgendwas anderes her. Das ganze treibt mich momentan in den Wahnsinn und ist ein unheimlicher Show-Stopper für das Spiel, der sowohl an Motivation als auch Zuversicht nagt.  

Wir wollen jetzt mal probieren die die Quadrate drastisch zu vergrößeren, und in den Quadraten dann viele kleine Quadrate haben. So werden dann immer große Teile generiert und innerhalb der Bereiche könnte man dann deutlich mehr Details darstellen.  

Was haltet ihr davon? Am liebsten würde ich ja mit [Perlin Noise] Karten generieren und die dann nehmen. Allerdings habe ich hier wieder unheimliche Probleme mit den Texturen. Ein Shaderansatz für die Texturen wäre ganz nett, aber momentan würde das dann auf 4 Texturen begrenzen. Deutlich zu wenig :(  

Vlt. hilft es ja einfach mal den Frust runterzuschreiben ;(