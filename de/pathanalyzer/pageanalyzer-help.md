# Einführung in den Page Analyzer {#intro}
Während die Haupt-Path Analyzer Anwendung, verfügbar über das Launchpad, sich auf die fortgeschrittene Pfadanalyse konzentriert, konzentriert sich der Page Analyzer nur auf die Pfade, die zu einer bestimmten Seite führen bzw. von dieser wegführen. Das Hauptziel des Programms ist es zu verstehen, wie Kunden zu einem bestimmten Ziel (einer Seite) kommen und was sie danach tun.
Datenvisualisierung hilft Ihnen dabei die Pfade mit dem meisten Traffic (Besuche) und dem höchsten Engagementwert pro Besuch zu verstehen,  so dass Sie gute und schlechte Pfade lokalisieren können. 
Sie können ein Drill-down für einen bestimmten Pfad veranlassen und so die Details des Pfads erkunden. 

## Lesen der Visualisierung {#map-key}
Die Visualisierung stellt die aktuell ausgewählte Seite in den Mittelpunkt (dargestellt als großer Kreis mit Seitensymbol) und zeigt alle Wege, die zu ihr hin und von ihr weg führen.

Der Landing-Bereich zeigt, wie viele Pfade mit der aktuell ausgewählten Seite begonnen haben.

Der Ausstiegsbereich zeigt die Anzahl der Ausstiege für die aktuell ausgewählte Seite und das insgesamt angesammelte [Ausstiegswertpotential](#exit-value-potential).

Die horizontalen Linien, die *zu* der aktuell ausgewählte Seite fließen, repräsentieren die ankommenden Pfade. 
Der oben auf den Linien liegende Kreis stellt die [Knoten](#node) auf dem Pfad dar. Grundsätzlichen führen Knoten zu Seiten.

Die horizontalen Linien, die *von* der aktuell ausgewählte Seite nach rechts fließen, repräsentieren die ausgehenden Pfade.

Der oben auf den Linien liegende Kreis stellt die [Knoten](#node) auf diesem Pfad dar. Grundsätzlichen führen Knoten zu Seiten.
Um die Visualisierung zu vereinfachen, wird nur die erste Seite auf ausgehenden Pfaden angezeigt.

Die Dicke der Linie definiert die Summe [Besuche](#visits) zur aktuell ausgewählten Seite von einem bestimmten Pfad aus. 
Je dicker der Pfad, desto mehr Besuche gehen zur der aktuell ausgewählten Seite für einen bestimmten Pfad. 

Die Linienfarbe definiert den [Wert pro Besuch](#value-per-visit) auf diesem bestimmten Pfad zur aktuell ausgewählten Seite. Je grüner der Weg, desto höher der [Wert pro Besuch](#value-per-visit) im Vergleich zu anderen Pfaden, die zu der aktuell ausgewählten Seite führen. Pfade mit dem geringsten Wert pro Besuch werden in rot dargestellt.

Die Größe des Kreises definiert den Gesamtengagementwert auf dem Weg, der zu der aktuell ausgewählten Seite führt. Je größer der Kreis, desto höher der [Engagementwert](#value).

Der Context Pane Bereich die aggregierten Gesamtwerte für die Besuche-, Wert- und Wert pro Besuch-Metriken sowie die Gesamtanzahl der Pfade.
Wenn Sie den Mauszeiger über einem bestimmten Pfad schweben, zeigt der Gesamtwert-Bereich die Metriken dieses Pfades. 

## Karten-Selector {#map-selector}

Sie können verschiedene Karten mit dem Karten-Selector-Steuerelement auswählen.
Sie können auch weitere Karten-Metadaten ansehen und eine Karte zu Ihrer Favoritenliste hinzufügen, die automatisch in Ihrem Profil gespeichert wird.

### Gruppen-Kartendaten {#group-map-data}

Karten bestehen aus seiner Baum-Datenstruktur, die wiederum aus  [Knoten](#node) besteht.
Weil erwartet wird, dass jeder [Knoten](#node) ein korrespondierendes Item in der Content (Master) Datenbank besitzt, wenn Sie das Kontrollkästchen der Gruppen-Kartendaten des Karten-Selectors auswählen; werden die Knoten vom Sitecore Datatemplate, von dem aus sie erstellt wurden, gruppiert. 
Beispielsweise können Sie diese beiden Pfade

- Home -&gt; TVs -&gt; 50" Flat Screen TV
- Home -&gt; Tablets -&gt; 12" Tablet

in einen einzigen Pfad gruppieren:  

- Landing Page -&gt; Produktkategorieseite -&gt; Produktdetailseite

Das Gruppieren von Kartendaten ist nützlich, wenn Sie eine Pfadanalyse auf einer Seitenkategorieebene im Vergleich zu einer einzelnen Seitenebene durchführen wollen. 

## Date Range Selector {#date-selector}
Sie können einen Datumsbereich des Datumsbereichselektors auswählen, indem Sie entweder ein individuelles Start- und Enddatum aus den Kalendern oder indem Sie einen vordefinierten Datumsbereich auswählen.

### Daten Fehlende Daten {#date-selector-missing-dates}
Es kann vorkommen, dass eine Karte keine Daten für einige Daten hat, auch wenn es verfügbare Daten vor oder nach diesen Daten gibt. 
Möglicherweise gibt es keine aufgezeichneten Interaktionen für ein Datum oder es ist ein Fehler während der Datenverarbeitung aufgetreten und die Daten, die im Fehler vorkamen wurden übersprungen. 
Der Datumsbereich-Selektor markiert Daten, für die keine Daten verfügbar sind.  
Bitte kontaktieren Sie Ihren Systemadministrator, wenn Sie im Kalender auf viele Daten ohne Daten stoßen.

### Nicht verfügbare Daten {#date-selector-unavailable-dates}
Je nach Datumsbereich, den Sie ausgewählt haben, kann es vorkommen, dass einige Daten als nicht auswählbar markiert werden. Wenn Sie zum Beispiel ein Enddatum auswählen, werden alle Daten vor dem aktuellen Startdatum als nicht verfügbar gekennzeichnet. Alle zukünftigen Daten werden auch als nicht verfügbar gekennzeichnet.

## Metrikfilter {#metrics-filter}
Dieser Filter konzentriert sich auf das Filtern von Knoten nach ihren wichtigsten Metriken: Besuche, Wert pro Besuch und Ausstiegswertpotential.
Sie können den Metrikfilter verwenden, um Störungen zu reduzieren oder interessante Zusammenhänge zwischen verschiedenen Metriken und um Kandidaten für eine Pfadoptimierung zu finden, zum Beispiel:

- Viele [Besuche](#visits), aber niedriger [Wert](#value).
- Hoher [Wert pro Besuch](#value-per-visit), aber wenige [Besuche](#visits).
- Hohes [Ausstiegswertpotential](#exit-value-potential).

## Anwendungsnachrichten {#application-messages}
Wenn Sie die Anwendung verwenden, sehen Sie verschiedene Meldungen in der Statusleiste.

### "Einige Pfade sind verborgen. Verwenden Sie den Filter, um andere Pfade sehen zu können." {#page-analyzer-hidden-paths}
Die Anwendung zeigt nur 10 Pfade auf einmal.
Sie können den Metriken-Filter verwenden, um die Anzahl der Pfade zu reduzieren, basierend auf beliebigen Metrik-Kriterien

### "Basierend auf 500 Pfaden aus X insgesamt." {#page-analyzer-maximum-paths}
Einige Seiten, wie die Homepage, können eine enorme Menge an eindeutige Pfade aufweisen, die durch sie hindurchlaufen. 
Für eine bessere Effizienz, verarbeitet die Anwendung nur die Top 500-Pfade.
Sie können eine segmentiertere Karte auswählen oder ein geringeres Datumsintervall.  

### "Die ausgewählte Karte wird erstellt. Sie sehen u.U. nur Teildaten." {#partial-map}
Diese Meldung wird angezeigt, wenn die aktuell ausgewählte Karte zwar kurzlich bereitgestellt wurde, jedoch der  Prozess des Aufbaus von Daten für diese Karte noch nicht abgeschlossen wurde. Daten für die neu bereitgestellte Karte sollten ca. 30 Minuten nach Bereitstellung der Karte verfügbar sein.

## Glossar {#glossary}

### Karte {#map}
Eine spezielle Marketing-Definition, die beschreibt, wie man Daten für die Pfadanalyse erstellt. 
Der Page Analyzer verwendet Kartendaten und  filtert alle Pfade, um nur diejenigen anzuzeigen, die durch die aktuell ausgewählte Seite führen. Dieses gefilterte Dataset dient zur Visualisierung.
Sie können zu einer anderen Karte wechseln, indem Sie den [Karten-Selektor](#map-selector) verwenden. 

### Pfad {#path}
Eine Sequenz von [Knoten](#node) bilden einen Pfad. Alle im Page Analyzer angezeigten Pfade führen durch die aktuell ausgewählte Karte. 

### Knoten {#node}

Ein Element auf einem [Pfad](#path). Für die misten Karten gilt, dass Knoten im Wesentlichen zu einer anderen Seite führen. 
Es gibt eine Reihe von Metriken, die auf jedem Knoten gespeichert sind: [Wert](#value), [Besuche](#visits),
[Wert pro Besuch](#value-per-visit), [Ausstiege](#exits), [Ausstiegswert](#exit-value), [Ausstiegswert pro Besuch](#exit-value-per-visit) und [durchschnittlich verbrachte Zeit](#average-time-spent).

### Ausstiegsknoten {#exit-node}

Knoten mit [Ausstiegen](#exits) größer als Null zeigen die Anzahl der [Besuche](#visits), die auf diesem Knoten beendet wurden.

### Besuchsmetrik {#visits}

Die Gesamtzahl der aggregierten Besuche auf einem bestimmten Knoten. Dazu gehören Besuchsmetriken von allen Nachfahrknoten.

### Wertmetrik{#value}
Der insgesamt aggregierte Engagementwert auf einem bestimmten Knoten. Dazu gehören Wertmetriken aus allen Nachfahrknoten. 

### Wert pro Besuchsmetrik {#value-per-visit}

Der aggregierte [Engagemenwert](#value) geteilt durch [Besuche](#visits) auf einem vorgegebenen Knoten.
Manchmal ist diese Metrik definiert als **Effizienz**.
Diese Metrik ist maßgeblich bei der Berechnung des [Ausstiegswertpotentials](#exit-value-potential).

### Ausstiegsmetrik {#exits}

Die Anzahl der Ausstiege auf einem vorgegebenen Knoten.
Diese Metrik gibt an, ob ein vorgegebener Knoten einen vollständigen Pfad oder einen Einstiegspfadumfasst. 
Jeder Knoten mit Ausgängen größer als Null umfasst einen vollständigen Pfad.
Diese Metrik ist maßgeblich bei der Berechnung des [Ausstiegswertpotentials](#exit-value-potential).

### Ausstiegswertmetrik {#exit-value}

Die aggregierten Engagementwerte auf einem bestimmten Knoten vor dem Ausstieg.
Nur Knoten bei denen Ausstiege stattgefunden haben besitzen diese Metrik.
Der Unterschied hierzwischen und der [Wertmetrik](#value) besteht darin, dass die Ausstiegwertmetrik nicht den Engagementwert der Nachfolgeknoten berücksichtigt

### Ausstiegswert pro Besuchsmetrik {#exit-value-per-visit}
Der aggregierte [Engagemenwert](#value) geteilt durch die [Besuche](#visits) auf einem vorgegebenen [Ausstiegsknoten](#exit-node). Nur für Knoten, auf denen Ausstiege stattgefunden haben, wird diese Metrik berechnet. 
Der Unterschied zwischen dieser Metrik und der [Wert pro Besuch](#value-per-visit) Metrik besteht darin, dass diese Metrik nicht den Engagementwert pro Besuch der Nachfahrknoten berücksichtigt. 
Diese Metrik ist maßgeblich für die Berechnung des [Ausstiegswertpotentials](#exit-value-potential).

### Ausstiegswertpotential-Metrik {#exit-value-potential}
Das Ausstiegswertpotential zeigt einen projizierten [Engagemenwert](#value), der durchschnittlich durch Optimierung gewonnen werden könnte.  
Es wird nur für die [Ausstiegsknoten](#exit-node) berechnet.
Sie können es als eine erweiterte Bounce-Metrik betrachten, wo neben den [Ausstiegen](#exits) auch der Engagementwertverlust oder Wertverlust berücksichtigt wird. 
Wenn man weiß, wie viel [Wert pro Besuch](#value-per-visit) auf allen weiter unten liegenden Pfaden angesammelt wird, und wie viel [Wert pro Besuch](#value-per-visit) im [Ausstiegsknoten](#exit-node) gespeichert wird, dann kann diese Metrik berechnet werden, indem 
man das Delta zwischen den beiden bildet und mit der Anzahl der Ausstiege multipliziert, unter der Verwendung der folgenden Formel:


(Wert pro Besuch – Ausstiegswert pro Besuch) * Ausstiege

