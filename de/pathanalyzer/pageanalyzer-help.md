# Einf�hrung in den Page Analyzer {#intro}
W�hrend die Haupt-Path Analyzer Anwendung, verf�gbar �ber das Launchpad, sich auf die fortgeschrittene Pfadanalyse konzentriert, konzentriert sich der Page Analyzer nur auf die Pfade, die zu einer bestimmten Seite f�hren bzw. von dieser wegf�hren. Das Hauptziel des Programms ist es zu verstehen, wie Kunden zu einem bestimmten Ziel (einer Seite) kommen und was sie danach tun.
Datenvisualisierung hilft Ihnen dabei die Pfade mit dem meisten Traffic (Besuche) und dem h�chsten Engagementwert pro Besuch zu verstehen,  so dass Sie gute und schlechte Pfade lokalisieren k�nnen. 
Sie k�nnen ein Drill-down f�r einen bestimmten Pfad veranlassen und so die Details des Pfads erkunden. 

## Lesen der Visualisierung {#map-key}
Die Visualisierung stellt die aktuell ausgew�hlte Seite in den Mittelpunkt (dargestellt als gro�er Kreis mit Seitensymbol) und zeigt alle Wege, die zu ihr hin und von ihr weg f�hren.

Der Landing-Bereich zeigt, wie viele Pfade mit der aktuell ausgew�hlten Seite begonnen haben.

Der Ausstiegsbereich zeigt die Anzahl der Ausstiege f�r die aktuell ausgew�hlte Seite und das insgesamt angesammelte [Ausstiegswertpotential](#exit-value-potential).

Die horizontalen Linien, die *zu* der aktuell ausgew�hlte Seite flie�en, repr�sentieren die ankommenden Pfade. 
Der oben auf den Linien liegende Kreis stellt die [Knoten](#node) auf dem Pfad dar. Grunds�tzlichen f�hren Knoten zu Seiten.

Die horizontalen Linien, die *von* der aktuell ausgew�hlte Seite nach rechts flie�en, repr�sentieren die ausgehenden Pfade.

Der oben auf den Linien liegende Kreis stellt die [Knoten](#node) auf diesem Pfad dar. Grunds�tzlichen f�hren Knoten zu Seiten.
Um die Visualisierung zu vereinfachen, wird nur die erste Seite auf ausgehenden Pfaden angezeigt.

Die Dicke der Linie definiert die Summe [Besuche](#visits) zur aktuell ausgew�hlten Seite von einem bestimmten Pfad aus. 
Je dicker der Pfad, desto mehr Besuche gehen zur der aktuell ausgew�hlten Seite f�r einen bestimmten Pfad. 

Die Linienfarbe definiert den [Wert pro Besuch](#value-per-visit) auf diesem bestimmten Pfad zur aktuell ausgew�hlten Seite. Je gr�ner der Weg, desto h�her der [Wert pro Besuch](#value-per-visit) im Vergleich zu anderen Pfaden, die zu der aktuell ausgew�hlten Seite f�hren. Pfade mit dem geringsten Wert pro Besuch werden in rot dargestellt.

Die Gr��e des Kreises definiert den Gesamtengagementwert auf dem Weg, der zu der aktuell ausgew�hlten Seite f�hrt. Je gr��er der Kreis, desto h�her der [Engagementwert](#value).

Der Context Pane Bereich die aggregierten Gesamtwerte f�r die Besuche-, Wert- und Wert pro Besuch-Metriken sowie die Gesamtanzahl der Pfade.
Wenn Sie den Mauszeiger �ber einem bestimmten Pfad schweben, zeigt der Gesamtwert-Bereich die Metriken dieses Pfades. 

## Karten-Selector {#map-selector}

Sie k�nnen verschiedene Karten mit dem Karten-Selector-Steuerelement ausw�hlen.
Sie k�nnen auch weitere Karten-Metadaten ansehen und eine Karte zu Ihrer Favoritenliste hinzuf�gen, die automatisch in Ihrem Profil gespeichert wird.

### Gruppen-Kartendaten {#group-map-data}

Karten bestehen aus seiner Baum-Datenstruktur, die wiederum aus  [Knoten](#node) besteht.
Weil erwartet wird, dass jeder [Knoten](#node) ein korrespondierendes Item in der Content (Master) Datenbank besitzt, wenn Sie das Kontrollk�stchen der Gruppen-Kartendaten des Karten-Selectors ausw�hlen; werden die Knoten vom Sitecore Datatemplate, von dem aus sie erstellt wurden, gruppiert. 
Beispielsweise k�nnen Sie diese beiden Pfade

- Home -&gt; TVs -&gt; 50" Flat Screen TV
- Home -&gt; Tablets -&gt; 12" Tablet

in einen einzigen Pfad gruppieren:  

- Landing Page -&gt; Produktkategorieseite -&gt; Produktdetailseite

Das Gruppieren von Kartendaten ist n�tzlich, wenn Sie eine Pfadanalyse auf einer Seitenkategorieebene im Vergleich zu einer einzelnen Seitenebene durchf�hren wollen. 

## Date Range Selector {#date-selector}
Sie k�nnen einen Datumsbereich des Datumsbereichselektors ausw�hlen, indem Sie entweder ein individuelles Start- und Enddatum aus den Kalendern oder indem Sie einen vordefinierten Datumsbereich ausw�hlen.

### Daten Fehlende Daten {#date-selector-missing-dates}
Es kann vorkommen, dass eine Karte keine Daten f�r einige Daten hat, auch wenn es verf�gbare Daten vor oder nach diesen Daten gibt. 
M�glicherweise gibt es keine aufgezeichneten Interaktionen f�r ein Datum oder es ist ein Fehler w�hrend der Datenverarbeitung aufgetreten und die Daten, die im Fehler vorkamen wurden �bersprungen. 
Der Datumsbereich-Selektor markiert Daten, f�r die keine Daten verf�gbar sind.  
Bitte kontaktieren Sie Ihren Systemadministrator, wenn Sie im Kalender auf viele Daten ohne Daten sto�en.

### Nicht verf�gbare Daten {#date-selector-unavailable-dates}
Je nach Datumsbereich, den Sie ausgew�hlt haben, kann es vorkommen, dass einige Daten als nicht ausw�hlbar markiert werden. Wenn Sie zum Beispiel ein Enddatum ausw�hlen, werden alle Daten vor dem aktuellen Startdatum als nicht verf�gbar gekennzeichnet. Alle zuk�nftigen Daten werden auch als nicht verf�gbar gekennzeichnet.

## Metrikfilter {#metrics-filter}
Dieser Filter konzentriert sich auf das Filtern von Knoten nach ihren wichtigsten Metriken: Besuche, Wert pro Besuch und Ausstiegswertpotential.
Sie k�nnen den Metrikfilter verwenden, um St�rungen zu reduzieren oder interessante Zusammenh�nge zwischen verschiedenen Metriken und um Kandidaten f�r eine Pfadoptimierung zu finden, zum Beispiel:

- Viele [Besuche](#visits), aber niedriger [Wert](#value).
- Hoher [Wert pro Besuch](#value-per-visit), aber wenige [Besuche](#visits).
- Hohes [Ausstiegswertpotential](#exit-value-potential).

## Anwendungsnachrichten {#application-messages}
Wenn Sie die Anwendung verwenden, sehen Sie verschiedene Meldungen in der Statusleiste.

### "Einige Pfade sind verborgen. Verwenden Sie den Filter, um andere Pfade sehen zu k�nnen." {#page-analyzer-hidden-paths}
Die Anwendung zeigt nur 10 Pfade auf einmal.
Sie k�nnen den Metriken-Filter verwenden, um die Anzahl der Pfade zu reduzieren, basierend auf beliebigen Metrik-Kriterien

### "Basierend auf 500 Pfaden aus X insgesamt." {#page-analyzer-maximum-paths}
Einige Seiten, wie die Homepage, k�nnen eine enorme Menge an eindeutige Pfade aufweisen, die durch sie hindurchlaufen. 
F�r eine bessere Effizienz, verarbeitet die Anwendung nur die Top 500-Pfade.
Sie k�nnen eine segmentiertere Karte ausw�hlen oder ein geringeres Datumsintervall.  

### "Die ausgew�hlte Karte wird erstellt. Sie sehen u.U. nur Teildaten." {#partial-map}
Diese Meldung wird angezeigt, wenn die aktuell ausgew�hlte Karte zwar kurzlich bereitgestellt wurde, jedoch der  Prozess des Aufbaus von Daten f�r diese Karte noch nicht abgeschlossen wurde. Daten f�r die neu bereitgestellte Karte sollten ca. 30 Minuten nach Bereitstellung der Karte verf�gbar sein.

## Glossar {#glossary}

### Karte {#map}
Eine spezielle Marketing-Definition, die beschreibt, wie man Daten f�r die Pfadanalyse erstellt. 
Der Page Analyzer verwendet Kartendaten und  filtert alle Pfade, um nur diejenigen anzuzeigen, die durch die aktuell ausgew�hlte Seite f�hren. Dieses gefilterte Dataset dient zur Visualisierung.
Sie k�nnen zu einer anderen Karte wechseln, indem Sie den [Karten-Selektor](#map-selector) verwenden. 

### Pfad {#path}
Eine Sequenz von [Knoten](#node) bilden einen Pfad. Alle im Page Analyzer angezeigten Pfade f�hren durch die aktuell ausgew�hlte Karte. 

### Knoten {#node}

Ein Element auf einem [Pfad](#path). F�r die misten Karten gilt, dass Knoten im Wesentlichen zu einer anderen Seite f�hren. 
Es gibt eine Reihe von Metriken, die auf jedem Knoten gespeichert sind: [Wert](#value), [Besuche](#visits),
[Wert pro Besuch](#value-per-visit), [Ausstiege](#exits), [Ausstiegswert](#exit-value), [Ausstiegswert pro Besuch](#exit-value-per-visit) und [durchschnittlich verbrachte Zeit](#average-time-spent).

### Ausstiegsknoten {#exit-node}

Knoten mit [Ausstiegen](#exits) gr��er als Null zeigen die Anzahl der [Besuche](#visits), die auf diesem Knoten beendet wurden.

### Besuchsmetrik {#visits}

Die Gesamtzahl der aggregierten Besuche auf einem bestimmten Knoten. Dazu geh�ren Besuchsmetriken von allen Nachfahrknoten.

### Wertmetrik{#value}
Der insgesamt aggregierte Engagementwert auf einem bestimmten Knoten. Dazu geh�ren Wertmetriken aus allen Nachfahrknoten. 

### Wert pro Besuchsmetrik {#value-per-visit}

Der aggregierte [Engagemenwert](#value) geteilt durch [Besuche](#visits) auf einem vorgegebenen Knoten.
Manchmal ist diese Metrik definiert als **Effizienz**.
Diese Metrik ist ma�geblich bei der Berechnung des [Ausstiegswertpotentials](#exit-value-potential).

### Ausstiegsmetrik {#exits}

Die Anzahl der Ausstiege auf einem vorgegebenen Knoten.
Diese Metrik gibt an, ob ein vorgegebener Knoten einen vollst�ndigen Pfad oder einen Einstiegspfadumfasst. 
Jeder Knoten mit Ausg�ngen gr��er als Null umfasst einen vollst�ndigen Pfad.
Diese Metrik ist ma�geblich bei der Berechnung des [Ausstiegswertpotentials](#exit-value-potential).

### Ausstiegswertmetrik {#exit-value}

Die aggregierten Engagementwerte auf einem bestimmten Knoten vor dem Ausstieg.
Nur Knoten bei denen Ausstiege stattgefunden haben besitzen diese Metrik.
Der Unterschied hierzwischen und der [Wertmetrik](#value) besteht darin, dass die Ausstiegwertmetrik nicht den Engagementwert der Nachfolgeknoten ber�cksichtigt

### Ausstiegswert pro Besuchsmetrik {#exit-value-per-visit}
Der aggregierte [Engagemenwert](#value) geteilt durch die [Besuche](#visits) auf einem vorgegebenen [Ausstiegsknoten](#exit-node). Nur f�r Knoten, auf denen Ausstiege stattgefunden haben, wird diese Metrik berechnet. 
Der Unterschied zwischen dieser Metrik und der [Wert pro Besuch](#value-per-visit) Metrik besteht darin, dass diese Metrik nicht den Engagementwert pro Besuch der Nachfahrknoten ber�cksichtigt. 
Diese Metrik ist ma�geblich f�r die Berechnung des [Ausstiegswertpotentials](#exit-value-potential).

### Ausstiegswertpotential-Metrik {#exit-value-potential}
Das Ausstiegswertpotential zeigt einen projizierten [Engagemenwert](#value), der durchschnittlich durch Optimierung gewonnen werden k�nnte.  
Es wird nur f�r die [Ausstiegsknoten](#exit-node) berechnet.
Sie k�nnen es als eine erweiterte Bounce-Metrik betrachten, wo neben den [Ausstiegen](#exits) auch der Engagementwertverlust oder Wertverlust ber�cksichtigt wird. 
Wenn man wei�, wie viel [Wert pro Besuch](#value-per-visit) auf allen weiter unten liegenden Pfaden angesammelt wird, und wie viel [Wert pro Besuch](#value-per-visit) im [Ausstiegsknoten](#exit-node) gespeichert wird, dann kann diese Metrik berechnet werden, indem 
man das Delta zwischen den beiden bildet und mit der Anzahl der Ausstiege multipliziert, unter der Verwendung der folgenden Formel:


(Wert pro Besuch � Ausstiegswert pro Besuch) * Ausstiege

