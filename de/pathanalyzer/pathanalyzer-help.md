# Einf�hrung in den Path Analyzer {#intro}
Der Path Analyzer erm�glicht es Ihnen, die Pfade zu untersuchen, die Ihre Kunden benutzen, w�hrend sie mit Ihrer Marke interagieren. Er konzentriert sich darauf, die effizientesten, die am wenigsten effizienten und die Pfade, die Optimierungspotential haben, zu identifizieren.
Sie k�nnen die Pfade, die die Kunden nehmen durch besondere
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels" target="_blank">Kan�le</a> (email marketing, social, and so on) analysieren, w�hrend mit <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity" target="_blank">Kampagnen</a>,
interagiert wird bzw. auf ihrem Weg, wichtige Gesch�ftsprozesse umzuwandeln, wie z.B.
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals" target="_blank">Ziele</a>,
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events" target="_blank">Events</a> und
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">Ergebnisse</a>.


## Wichtige Szenarien {#scenarios}

### 1. Erkunden der Karte {#scenario1}
[Die wichtigsten Visualisierungssignale zu verstehen](#map-key) bzw. die Daten hinter ihnen, ist sehr wichtig, denn nur so kann man eine Karte effektiv lesen und Muster erkennen. Die unten aufgef�hrten Funktionen sind bei Ihrer Pfadanalyse n�tzlich, besonders wenn Sie die Anwendung das erste Mal benutzen und sich nicht sicher sind, wo Sie beginnen sollen.

[Das Berichte-Feature](#reports), verf�gbar �ber das Context Pane, hilft Ihnen dabei, Wege schnell in jeder Berichtkategorie zu markieren. 
Wenn Sie zum Beispiel alle Pfade sehen wollen, die keinen [Engagementwert](#value) generieren, klicken Sie einfach auf die "Pfade ohne Wert" Kategorie und durchbl�ttern dann die Top 10 Pfade.
Es gibt insgesamt [8 Reportkategorien](#reports) zum Erkunden.

[Die Dashboardansicht](#dashboard) ist n�tzlich, wenn Sie gerade erst mit der Pfadanalyse beginnen und sich noch nicht so gut mit [anderen Kartenansichten](#map-views) auskennen.
In der Dashboardansicht k�nnen Sie sich Folgendes ansehen: [Karten-KPIs](#map-kpis); [Top-Pfadeinstiege](#top-path-entries) und [Featured Path](#featured-path); und Sie k�nnen auf das [Berichte](#reports) und [Funnels](#funnels) Feature zugreifen.

[Die Tabellenansicht](#table-view) ist eine weitere gute M�glichkeit, mit der Pfadanalyse zu beginnen. Sie verwendet eine Excel-�hnliche Visualisierung, die alle Pfade und deren Metriken anzeigt und erm�glicht das Sortieren und Filtern. 

[Der Metrik-Filter](#metrics-filter), verf�gbar f�r alle Ansichten, au�er f�r das Dashboard, versetzt Sie in die Lage, sich auf Pfade zu konzentrieren, basierend auf einem bestimmten Satz von Metriken.
Sie k�nnen den Filter verwenden, um eine Karte der Pfade mit hohem [Wert](#value), aber niedriger [Besuchszahl](#visits) anzuzeigen, Pfade mit hohem [Wert pro Besuch](#value-per-visit) oder Pfade mit hohem [Ausstiegswertpotential](#exit-value-potential).
Auf diese Weise k�nnen Sie die Karte so filtern, dass gute Pfade, schlechte Pfade und Pfade mit Optimierungspotential angezeigt werden.

### 2. Erkundung von Pfaden von oder zu einer bestimmten Seite {#scenario2}

Wenn Sie den Namen einer bestimmten Seite kennen, kann der Path Analyzer ganz einfach alle Pfade anzeigen, die zu dieser Seite hin bzw. von ihr weg f�hren, indem Sie den [Pfadfilter](#path-filter) verwenden, um einen Pfad zu erstellen, der auf dem Seitennamen basiert.
Wenn Sie eine Zielseite im Sinn haben, k�nnen Sie sie im Pfadfilter inkludieren, um alle Pfade von Seite A zu Seite B zu erfassen. 
Sie k�nnen [Experience-Karten](#experience-maps) verwenden, um Pfade zu filtern, die zu einem Ziel f�hren.

�hnlich wie bei [Szenario #1](#scenario1), k�nnen Sie den [Metrik-Filter](#metrics-filter) benutzen, um eine gefilterte Karte basierend auf einer beliebigen Kombination von Metriken zu verfeinern.

Nachdem Sie den Filter angewendet haben, k�nnen Sie entweder verschiedene Ansichten erkunden, indem Sie die gefilterte Karte
[lesen](#map-key) oder das [Berichte Feature](#reports) einsetzen, um z�gig die Top 10 Pfade der 
[Berichte-Kategorie](#reports) zu durchforsten.
Die Berichte zeigen nur Pfade, die zum angewandten [Pfadfilter](#path-filter) und [Metrik-Filter](#metrics-filter) passen.

### 3. Makro-Level Pfadanalyse (Ziele, Events, Ergebnisses) {#scenario3}

Wenn Karten auf Seitenebene zu viele Details bieten, sind [Experience-Karten](#experience-maps) oft n�tzlich, um eine Pfadanalyse auf Makro-Level verstehen zu k�nnen. Dabei wird sich auf
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels" target="_blank">Kan�le</a>, <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity" target="_blank">Kampagnen</a>, <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals" target="_blank">Ziele</a>, <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events" target="_blank">Events</a> und <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">Ergebnisse </a> konzentriert.</p>

### 4. Erkundung einer Kampagne oder Channel Traffic {#scenario4}

Wenn Sie verstehen wollen, wie Ihre Kunden mit Ihrer Marke mittels einem bestimmten <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels" target="_blank">Kanal</a> interagieren oder einer <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity" target="_blank">Kampagne</a>, so k�nnen Sie eine der standardm��igen [Kanalkarten ausw�hlen ](#channel-maps) ausw�hlen, indem Sie den [Karten-Selector](#map-selector) anw�hlen oder eine neue [Kampagnekarte](#campaign-maps) [erstellen und einsetzen](#how-to-create-a-new-map), die sich auf die Kampagne, die Sie interessiert konzentriert. 

Sie k�nnen auch [Experience-Karten](#experience-maps) wie in [Szenario #3](#scenario3) verwenden und den [Pfadfilter](#path-filter) benutzen, um nur die Pfade von einem bestimmten Kanal oder einer Kampagne anzuzeigen.

### 5. Erkundung einer Karte, die sich auf ein bestimmtes Segment konzentriert {#scenario5}
Um Pfade aus einem bestimmten Kundensegment zu erkunden [erstellen Sie eine neue Karte](#how-to-create-a-new-map) und spezifizieren dann Ihre Segmentregeln im Filterfeld unter Verwendung der <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/the_rule_set_editor" target="_blank">Rule Set Editor</a> Schnittstelle.
Nachdem die neue Karte eingesetzt wurde, k�nnen Sie sie im Karten-Selector ausw�hlen und sie genauso erforschen, wie die Standardkarten.

### 6. Pfade erkunden, die zu einem Ziel f�hren {#scenario6}
Eine M�glichkeit Pfade, die zu einem Ziel f�hren zu erkunden, liegt darin, die standardm��ige
[Experience-Karte mit Zielen](#experience-maps) zu benutzen und das Ziel im 
in [Pfadfilter](#path-filter) zu spezifizieren.

Eine weitere M�glichkeit besteht darin, eine neue [Zielkarte](#goal-maps) zu [erstellen und einzusetzen](#how-to-create-a-new-map), die sich nur auf die Pfade zum angegebenen Ziel konzentriert.
Die gleiche Technik k�nnen Sie verwenden, um Pfade zu bestimmten Assets oder Ergebnissen zu erforschen.

## Karten {#maps}
Eine Karte ist eine spezielle Marketing-Definition f�r Pfadanalysen, die zwei wichtige Attribute hat: Kartentyp und Karte-Filter. Der Kartentyp beschreibt, wie man Daten erstellt, die die Karte versorgen. Dies wird [hier](#map-types) noch ausf�hrlicher beschrieben. Der Kartenfilter, ein optionales, jedoch wichtiges Attribut, hilft dabei, eine segmentierte Karte zu definieren, indem der <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/the_rule_set_editor" target="_blank">Rule Set Editor </a> verwendet wird, sowie eine umfangreiche Reihe von Bedingungen.

Neben diesen beiden wichtigen Attributen hat jede Karte eine eindeutige Kennung, Namen und Typ. Sie k�nnen auch weitere optionale Attribute, wie z. B. Beschreibung, inkludieren.

�hnlich wie bei anderen Marketing Definitionselementen, [erstellen Sie eine Karte in der Marketing Control Panel](#how-to-create-a-new-map).

Karten werden unter der Verwendung der [Kartenansicht](#map-views) visualisiert.

## Kartentypen {#map-types}
Der Kartentyp schreibt vor, wie die Interaktionsdaten von xDB f�r die Pfadanalyse umgewandelt werden.  Standardm��ig gibt es verschiedene Kartentypen.

### Seitenkarten {#page-maps}
Diese Karten werden aus einer Sequenzen der Seitenbesuche innerhalb einer bestimmten Interaktion aufgebaut. Standardm��ig stehen einige Untertypen f�r Seitenkarten zur Verf�gung. 
Diese Kartenuntertypen sind praktisch, da sie es Ihnen erm�glichen, eine Seitenkarte schnell zu erstellen, die sich auf ein bestimmtes Interaktionsattribut (Kanal, Kampagne, Ziel, Asset, usw.) konzentriert.

#### Zielkarten {#goal-maps}
Zielkarten erm�glichen es Ihnen, eine Seitenkarte zu erstellen, die zu einem bestimmten Ziel f�hrt. Zielkarten vernachl�ssigen Seiten, die besucht wurden, nachdem ein bestimmtes Ziel erreicht wurde.

Sie k�nnen Zielkarten im Reverse-Modus erstellen, indem Sie Sie die Reverse Checkbox im Zielkartendefinitionsitem im Marketing Control Panel ausw�hlen.
Eine Reverse-Zielkarte dreht die Sequenz von Seiten um, die zu einem bestimmten Ziel f�hren und verwendet das ausgew�hlte Ziel als Ausgangspunkt der Karte anstatt des herk�mmlichen
[Internetknotens ](#internet-node).

#### Asset-Karten {#asset-maps}
Asset-Karten erm�glichen es Ihnen eine Seitenkarte zu erstellen, die zu einem bestimmten Asset-Download f�hrt.  
Asset-Karten vernachl�ssigen Seiten, die besucht wurden, nachdem ein bestimmtes Asset heruntergeladen wurde.

Sie k�nnen Asset-Karten im Reverse-Modus erstellen, indem Sie die Reverse Checkbox im Assetkartendefinitionsitem in der Marketing Control Panel ausw�hlen.
Eine Reverse-Asset-Karte dreht die Sequenz von Seiten um, die zu einem bestimmten Assetdownload f�hren und verwendet das ausgew�hlte Asset als Ausgangspunkt der Karte anstatt des herk�mmlichen [Internetknotens](#internet-node).

#### Kampagnekarten {#campaign-maps}
Kampagnekarten erm�glichen es Ihnen, eine Seitenkarte f�r alle Interaktionen einer bestimmten Kampagne zu erstellen.

#### Kanalkarten {#channel-maps}
Kanalkarten versetzen Sie in die Lage, eine Seitenkarte f�r alle Interaktionen aus einem bestimmten Kanal zu erstellen.

#### Ergebniskarten {#outcome-maps}
Ergebniskarten versetzen Sie in die Lage, eine Seitenkarte zu erstellen, die zu einem bestimmten Ergebnis f�hrt.

### Experience-Karten {#experience-maps}
Anders als Seitenkarten k�nnen Experience-Karten andere Interaktionsattribute enthalten, wie z.B. 
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels" target="_blank">Kan�le</a>,
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity" target="_blank">Kampagnen</a>,
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals" target="_blank">Ziele</a>,
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events" target="_blank">Events</a> und
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">Ergebnisse</a>,
zuz�glich zu den Seiten.

Sie w�hlen diese Interaktionsattribute mithilfe der Kontrollk�stchen-Optionen im Experience-Kartendefinitionsitem im Marketing Control Panel.
Auf diese Weise versetzen Experience-Karten Sie in die Lage, sich auf mehr umfassende Pfadanalysen zu konzentrieren als die detaillierteren [Seitenkarten ](#page-maps) es zulassen.

Standardm��ig stehen drei Experience-Karten zur Verf�gung:

- Experience-Karte mit Zielen. Umfasst Kan�le, Kampagnen (falls verf�gbar), alle Ziele und Ergebnisse.
- Experience-Karte nur mit Value-Zielen. Genau wie oben, nur dass hier lediglich Ziele mit Engagementwert hinzugef�gt werden.
- Experience-Karte mit Seitenevents. Umfasst Kan�le, Kampagnen (falls verf�gbar), nur Einstiegs- und Ausstiegsseiten, alle Seitenevents und Ergebnisse.


Sie k�nnen mit dem Marketing Control Panel ganz einfach [eine neue Karte erstellen](#how-to-create-a-new-map), basierend auf jeder vorhandenen Karte.

### Seitenspezifische Karten {#site-specific-maps}
Neben den Kartentypen k�nnen Karten entweder �global oder �seitenspezifisch� sein. Globale Karten werden f�r alle Seiten erstellt, w�hrend seitenspezifische Karten nur f�r eine bestimmte Seite erstellt werden. Ob eine Karte global oder seitenspezifisch ist, h�ngt vom Ort der Karte innerhalt des Content Trees des Path Analyzers im Marketing Control Panel ab. Alle globale Karten befinden sich im */Maps/Default maps/Global maps* Ordner und alle seitenspezifischen Karten im
*/Maps/Default maps/Site maps* Ordner.

### Benutzerdefinierte Karten {#custom-maps}
Wenn benutzerdefinierte Karten registriert sind, was normalerweise nur einen geringen Entwicklungsaufwand erfordert, finden Sie sie im */Maps/Custom maps* Ordner.

### Wie erstelle ich eine neue Karte {#how-to-create-a-new-map}

Um eine neue Karte zu erstellen:

1. �ffnen Sie das Marketing Control Panel vom Launchpad.
2. Navigieren Sie zum Path Analyzer Item.
3. Erweitern Sie das Kartenitem unter Path Analyzer.
4.  W�hlen Sie den entsprechenden Ordner f�r Ihre neue Kartebasierend auf den oben beschriebenen verf�gbaren Kartentypen.
5. Erstellen Sie ein neues Kartenelement.
6. Geben Sie die erforderlichen Attribute und optionale Attribute f�r Ihre Karte an
7. Speichern Sie das Kartenelement.
8. Setzen Sie die neue Karte unter Verwendung des Deploy Workflow Befehls in der Registrierkarte Review ein.

Vergangene bzw. Live-Daten f�r die Karte erscheinen etwa 30 Minuten nach der Bereitstellung.

## Karten-Selector {#map-selector}
Mit Hilfe der Karten-Selektor-Steuerung k�nnen Sie verschiedene Karten ausw�hlen.
Sie k�nnen auch weitere Karten-Meta-Daten  ansehen und eine Karte zu Ihrer Favoritenliste hinzuf�gen, die automatisch in Ihrem Profil gespeichert wird.

### Gruppen-Kartendaten {#group-map-data}
Karten werden mit [Baumdatenstrukturen](#tree), die aus [Knoten](#node) bestehen, betrieben.
Weil erwartet wird, dass jeder [Knoten](#node) ein entsprechendes Item in der Content (Master) Datenbank hat, zumindest wenn Sie das Daten- Kontrollk�stchen f�r die Gruppenkarte im Karten-Selektor ausw�hlen, werden die Knoten vom Sitecore Datentemplate, von dem aus sie auch erstellt wurden, in Gruppen eingeteilt.
Zum Beispiel k�nnen Sie diese zwei Pfade:

- Home -&gt; TVs -&gt; 50" Flat Screen TV

- Home -&gt; Tablets -&gt; 12" Tablet

in einen einzigen Pfad  gruppieren:
- Landing Page -&gt; Produktkategorie-Seite -&gt; Produktdetail-Seite

Gruppenkartendaten sind n�tzlich, wenn Sie eine Pfadanalyse auf Seitenkategorielevel durchf�hren wollen im Vergleich zu einem individuellen Seitenlevel.
## Datenbereich-Selektor {#date-selector}
Sie k�nnen einem Datumsbereich mithilfe des Datumsbereich-Selektors festlegen, indem Sie entweder ein individuelles Start- und Enddatum aus den Kalendern w�hren oder indem Sie einen vordefinierten Datumsbereiche ausw�hlen.

### Daten Fehlende Daten{#date-selector-missing-dates}
Es kann vorkommen, dass eine Karte keine Daten f�r einige Daten hat, auch wenn es verf�gbare Daten vor oder nach diesen Daten gibt. 
M�glicherweise gibt es keine aufgezeichneten Interaktionen f�r ein Datum oder es ist ein Fehler w�hrend der Datenverarbeitung aufgetreten und die Daten, die im Fehler vorkamen wurden �bersprungen. Der Datumsbereich-Selektor markiert Daten, f�r die keine Daten verf�gbar sind.  
Bitte kontaktieren Sie Ihren Systemadministrator, wenn Sie im Kalender auf viele Daten ohne Daten sto�en.

### Nicht verf�gbare Daten{#date-selector-unavailable-dates}
Je nach Datumsbereich, den Sie ausgew�hlt haben, kann es vorkommen, dass einige Daten als nicht ausw�hlbar markiert werden. Wenn Sie zum Beispiel ein Enddatum ausw�hlen, werden alle Daten vor dem aktuellen Startdatum als nicht verf�gbar gekennzeichnet. Alle zuk�nftigen Daten werden auch als nicht verf�gbar gekennzeichnet.

## Kartenschl�ssel{#map-key}
Der folgende Kartenschl�ssel gilt f�r radiale, horizontale und vertikale Strukturansichten.

Wenn Sie eine Karte lesen, repr�sentieren die Gr��e und Farbe der Kreise und Linien zwischen den Knoten auf der Karte Informationen dar�ber, welche Pfade einen h�heren [Engagementwert](#value) oder einen
h�heren [Wert pro Besuch](#value-per-visit) bieten oder die am h�ufigsten [besuchten](#visits). 

Kreise repr�sentieren [Knoten](#node). Je nach ausgew�hltem Kartentyp, k�nnen Knoten Seiten, Ziele oder andere Marketingaktivit�ten repr�sentieren. Kreise haben die folgenden zwei visuellen Eigenschaften, die Informationen �ber den Knoten liefern: Gr��e und Farbe.

Die Gr��e eines Kreises zeigt die Gesamtzahl des [Engagementwerts](#value) eines [Knotens](#node) und aller seiner Nachfahren.
Mit anderen Worten, stellt ein gr��eren Knoten einen gr��eren Gesamtwert des [Engagementwertes](#value) dar.

Die Farbe eines Kreises zeigt den [Wert pro Besuch](#value-per-visit) eines [Knotens](#node) im Vergleich zum Wert pro Besuch seiner Eltern und hilft Ihnen, die �nderung in dieser Metrik zu erkennen, wenn Sie den Pfad weiter unten betrachten. Wenn ein Kreis rot wird, dann hat der [Wert pro Besuch](#value-per-visit) bei diesem [Knoten](#node) abgenommen.
Wird ein Kreis gr�ner als seine Eltern wird, dann hat der [Wert pro Besuch](#value-per-visit) bei diesem [Knoten](#node) zugenommen.
Die Kreisfarbe hilft Ihnen auch dabei die [Wert pro Besuch](#value-per-visit) Metrik zwischen Geschwisterknoten zu vergleichen und zu bestimmen, wo der Pfad f�r den h�chsten
[Wert pro Besuch](#value-per-visit) von einem bestimmten [Knoten](#node) aus fortgef�hrt wird.

Kreise mit einem dicken dunkelgrauen Rahmen stehen f�r besondere "[andere Knoten](#other-nodes)".

Linien, die die Kartenknoten verbinden, stellen Pfade zwischen [Knoten](#node) A und [Knoten](#node) B dar. Linien haben die folgenden visuellen Eigenschaften und bieten Informationen �ber den [Pfad](#path): Dicke und teilweise Schattierung.

Die St�rke einer Linie zeigt an, wie viele [Besuche](#visits) (Traffic) von [Knoten](#node) A nach [Knoten](#node) B im Vergleich zu den Geschwistern des [Knotens](#node) B geflossen ist, was zu einer einfacheren Identifizierung von High-Traffic-Pfade f�hrt.

Eine partielle Schattierung einer Zeile erg�nzt Linienst�rke und wird verwendet, um Pfadbesuche in einer tieferen Schicht zu zeigen, es schwieriger ist, Unterschiede in der Liniendicke zu sehen.

Im Allgemeinen sollten Sie nach dicken Linien mit entweder kleinen oder roten Kreisen suchen, die ein hohes Volumen von [Besuchen](#visits) eines Pfades anzeigen zu Pfaden, die einen niedrigen [Engagementwert](#value) (Gr��e) und wenig [Wert pro Besuch](#value-per-visit) (Farbe) aufweisen.

### Andere Knotens {#other-nodes}
Aufgrund der Einschr�nkungen der Strukturansichten (radial, horizontal und vertikal) beim Visualisieren gro�er Karten mit extremen Fanouts, k�nnen weniger bedeutende Knoten, die auf einer bestimmten Ebene der Visualisierung nicht passen, in einem speziellen �anderen� Knoten kombiniert werden. Die [Tabellenansicht](#table-view) hat diese Einschr�nkung nicht.

Sie k�nnen die Liste der Knoten, die in �Andere Knoten� kombiniert wurden, ansehen, indem Sie  den Weiter Tab im Control Pane ausw�hlen oder den Tab Andere im Knoten Popover.

Das Anwenden eines [Pfadfilters](#path-filter) oder eines [Metrikfilters](#metrics-filter) hilft normalerweise dabei, die Anzahl der auf einer Karte angezeigten �Anderen Knoten� zu verringern.

## Kartenansicht {#map-views}
Es gibt f�nf verschiedene Ansichten aus denen Sie zur Analyse Ihrer Karten w�hlen k�nnen. Dashboard ist die standardm��ige Ansicht, die Ihnen einf�hrende Einblicke zur Pfadanalyse bietet und [unten](#dashboard) beschrieben wird.

### Radiale Ansicht {#radial-view}
Bei der radialen Ansicht liegt der Vorteil darin, dass mehr Kartendaten auf den Bildschirm passen,  jedoch ist sie nicht ideal f�r kleinere oder gefilterte Karten.
Der [Internetknoten](#internet-node) steht im Mittelpunkt dieser Ansicht.

### Vertikale Ansicht {#vertical-view}
Die vertikale Ansicht ist viel besser geeignet zur Darstellung von kleineren Karten oder gefilterten Karten und bietet in der Regel bessere Lesbarkeit im Vergleich zur [radialen Ansicht](#radial-view). Der [Internetknoten](#internet-node) befindet sich ganz oben in dieser Ansicht.

### Horizontale Ansicht {#horizontal-view}
�hnlich wie bei der vertikalen Ansicht ist die horizontalen Ansicht ist gut f�r kleinere Karten geeignet und bietet in der Regel bessere Lesbarkeit im Vergleich zur [radialen Ansicht](#radial-view).
Der [Internetknoten](#internet-node) befindet sich auf der linken Seite.

### Tabellenansicht {#table-view}
Die Tabellenansicht ist anders, weil sie nur [vollst�ndige Pfade](#path) zeigt, was daran liegt, dass die Kartendaten sich in einer [Baumstruktur ](#tree) befinden, die  nicht einfach als Tabelle angesehen werden k�nnen.

## Dashboard {#dashboard}
Dashboard ist eine spezielle Ansicht, die einf�hrende Einblicke zur Pfadanalyse bietet.

### Karten-KPIs {#map-kpis}
Im Dashboard stehen standardm��ig sechs Key Performance Indicators (KPI) f�r die folgenden Metriken zur Verf�gung: [Besuche](#visits), [Wert](#value), [Wert pro Besuch](#value-per-visit) und optionale Ergebnismetriken: [Geldwert](#monetary-value), [Ergebnisse](#outcomes) und [durchschnittlicher Geldwert](#average-monetary-value).

Ergebnismetriken werden nicht standardm��ig angezeigt und k�nnen unter [Anwendungseinstellungen](#application-settings) aktiviert werden.

Jede Karten-KPI hat einen Trend-Indikator, der die Erh�hung oder Verringerung einer Metrik im Vergleich mit der gleichen Metrik �ber das gleiche Datumsintervall f�r die gleiche Karte in der Vergangenheit zeigt. Wenn z.B. der aktuell ausgew�hlte Datumsbereich heute ist, basiert das Trendbarometer auf den Daten von gestern.

### Top Pfadeinstiege{#top-path-entries}
Diese Liste zeigt die Top-10-Pfad Ansatzpunkte auf der aktuellen Karte. In der Pfad-Analyzer-Terminologie sind dies die Top [Knoten](#node) auf der ersten Ebene, sortiert basierend auf einer Kombination aus [Wert-](#value) und [Besuchs-](#visits) Metriken.

### Empfohlene Pfad {#featured-path}
Der empfohlene Pfad zeigt den Pfad von der aktuell ausgew�hlten Karte mit den interessantesten und wichtigsten Marketing-Kennzahlen. Die Auswahl des empfohlenen Pfades basiert auf einem Algorithmus, der entweder das [Ausstiegswertpotential](#exit-value-potential) ber�cksichtigt oder den [Wert](#value) und [Besuche](#visits) kombiniert und dann den Top Pfad in der Metrikkategorie w�hlt.
Da die M�glichkeit zur Optimierung f�r kurze Pfade relative eingeschr�nkt ist,  priorisiert der Algorithmus die l�ngsten Wege.

### Favorite Funnel {#favorite-funnel}
Ein Favorite Funnel ist ein Funnel, der als Favoriten auf einer bestimmten Karte markiert wurde. Dies kann jederzeit im Context Pane unter Funnels ge�ndert werden. Ein Favorite Funnel wird in Ihrem Benutzerprofil gespeichert und wird mit der Karte von der aus er als Favorit gekennzeichnet wurde assoziiert.

## Berichte {#reports}
Die Path Analyzer Berichte zeigen Top-Pfade in verschiedenen Kategorien.
Berichte bieten eine Einf�hrung in die interessantesten Pfade in der aktuell ausgew�hlten Karte und versetzen Sie in die Lage, schlechte und gute Pfade schnell identifizieren zu k�nnen.
Standardm��ig stehen acht Berichtskategorien zur Verf�gung. Bis zu 10 Pfade stehen zur Auswahl in jeder Kategorie zur Verf�gung.

### Am meisten besucht {#highest-visited-report}
Die Pfade mit den meisten [Besuchen](#visits).

### H�chster Wert {#highest-valuable-report}
Die Pfade, die dem h�chsten [Engagementwert](#value).

### Die meisten Besuche und der h�chste Wert {#highest-visitsvalue-report}
Die Pfade, die den h�chsten [Engagementwert](#value) und die meisten [Besuche](#visits) generieren.

### H�chster Wert pro Besuch {#highest-valuepervisit-report}
Die Pfade, die den h�chsten [Wert pro Besuch](#value-per-visit) generieren.

### Pfade ohne Wert {#paths-without-value-report}
Die Pfade, die Kunde verlassen haben, ohne einen [Engagementwert](#value) zu generieren.

### H�chstes Ausstiegswertpotential {#highest-evp-report}
Die Pfade, die das h�chste [Ausstiegswertpotential](#exit-value-potential) generieren.

### H�chste Ergebnisse {#highest-outcomes-report}
Die Pfade, die die meisten [Ergebnisse](#outcomes) generieren.

### H�chster Geldwert {#highest-monetaryvalue-report}
Die Pfade, die den h�chsten [Geldwert](#monetary-value) insgesamt generieren und aus Ergebnissen kommen.

## Funnels {#funnels}

Ein Funnel ist eine klar definierte Abfolge von Schritten, von denen erwartet wird, dass Kunden sie auf dem Weg zur Verwirklichung eines Gesch�ftsziels nehmen. Unternehmen definieren ihre eigenen Funnel. F�r eine e-Commerce-Website ist es wahrscheinlich ein Checkout
Funnel, der als Abfolge von Seiten, Seitenevents oder Zielen, je nach den Besonderheiten der Umsetzung, dargestellt werden k�nnte.

Funnels im Path Analyzer versetzen Sie in die Lage, die Aktionen und Pfade, die Kunden auf ihrem Weg zum Erreichen ihrer Ziele und Ergebnisse nehmen, zu analysieren. Sie k�nnen dann die Pfade optimieren, um die Konversionsraten zu verbessern, zum Beispiel indem <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/personalization" target="_blank">Personalisierung</a>,
<a href="https://doc.sitecore.net/sitecore_experience_platform/analyzing__reporting/experience_optimization__content_testing/ab_and_multivariate_testing" target="_blank">M/V Testing</a>,
oder <a href="https://doc.sitecore.net/sitecore_experience_platform/analyzing__reporting/experience_optimization__content_testing" target="_blank">einen Inhaltstest </a> implementieren.

Die Funnel Funktion ist �ber das Context Pane erreichbar, wo Sie einen Funnel ausw�hlen und erkunden k�nnen, der im Marketing Control Panel definiert ist.

Nachdem Sie ein Funnel ausgew�hlt haben, sehen Sie eine grafische Darstellung der nachverfolgten Schritte eines Funnels im Path Analyzer in Form eines Balkendiagramms. Das Balkendiagramm bietet Ihnen Informationen �ber die Anzahl der Kunden, die im Funnel die einzelnen Schritte vollst�ndig durchlaufen, und kl�rt Sie dar�ber auf, wie viele Kunden zum n�chsten Stadium weitergehen. Au�erdem k�nnen Sie zwischen den wichtigen Metriken, wie [Besuche](#visits), [Wert](#value) und [Wert pro Besuch](#value-per-visit). hin und her wechseln.
Unterhalb des Diagramms wird die Liste der anderen Metriken angezeigt, die die wichtigsten Leistungsindikatoren f�r den Funnel anzeigen. Diese Metriken werden dem letzten Schritt des Funnels entnommen. Diese Daten werden basierend auf dem Geltungsbereich einer Interaktion berechnet im Gegensatz zur Lifetime Kundenreise.

Jeder Funnel kann als Favorit markiert werden, indem Sie auf das Stern-Symbol neben dem Funnelnamen klicken. Dadurch Machen Sie den Funnel in der [Dashboardansicht](#dashboard). 

Um neue ausgew�hlten Pfad als Funnel zu speichern, klicken Sie auf Als Funnel speichern im Fu�zeilenbereich des Context Panes.

## Kartenfilter {#map-filters}
Es gibt zwei Arten von Filtern, die Sie in die Lage versetzen, sich auf bestimmte Pfade zu konzentrieren.

### Pfadfilter {#path-filter}
Pfadfilter erm�glichen es Ihnen, eine Karte basierend auf dem Namen eines Knotens, der entweder eine Seite, ein Ziel oder ein anderes Marketingattribut sein kann, je nach Typ der aktuellen Karte, zu filtern.
Z.B. k�nnen Sie den Pfadfilter verwenden, um zu erfahren, wie Kunden auf eine f�r sie interessante Seite gelangen.
Legen Sie einfach eine bestimmte Seite als Element des Pfadfilters fest und klicken auf Anwenden.  
Die Karte wird entsprechend angepasst.

Der Pfadfilter erm�glicht es Ihnen, einen Kartenfilter  von Seite A nach Seite B zu erstellen. In der Regel ben�tigen Sie nicht mehr als drei Elemente im Pfadfilter, Sie k�nnen dort jedoch beliebig viele Elemente festlegen. 
Der Pfadfilter grenzt die Liste der Optionen ein, basierend auf den in der aktuellen Karte verf�gbaren Daten.

### Metrikfilter {#metrics-filter}
Dieser Filter konzentriert sich auf das Filtern von Knoten nach ihren wichtigsten Metriken: [Besuche](#visits), [Wert](#value), [Wert
Pro Besuch](#value-per-visit) und [Ausstiegswertpotential](#exit-value-potential).

Wegen seiner untergeordneten Natur im Verh�ltnis zum [Pfadfilter](#path-filter), kann der Metrikfilter zeigen, wie viele �bereinstimmungen es f�r den aktuellen 
[Pfadfilter](#path-filter) gibt sowie die Korrelation zwischen verschiedenen Metriken.
Sie k�nnen den Metrikfilter auch ohne den [Pfadfilter](#path-filter) benutzen und die weniger benutzten Knoten herausfiltern, was zu einer Reduzierung von St�rungen auf der aktuellen Karte f�hrt.  

Schlie�lich k�nnen Sie mit dem Metrikfilter auch interessante Zusammenh�nge zwischen verschiedenen Metriken finden und daf�r, Kandidaten f�r eine Pfadoptimierung herauszufinden, zum Beispiel: 

- Viele [Besuche](#visits), aber niedriger [Wert](#value).

- Hoher [Wert pro Besuch](#value-per-visit), aber wenige [Besuche](#visits).

- Hohes [Ausstiegswertpotential](#exit-value-potential).

## Eine Karte exportieren {#export-map}

Sie k�nnen Daten f�r jede Karte als durch Kommas getrenntes Dataset mithilfe der folgenden beiden Befehle aus dem Men� Aktion" exportieren

- Als CSV runterladen

- Ins Clipboard kopieren

Beide Befehle arbeiten mit dem gleichen Format und existieren, um verschiedene Export-Workflows zu erm�glichen. 

## Anwendungsnachrichten {#application-messages}

Wenn Sie die Anwendung verwenden, sehen Sie verschiedene Meldungen in der Statusleiste.

### "Die Tabellenansicht zeigt die Top X-Pfade aus Y insgesamt." {#table-top}
Diese Nachricht wird angezeigt, wenn die [Tabellenansicht](#table-view) eine extrem gro�e Karten rendert. 
Die [Tabellenansicht](#table-view) kann nur die Top 500 [vollst�ndigen
Pfade](#path) zeigen. Empfohlene Ma�nahmen f�r diese Nachricht sind: verwenden Sie entweder den
[Pfadfilter](#path-filter) oder den [Metrikfilter](#metrics-filter), um die Anzahl der sichtbaren Zeilen zu verringern;
Verringern Sie das Datenbereichsintervall  f�r die Karte; oder [erstellen](#how-to-create-a-new-map) oder [w�hlen](#map-selector) Sie eine gefilterte Karte, die �ber weniger Daten verf�gt.

### "X weniger bedeutende Knoten wurden zusammen mit anderen Knoten gruppiert." {#other-nodes-message}
Diese Meldung kann mit der radialen, horizontalen oder vertikalen Ansicht auf gro�en Karten mit extremen Fanouts angezeigt werden. Um sicherzustellen, dass die Karte gut lesbar ist, k�nnen 
weniger bedeutende Knoten, die nicht auf einer bestimmten Ebene der Visualisierung passen in einem �anderen� Knoten kombiniert werden. Beachten Sie, dass die [Tabellenansicht](#table-view) dieser Einschr�nkung nicht unterliegt. Empfohlene Ma�nahmen f�r diese Nachricht sind: verwenden Sie entweder den [Pfadfilter](#path-filter) oder den [Metrikenfilter](#metrics-filter), um die Anzahl der sichtbaren Knoten zu verringern; verringern Sie die Reichweite des Datenintervalls f�r die Karte; der [erstellen](#how-to-create-a-new-map) oder [w�hlen](#map-selector) Sie eine gefilterte Karte, die �ber weniger Daten verf�gt.

### "Die ausgew�hlte Karte wird erstellt. Sie k�nnen Teildaten sehen." {#partial-map}
Diese Meldung kann angezeigt werden, wenn die aktuell ausgew�hlte Karte erst k�rzlich bereitgestellt wurde, aber der Prozess zur Erstellung der Daten noch nicht vollst�ndig ist.
Daten f�r die neu bereitgestellte Karte sollten ca. 30 Minuten nach Bereitstellung der Karte verf�gbar sein.

## Anwendungseinstellungen {#application-settings}

Es folgt eine Liste der Anwendungseinstellungen, die Sie �ndern k�nnen, um Ihr Path Analyzer- Erlebnis abzupassen:
:

- Deaktivieren/Aktivieren von �bergangseffekten

- Label standardm��ig Anzeigen/Verbergen 

- Legende standardm��ig Anzeigen/Verbergen

- Ergebnismetriken Anzeigen/Verbergen

- Tipps beim Start Anzeigen/Verbergen

- Auswahl von Daten fehlende Daten zulassen 

Diese Einstellungen sind im Men� Aktion unter Einstellungen verf�gbar.
## Glossar {#glossary}

### Karte {#map}

Eine spezielle Marketing-Definition, die beschreibt, wie man Daten f�r die Pfadanalyse erstellt. Jede bereitgestellte Karte hat einen [Baum](#tree), der in der Berichtsdatenbank gespeichert ist.

### Baum {#tree}

Die aggregierte Datenstruktur f�r die Pfadanalyse ist in einer Berichtsdatenbank f�r jede bereitgestellte Karte gespeichert und bestehend aus Hierarchie [Knoten](#node).
Jeder Baum muss einen speziellen Root-Knoten, der als [Internetknoten ](#internet-node) bezeichnet wird.

### Knoten {#node}

Der zentraler Teil des [Baums](#tree).
Alle Knoten au�er der [Internetknoten](#internet-node) besitzen einen Parentknoten und haben und k�nnen Childknoten haben. 
Je nach Karte [Kartentyp](#map-types) kann ein Knoten entweder eine Seite (auf einer [Seitenkarte](#page-maps)), 
ein Ziel oder ein anderes Marketingattribut (Kanal, Kampagne, usw.) auf einer [Experiencekarte](#experience-maps) repr�sentieren.

Jeder Knoten hat eine eindeutige numerische ID, einen Namen und eine GUID, die einem Element aus der Inhaltsdatenbank entspricht.

Es gibt verschiedene Arten von Metriken, die auf jedem Knoten gespeichert sind: 

- **Aggregierte Metriken**, einschlie�lich [Wert](#value), [Besuche](#visits), [durchschnittlich verbrachte Zeit](#average-time-spent), [Ergebnisse](#outcomes) und [Geldwert](#monetary-value).
Diese Metriken enthalten Werte aus allen nachfolgenden Knoten.

- **Ausstiegsmetriken**, einschlie�lich [Ausstiege](#exits) und [Ausstiegswert](#exit-value).
Diese Metriken beinhalten keine Werte aus allen nachfolgenden Knoten und werden nur berechnet, wenn der aktuelle Knoten ist ein [Ausstiegsknoten](#exit-node) ist.

- **Berechnete Metriken**, einschlie�lich [Wert pro Besuch](#value-per-visit), [Ausstiegswert pro Besuch](#exit-value-per-visit), [durchschnittlicher Geldwert](#average-monetary-value) und [Ausstiegswertpotential](#exit-value-potential).

### Ausstiegsknoten {#exit-node}

Knoten mit [Ausstiegen](#exits) gr��er als Null zeigen die Anzahl der [Besuche](#visits), die auf diesem Knoten beendet wurden.

### Internetknoten {#internet-node}

Ein spezieller [Rootknoten](#node),  Das dient als ein Startknoten f�r alle der als Startknoten f�r alle [Pfade](#path) dient und alle wichtigen Metriken von allen Pfaden auf einer vorgegebenen [Karte](#map) sammelt.

### Pfad {#path}

Eine Sequenz von [Knoten](#node) bildet einen Pfad. Aufgrund der aggregierten Natur des
[Baums](#tree) ist es wichtig, zwischen zwei Arten von Pgaden zu unterscheiden:
**Einstiegspfad** und **Vollst�ndiger Pfad**.

A **Ein vollst�ndiger Pfad** besteht aus einem ganzen Besuch, vom Einstiegsknoten bis zum [Ausstiegsknoten](#exit-node).
An **EIn einstiegspfad** muss jedoch nicht mit dem Ausstieg enden.
Es ist wichtig, den Unterschied zwischen den beiden Arten von Pfaden zu verstehen, 
Weil die [Tabellenansicht](#map-views) und das [Berichte-Feature](#reports) nur mit vollst�ndigen Pfaden funktioniert.

### Besuchsmetrik {#visits}

Die Gesamtzahl der aggregierten Besuche auf einem bestimmten Knoten. Dazu geh�ren Besuchsmetriken von allen Nachfahrknoten.

### Wertmetriken {#value}
Der insgesamt aggregierte Engagementwert auf einem bestimmten Knoten. Dazu geh�ren Wertmetriken aus allen Nachfahrknoten. 

### Wert pro Besuchsmetrik {#value-per-visit}

Der aggregierte [Engagemenwert](#value) geteilt durch [Besuche](#visits) auf einem vorgegebenen Knoten.
Manchmal ist diese Metrik definiert als **Effizienz**.
Diese Metrik ist ma�geblich bei der Berechnung des [Ausstiegswertpotentials](#exit-value-potential).

### Ausstiegsmetrik{#exits}

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

### Ergebnismetrik {#outcomes}

Die Gesamtanzahl von auf einem vorgegebenen Knoten realisierten Ergebnissen. Dazu geh�ren Ergebnisse aller Nachfahrknoten.
Erfahren Sie mehr �ber die Ergebnisse <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">hier</a> mehr �ber die Ergebnisse.

### Geldwert-Metrik {#monetary-value}

Die Gesamtsumme des Geldwerts, der auf einem vorgegebenen [Knoten](#node) gewonnen wurde. Der Geldwert wird aus den realisierten Ergebnissen abgerufen. Dazu geh�ret der Geldwert aus allen Nachfahrknoten.
Erfahren Sie <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">hier</a> mehr �ber Ergebnisse.

### Durchschnittlicher Geldwert-Metrik {#average-monetary-value}

Der durchschnittlich pro Ergebnis auf einem vorgegebenen [Knoten](#node) gewonnene Geldwert. Der Geldwert wird aus realisierten Ergebnissen abgerufen. 
Dies umfasst den durchschnittlichen Geldwert  aller Nachfahrknoten. 
Erfahren Sie <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">hier</a> mehr �ber Ergebnisse.

### Durchschnittlich verbrachte Metrik {#average-time-spent}

Die durchschnittliche Zeit, die Kunden bei einem vorgebebenen [Knoten](#node) in Sekunden verbringen.



