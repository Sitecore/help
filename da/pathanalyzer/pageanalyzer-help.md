# Sådan kommer du i gang med Page Analyzer {#intro}

Mens hovedapplikation Path Analyzer, der er tilgængelig via Startområde, har fokus på avanceret sti-analyse,
fokuserer Page Analyzer kun på de stier, der fører til og fra en bestemt side. Hovedmålet for applikationen er at forstå, hvordan kunder kommer til en bestemt destination (en side), og hvad de derefter gør. Datavisualiserigsindikatorer hjælper dig med at forstå stierne med mest trafik(besøg) og største engagement-værdi pr. besøg, så du kan udpege gode og dårlige stier. Du kan dykke ned i en bestemt sti og undersøge stidetaljerne.

## Sådan aflæses visualisering {#map-key}

Visualisering placerer den aktuelt valgte side i midten (vist som en stor cirkel med sideikon) og viser alle stier, der fører ind og ud af den.

Startområdet viser, hvor mange stier, der startede med den aktuelt valgte side.

Udgangsområdet viser antallet af udgange på den aktuelt valgte side og det samlede [udgangsværdipotentiale](#exit-value-potential)

De vandrette linjer, der går ind *i* den aktuelt valgte side, repræsenterer indgående stier. Cirklerne, der er placeret øverst på linjerne, repræsenterer [noder](#node) på stien. Noder oversættes generelt til sider.

De vandrette linjer, der går *fra* den aktuelt valgte side til højre, repræsenterer udgående stier. Cirklerne, der er placeret øverst på linjerne, repræsenterer [nodes](#node) på stien. Noder oversættes generelt til sider. For at forenkle visualisering, er det kun den første side, der er vist på udgående stier.

Linjetykkelsen definerer det samlede antal [besøg](#value-per-visit) på den aktuelt valgte side fra den specifikke sti. 
Jo tykkere stien er, jo flere besøg kommer der til den side for en given sti.

Linjefarven definerer [værdi pr. besøg](#value-per-visit) på denne specifikke sti til den aktuelt valgte side. 
Jo grønnere stien er, jo højere [værdi pr. besøg](#value-per-visit) sammenlignet med andre stier, der fører til den aktuelt valgte side.
Stier med mindste værdi pr. besøg er vist med rødt.

Størrelsen af cirklen definerer den samlede engagement-værdi på stien, der fører til den aktuelt valgte side.
Jo større cirklen er, jo højere [engagement-værdi](#value).

Kontekstrudeområdet viser samlet total for besøg, værdi og værdi per besøgsmetrik, samt det samlede stiantal.
Hvis peger på en bestemt sti, viser total-området metrik fra denne sti.

## Kortvælger {#map-selector}

Du kan vælge forskellige kort med kortvælgerkontrollen. Du kan også se flere kort-metadata og tilføje et kort til din foretrukne liste, der automatisk gemmes på din profil.

### Grupper kortdata {#group-map-data}

Kort drives af trædatastrukturer, der består af [noder](#node).
Da hver enkelt [noder](#node) forventes at have et tilhørende element i indholds(master)-databasen,
hvis du vælger kortvælgerens afkrydsningsfelt Grupper kortdata, grupperes noderne af Sitecore-dataskabelonen, hvorfra de var oprettet.

Du kan f.eks. gruppere disse to stier:

- Home -&gt; TVs -&gt; 50" fladskærms-TV

- Home -&gt; Tablets -&gt; 12" tablet

til en enkelt stri:

- Startside -&gt; Produktkategoriside -&gt; Produktdetaljeside

Det er nyttigt at gruppere kortdata, når du vil udføre en sti-analyse på et sidekategoriniveau sammenlignet med et individuelt sideniveau.

## Datoområdevælger {#date-selector}

Du kan vælge et datoområde vha. dataoområdevælgeren enten ved at
vælge individuelle start- og slutdatoer fra kalendere, eller ved at
vælge en af de foruddefinerede datoområder.

### Datoer mangler data {#date-selector-missing-dates}

Der kan være tilfælde, hvor et kort ikke har nogen tilgængelige data for nogle datoer, selvom der er tilgængelige data før eller efter disse datoer.
Dette kan skyldes, at der ikke er registreret nogen interaktioner for en dato, eller fordi der er opstået en fejl under databehandlingen, og de involverede datoer med fejl er sprunget over.
Datointerval-vælgeren fremhæver datoer, hvor der ikke er adgang til data.
Kontakt systemadministratoren, hvis du oplever mange datoer i kalenderen, hvor der ikke er tilgængelige data.

### Utilgængelige datoer {#date-selector-unavailable-dates}

Afhængig af det datointerval, du har valgt, kan nogle datoer være
markeret utilgængelige. F.eks. Når du vælger en slutdato,
er alle datoerne forud for den aktuelle startdato markeret som utilgængelige.
Alle fremtidige datoer er også markeret som utilgængelige.

## Metrik-filter {#metrics-filter}

Dette filter fokuserer på filtrering af noder efter deres nøglemetrik: besøg, værdi, værdi pr. besøg og udgangsværdipotentiale.
Du kan bruge metrik-filteret til at reducere støjen eller til at finde interessante sammenhænge mellem forskellige metrikker og til at finde stioptimeringskandidater, f.eks.:

- Mange [besøg](#visits), men lav [værdi](#value).
- Høj [værdi pr. besøg](#value-per-visit), men lavt antal [besøg](#visits).
- Høj [udgangsværdipotentiale](#exit-value-potential).

## Applikationsmeddelelser {#application-messages}

Når du bruger applikationen, kan du se forskellige meddelelser i meddelelsesbjælken.

### "Nogle stier er skjulte. Brug filter til at se andre stier." {#page-analyzer-hidden-paths}

Applikationen viser kun 10 stier ad gangen. Du kan bruge metrik-filteret til at reducere antallet af stier, baseret på metrikkriterier.

### "Baseret på 500 stier ud af i alt X." {#page-analyzer-maximum-paths}

Nogle sider, som f.eks. Startsiden, kan have et massivt antal stier, der går via dem.
For at være effektiv, behandler applikationen kun de øverste 500 stier.
Du kan plukke et mere segmenteret kort eller vælge et mindre datointerval for at gøre noget ved dette.

### "Det valgte kort er under opbygning. Du ser måske delvise data." {#partial-map}

Denne meddelelse ses, hvis det aktuelt valgte kort lige er installeret,
men processen med opbygning af data endnu ikke er fuldført. Data for det nyinstallerede kort bør være tilgængelig ca. 30 minutter, efter kortet er installeret.

## Ordliste {#glossary}

### Map {#map}

En speciel marketingdefinition, der beskriver, hvordan data opbygges til sti-analyse.
Page Analyzer bruger kortdata og filtre til kun at vise dem, der går gennem den aktuelt valgte side.
Det filtrerede datasæt bruges til visualisering.
Du kan skifte til et andet kort med [kortvælgeren](#map-selector).

### Sti {#path}

En sekvens med [noder](#node) udgør en sti. Alle stier, der vises i Page Analyzer, går gennem den aktuelt valgte side.

### Node {#node}

Et element på en [sti](#path). For de fleste kort oversættes noder hovedsagelig til andre sider. 
Der er et sæt med metrikker, der gemmes på hver enkelt node: [værdi](#value), [besøg](#visits),
[værdi pr. besøg](#value-per-visit), [udgang](#exits), [udgangsværdi](#exit-value), [udgangsværdi pr. besøg](#exit-value-per-visit) og 
[gennemsnitlig tid brugt](#average-time-spent).

### Udgangsnode {#exit-node}

Node med [udgange](#exits) højere end nul, indikerer antallet af [besøg](#visits) der er afsluttet på denne node.

### Besøgsmetrik {#visits}

Det samlede antal besøg på en given node. Denne indeholder besøgsmetrikker fra alle underordnede noder.

### Værdimetrik {#value}

Den samlede engagement-værdi på en given node. Denne indeholder værdimetrikker fra alle underordnede noder.

### Værdi pr. besøgsmetrik {#value-per-visit}

Den samlede [engagement-værdi](#value) divideret med antal [besøg](#visits) på en given node.
Nogle gange defineres denne metrik som **effektivitet**.
Denne metrik er medvirkende til beregning af [udgangsværdipotentiale](#exit-value-potential).

### Udgangsmetrik {#exits}

Det samlede antal udgange på en given node.
Denne metrik identificerer, om en given node består af en fuld sti eller en indgangssti.
En node med flere udgange end nul, udgør en fuld sti.
Denne metrik er medvirkende til beregning af [udgangsværdipotentiale](#exit-value-potential).

### Udgangsværdimetrik {#exit-value}

Den samlede engagement-værdi på en given node, før udgang.
Kun noder, hvor der opstod udgang, har denne metrik.
Forskellen mellem denne og [værdimetrik](#value) er, at udgangsværdimetrik ikke tager højde for engagement-værdien af underordnede værdier.

### Udgangsværdi pr. besøg-metrik {#exit-value-per-visit}

Den samlede [engagement-værdi](#value) divideret med antal [besøg](#visits) på en given [udgangsnode](#exit-node). Kun noder,
hvor der opstod udgang, har denne metrik beregnet. Forskellen mellem denne
metrik og [værdi pr. besøg](#value-per-visit)-metrik er, at denne metrik ikke
medtager engagement-værdi pr. besøg fra underordnede noder.
Denne metrik er medvirkende til beregning af [udgangsværdipotentiale](#exit-value-potential).

### Udgangsværdipotentiale-metrik {#exit-value-potential}

Udgangspotentialet indikerer en beregnet [engagement-værdi](#value), der kan være
opnået i gennemsnit via optimering. Det beregnes kun for [udgangsnoder](#exit-node).
Du kan betragte det som en avanceret bounce-metrik, hvor der også tages højde for tab på engagement-værdien eller værdilækage
ud over kun [udgange](#exits). Hvis du ved, hvor stor [værdi pr. besøg](#value-per-visit), der er
samlet på alle stier længere nede, og hvor stor [værdi pr. besøg](#value-per-visit), der er gemt på [udgangsnoden](#exit-node), så kan metrikken
beregnes ved at tage delta mellem de to og gange med antallet af udgange med følgende formel:

(værdi pr. besøg - udgangsværdi pr. besøg) * udgange