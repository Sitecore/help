# Kom i gang med Path Analyzer {#intro}
Med Path Analyzer kan du analysere de stier, som kunder følger, når de
interagerer med dit brand, med fokus på identifikation af de mest
effektive og mindst effektive stier og stier med potentiale til
optimering. Du kan analysere de stier, som kunderne især følger
[kanaler](https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels)
(e-mail-marketing, social osv.), mens der interageres med
[kampagner](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity),
og deres måde at konvertere forretningskritiske aktiviteter, som f.eks.
[mål](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals),
[events](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events)
og
[resultater](https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes).

## Nøglescenarier {#scenarios}

### 1. Undersøgelse af kortet {#”scenario1"}

[Sådan forstås de visuelle referencer](#map-key), og dataene bag dem er
vigtige for at kunne aflæse et kort effektivt og spotte mønstre. De
funktioner, der oplistet nedenfor, er nyttige, når du begynder din
analyse af stier, især, hvis det er første gang, du anvender programmet,
og du ikke er sikker på, hvor du skal starte.

[Rapportfunktion](#reports), der er tilgængelig fra kontekstruden,
hjælper med hurtigt at fremhæve mønstre på en given rapportkategori.
Hvis du f.eks. ønsker at se alle stier, som ikke generer en
[engagement-værdi](#value), vælger du ganske enkelt kategorien "Stier
uden værdi" og klikker gennem top 10-stierne. Der er i alt [8
rapportkategorier](#reports), der kan undersøges.

[Dashboard-visning](#dashboard) er nyttig, hvis du lige er startet med
sti-analyse og ikke er helt fortrolig med [andre kortvisninger](#map-views)
endnu. I dashboard-visning kan du
se: [Kort-KPI’er](#map-kpis); [Førende
sti-indgange](#top-path-entries); og [Udvalgt sti](#featured-path); og
du kan få adgang til [rapporter](#reports) og [kanaler](#funnels)
-funktioner.

[Tabel-visning](#table-view) er en anden fremragende måde at starte
sti-analyse på. Det anvender en visualisering, der minder meget om
Excel, med alle stier og nøgle-metrikker, og gør det muligt at udføre
filtrering.

[Der er adgang til metrik-filter](#metrics-filter) fra alle visninger,
bortset fra dashboardet, hvor du kan fokusere på stier, der er baseret
på et bestemt sæt metrikker. Du kan anvende filteret til at vise et kort
over stier med høj [værdi](#value), men med lavt [besøgstal](#visits),
stier med høj [værdi pr. besøg](#value-per-visit), eller stier med høj
[udgangsværdipotentiale](#exit-value-potential). På denne måde kan du
filtrere kortet, så det viser gode stier, ringe stier og stier til
optimering.

### 2. Du kan undersøge sider fra eller til en bestemt side {#scenario2}

Hvis du kender navnet på en bestemt side, kan Path Analyzer let vise
alle stier, der fører til og fra denne side vha.
[sti-filter](#path-filter) , så du kan oprette en sti, baseret på sidens
navn. Hvis du har en destinationsside i tankerne, kan du inkludere den i
sti-filteret, så du kan få alle stier fra side A til side B. Med
[oplevelseskort](#experience-maps) kan du anvende denne teknik til at
filtrere stier, der fører til et mål.

Svarende til [Scenarie 1](#scenario1), kan du anvende
[metrik-filteret](#metrics-filter) til yderligere at forfine et
filtreret kort, der er baseret på en kombination af nøgle-metrikker.

Når du anvender filteret, kan du enten undersøge forskellige visninger
efter [læsning](#map-key) af det filtrerede kort eller benytte dig af
[rapport-funktionen](#reports) for hurtigt at navigere til top
10-stierne i en given [rapport-kategori](#reports). Rapporterne viser
kun stier, der matcher med det anvendte [sti-filter](#path-filter) og
[metrik-filteret](#metrics-filter).

### 3. Sti-analyse på makroniveau (mål, events, resultater) {#scenario3}

Når kort på sideniveau giver for mange detaljer,
[Oplevelseskort](#experience-maps) er ofte nyttige for at forstå
sti-analyse på makroniveau med fokus på
[kanaler](https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels),
[kampagner](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity),
[mål](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals),
[events](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events)
og
[resultater](https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes).

### 4. Undersøgelse af en kampagne- eller kanaltrafik {#scenario4}

Hvis du ønsker at forstå, hvordan dine kunder interagerer med dit brand
gennem en bestemt
[kanal](https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels)
eller
[kampagne](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity),
kan du plukke en af standard [kanalkortene](#channel-maps) med
[kortvælgeren](#map-selector) eller [oprette og
installere](#how-to-create-a-new-map) et nyt
[kampagnekort](#campaign-maps) med fokus på den omhandlede kampagne. Du
kan også anvende [oplevelseskort](#experience-maps), som i [Scenarie
3](#scenario3) og anvende [sti-filteret](#path-filter) til at vise stier
fra en bestemt kanal eller kampagne.

### 5. Oplev et kort med fokus på et bestemt segment {#scenario5}

Hvis du vil undersøge stier fra et bestemt kundesegment, [kan du oprette
et nyt kort](#how-to-create-a-new-map) og derefter angive
segmentreglerne i filterfeltet vha. den kendte [grænseflade
med](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/the_rule_set_editor)
regelsæt-editoren. Når det nye kort er installeret, kan du vælge det i
kortvælgeren og undersøge det på samme måde, som du ville undersøge
standardkortene.

### 6. Undersøgelse af stier, der fører til et mål {#scenario6}

En måde at undersøge stier, der fører til et givent mål, er at anvende
standard [oplevelseskort med mål](#experience-maps) og angive målet i i
[sti-filteret](#path-filter).

En anden måde er at [oprette og installere](#how-to-create-a-new-map) et
nyt [målkort](#goal-maps), der kun har fokus på stier med det angivne
mål. Du kan anvende samme teknik til at undersøge stier for bestemte
aktiver eller resultater.

## Kort {#maps}

Et kort er en speciel markedsføringsdefinition for sti-analyse, der har
to nøgleattributter: korttype og kortfilter. Korttypen beskriver,
hvordan der opbygges de data, der driver kortet, og beskrives mere
detaljeret [her](#map-types). Kortfilteret er en ekstra, men vigtig
attribut, der hjælper med at definere et segmenteret kort vha.
[regelsæt-editoren](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/the_rule_set_editor)
og et omfattende sæt betingelser.

Ud over disse to nøgleattributter, har hvert enkelt kort en unik
identifikator, et navn og en type. Du kan også inkludere andre ekstra
attributter, som f.eks. beskrivelse.

Svarende til andre marketingdefinitionselementer kan du [oprette et kort
i marketingkontrolpanelet.](#how-to-create-a-new-map).

Kort visualiseres vha. [kortvisning](#map-views).

## Korttyper {#map-types}

Korttyper foreskriver, hvordan interaktionsdata fra xDB transformeres
til sti-analyse. Der er forskellige korttyper tilgængelige som standard.

### Sidekort {#page-maps}

Disse kort er opbygget ud fra sekvenser af sidebesøg i en given
interaktion. Der er som standard nogle få undertyper tilgængelige for
sidekort. Disse kortundertyper er bekvemme, da du let kan oprette et
sidekort med fokus på en bestemt interaktionsattribut (kanal, kampagne,
mål, aktiv osv.).

#### Målkort {#goal-maps}

Med målkort kan du oprette et sidekort, der fører til et bestemt mål.
Målkort ser bort fra sider, der er besøgt, efter et bestemt mål er nået.

Du kan oprette målkort i modsat tilstand ved at vælge afkrydsningsfeltet
Omvendt på målkortdefinitionselementet i marketingkontrolpanelet. Et
omvendt målkort vender rækkefølgen af sider, der fører til et bestemt
mål og anvender det valgte mål som startpunkt på kortet i stedet for den
konventionelle [internet-node](#internet-node).

#### Aktivkort {#asset-maps}

Med aktivkort kan du oprette sidekort, der fører til en bestemt
aktiv-download. Aktivkort ser bort fra sider, der er besøgt, efter et
bestemt aktiv er downloadet.

Du kan opbygge aktivkort i modsat tilstand ved at vælge
afkrydsningsfeltet Omvendt på aktivkortdefinitionselementet i
marketingkontrolpanelet. Et omvendt aktivkort vender rækkefølgen af
sider, der fører til download af et bestemt aktiv, og anvender det
valgte aktiv som startpunkt i stedet for den konventionelle
[internet-node](#internet-node).

#### Kampagnekort {#campaign-maps}

Med kampagnekort kan du oprette et sidekort for alle interaktioner fra
en bestemt kampagne.

#### Kanalkort {#channel-maps}

Med kanalkort kan du oprette et sidekort for alle interaktioner fra en
bestemt kanal.

#### Resultatkort {#outcome-maps}

Med resultatkort kan du oprette et sidekort, der fører til et bestemt
resultat.

### Oplevelseskort {#experience-maps}

I modsætning til sidekort kan oplevelseskort indeholde andre
interaktionsattributter, som f.eks.
[kanaler](https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels),
[kampagner](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity),
[mål](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals),
[events](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events)
og
[resultater](https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes),
som tillæg til sider. Du kan vælge disse interaktionsattributter med
afkrydsningsfelterne på oplevelseskortdefinitionselementet i
marketingkontrolpanelet. På denne måde kan oplevelseskort sætte dig i
stand til at fokusere mere på analyse på højt niveau i stedet for mere
detaljerede [sidekort](#page-maps).

Der er som standard adgang til tre oplevelseskort:

-   Oplevelseskort med mål. Indeholder kanal, kampagne (hvis
    tilgængelig), alle mål og resultater.

-   Oplevelseskort kun med værdimål. Samme som ovenfor, bortset fra, at
    mål med engagementværdi er tilføjet.

-   Oplevelseskort med side-events. Indeholder kanal, kampagne (hvis
    tilgængelig), kun indgangs- og udgangsside, alle side events og
    resultater.

Du kan let [oprette et nyt kort](#how-to-create-a-new-map), baseret på
et eksisterende kort med marketingkontrolpanelet.

### Sidespecifikke kort {#site-specific-maps}

Ud over korttyper, kan kort enten være **globale** eller
**sidespecifikke**. Globale kort er opbygget til alle sider, mens
sidespecifikke kort kun er bygget til en bestemt side. Om et kort er
globalt eller sidespecifikt, bestemmes af placeringen af kortet i
indholdet på træet i Path Analyzer i marketingkontrolpanelet. Alle
globale kort er placeret i */Kort/Standardkort/Globale kort*-mappen, og
alle sidespecifikke kort er placeret i
*/Kort/Standardkort/Sidekort*-mappen.

### Brugerdefinerede kort {#custom-maps}

Hvis der er registreret brugerdefinerede kort, der typisk kræver mindre
udviklingsindsats, kan du finde dem i */Kort/Brugerdefinerede
kort*-mappen.

### Sådan oprettes et nyt kort {#how-to-create-a-new-map}

Sådan oprettes et helt nyt kort:

1.  Åbn marketingkontrolpanelet fra startområdet.

2.  Gå til elementet Path Analyzer.

3.  Udvid kortelementet under Path Analyzer.

4.  Vælg den mapper, der passer til dit nye kort, baseret på de
    tilgængelige korttyper, der er beskrevet ovenfor.

5.  Opret et nyt kortelement.

6.  Angiv de nødvendige attributter, og evt. ekstra attributter til
    kortet.

7.  Gem kortelementet.

8.  Installer det nye kort med kommandoen til
    installationsarbejdsprocessen på fanen Gennemse.

Der opbygges historisk og livedata for kortet ca. 30 minutter efter
installation.

## Kortvælger {#map-selector}

Du kan vælge forskellige kort med kontrollen Kortvælger. Du kan også se
mere kort-metadata og tilføje et kort til din favoritliste, der
automatisk gemmes på din profil.

### Grupper kortdata {#group-map-data}

Kort drives af [træ-datastrukturer](#tree), der består af
[noder](#node). Da hver enkelt [node](#node) forventes at have et
tilhørende element i indholds(master)-databasen, hvis du vælger
kortvælgerens afkrydsningsfelt Grupper kortdata, grupperes noderne af
Sitecore-dataskabelonen, hvorfra de var oprettet.

Du kan f.eks. gruppere disse to stier:

-   Home -\> TVs -\> 50" fladskærms-TV

-   Home -\> Tablets -\> 12"-tablet

til en enkelt sti:

-   Startside -\> Produktkategoriside -\> Produktdetaljeside

Det er nyttigt at gruppere kortdata, når du vil udføre en sti-analyse på
et sidekategoriniveau sammenlignet med et indviduelt sideniveau.

## Datoområdevælger {#date-selector}

Du kan vælge et datointerval vha. dataoområdevælgeren enten ved at vælge
individuelle start- og slutdatoer fra kalendere, eller ved at vælge en
af de foruddefinerede datoområder.

### Datoer mangler data {#date-selector-missing-dates}

Der kan være tilfælde, hvor et kort ikke har nogen tilgængelige data for
nogle datoer, selvom der er tilgængelige data før eller efter disse
datoer. Dette kan skyldes, at der ikke er registreret interaktioner for
en dato, eller fordi der er opstået en fejl under databehandlingen, og
de involverede datoer med fejl er sprunget over. Datointerval-vælgeren
fremhæver datoer, hvor der ikke er adgang til data. Kontakt
systemadministratoren, hvis du oplever mange datoer i kalenderen, hvor
der ikke er tilgængelige data.

### Utilgængelige datoer {#date-selector-unavailable-dates}

Afhængig af det datointerval, du har valgt, kan nogle datoer være
markeret utilgængelige. F.eks. Når du vælger en slutdato, er alle
datoerne forud for den aktuelle startdato markeret som utilgængelige.
Alle fremtidige datoer markeres også som utilgængelige.

## Kortnøgle {#map-key}

Følgende kortnøgle anvendes på radial, vandret og lodret trævisning.

Når du læser et kort, repræsenterer størrelsen og farven på cirklerne og
linjerne mellem noderne på kortet information om, hvilke stier, der
giver højere [engagement-værdi](#value), højere [værdi pr.
besøg](#value-per-visit) eller er de mest [besøgte](#visits).

Cirkler repræsenterer [noder](#node). Afhængig af den valgte korttype,
kan noder repræsentere sider, mål eller andre markedsføringsaktiviteter.
Cirkler har følgende to visuelle egenskaber med information om noden:
størrelse og farve.

Størrelsen af en cirkel indikerer den samlede [engagement-værdi](#value)
for en [node](#node) og alle underelementerne. Med andre ord, så udgør
en større node en større samlet [engagement-værdi](#value).

Farven på en cirkel indikerer [værdi pr. besøg](#value-per-visit) for en
[node](#node), sammenlignet med værdi pr. besøg af dens overordnede, og
den hjælper dig med at spotte ændringen i denne metrik, når du går
yderligere ned i dybden på denne sti. Hvis en cirkel bliver rød, så er
[værdi pr. besøg](#value-per-visit) faldet for denne [node](#node). Hvis
en cirkel bliver grønnere end dens overordnede, så er [værdi pr.
besøg](#value-per-visit) steget for denne [node](#node). Cirkelfarven
hjælper dig også med at sammenligne [værdi pr.
besøg](#value-per-visit)-metrikken mellem sidestillede noder og
bestemmer, hvor de højeste [værdi pr. besøg](#value-per-visit)-stier
fortsætter fra en given [node](#node).

Cirkler med en tyk mørkegrå kant udgør specielle "[andre
noder](#other-nodes)".

Linjer, der forbinder kortnoder, repræsenterer stier mellem
[node](#node) A og [node](#node) B. Linjer, der har følgende visuelle
egenskaber, giver informationer om [stien](#path): tykkelse og delvise
skygge.

Tykkelsen af en linje indikerer, hvor mange [besøg](#visits) (trafik) ,
der gik fra [node](#node) A til [node](#node) B, sammenlignet med
sideordnede for [node](#node) B, der gør det let at identificere stier
med høj trafik.

En delvis skygge på en linje komplementerer linjetykkelsen og anvendes
til at vise sti-besøg på dybere niveauer, hvor det er sværere at se
forskellen i linjetykkelsen.

Som en generel retningslinje, så se efter tykke linjer, uanset om det er
små eller røde cirkler, der angiver et højt antal [besøg](#visits) på
stier, der hhv. har lav [engagement-værdi](#value) (size) og lav [værdi
pr. besøg](#value-per-visit) (farve).

### Andre noder {#other-nodes}

På grund af begrænsningerne i trævisninger (radial, vandret og lodret)
når visualisering af store kort med ekstremt meget indhold, bliver
mindre vigtige noder, der ikke passer i et bestemt visualiseringsniveau,
kombineret til en speciel "anden" node. [Tabel-visning](#table-view) har
ikke denne begrænsning.

Du kan se en liste over noder, der er kombineret i "Andre noder" ved at
vælge fanen Næste på kontekstruden eller vælge fanen Andre i
node-popoveren.

Ved at anvende entet et [sti-filter](#path-filter) eller et
[metrik-filter](#metrics-filter) reduceres normalt antallet af "Andre
noder", der vises på et kort.

## Kortvisning {#map-views}

Der er fem forskellige visninger tilgængelige, som man kan vælge blandt
til analyse af dine kort. Dashboard er en standardvisning, der giver en
introduktion til sti-analyse og er beskrevet [nedenfor](#dashboard).

### Radial visning {#radial-view}

Radial visning har den fordel at kunne vise mere kortdata på skærmen,
men er ikke ideel til mindre kort eller filtrerede kort.
[Internet-noden](#internet-node) er i midten af denne visning.

### Lodret visning {#vertical-view}

Lodret visning er meget bedre til at vise mindre kort eller filtrerede
kort og giver oftest en bedre læsbarhed i forhold til [radial
visning](#radial-view). [Internet-noden](#internet-node) findes øverst
på denne visning.

### Vandret visning {#horizontal-view}

Svarende til lodret visning, så er vandret visning god til mindre kort
og giver sædvanlig bedre læsbarhed i forhold til [radial
visning](#radial-view). [Internetnoden](#internet-node) er længst til
venstre.

### Tabelvisning {#table-view}

Tabel-visning er anderledes, da den kun viser [fulde stier](#path), der
skyldes, at kortdata er i en [træstruktur](#tree), der ikke let kan
vises som en tabel.

##Dashboard {#dashboard}

Dashboard er en speciel visning, der introducerer til sti-analyse.

### Kort-KPI’er {#map-kpis}

Der er adgang til seks Key Performance Indicators (KPI’er) på
dashboardet som standard for følgende metrik: [besøg](#visits),
[værdi](#value), [værdi pr. besøg](#value-per-visit) og ekstra
resultat-metrikker: [pengeværdi](#monetary-value),
[outcomes](#outcomes), og [gennemsnitlig
pengeværdi](#average-monetary-value).

Resultat-metrikker vises ikke som standard og kan aktiveres fra
[Applikations- indstillinger](#application-settings).

Hver enkelt kort-KPI har en trend-indikator, der viser stigning eller
fald i en metrik, sammenlignet med metrikken over samme datointerval for
samme kort tidligere. F.eks. Hvis det aktuelt valgte datointerval er i
dag, så baseres trend-indikatoren på dataene fra i går.

### Førende sti-indgange {#top-path-entries}

Denne liste viser top 10-stien, med startpunkter på det aktuelle kort. I
Path Analyzer-terminologi er disse top 10 [noder](#node) i første
niveau, sorteret efter kombineret [værdi-](#value) og
[besøgs](#visits)-metrikker.

### Udvalgt sti {#featured-path}

Den udvalgte sti viser stien fra det aktuelt valgte kort med det mest
interessante sæt med nøglemarketing-metrikker. Valget af udvalgt sti er
baseret på en algoritme, der vurderer, om kontoen enten har en
[udgangsværdi potentiale](#exit-value-potential) eller er kombineret med
[værdi](#value) og [besøg](#visits), og derefter vælger den øverste sti
i hver enkelt metrik-kategori. Eftersom muligheden for optimering er
relativt begrænset for korte stier, så prioriterer algoritmen de længste
stier.

### Foretrukken kanal {#favorite-funnel}

A Foretrukken kanal er en kanal, der er markeret som foretrukken på et
bestemt kort. Dette kan ændres til hver en tid på kontekstruden under
Kanaler En foretrukken kanal gemmes i din brugerprofil og tilknyttes det
kort, hvor den er markeret som foretrukken.

## Raporter {#reports}

Path Analyzer-rapporter viser de øverste stier i forskellige kategorier.
Rapporter introducerer det mest interessant stier i det aktuelt valgte
kort, så du hurtigt kan finde frem til gode og dårlige stier. Som
standard er der adgang til otte rapportkategorier. Der er adgang til op
til 10 stier, som kan vælges i hver enkelt kategori.

### Højest besøgte {#highest-visited-report}

Stier med det højeste antal [besøg](#visits).

### Højeste værdi {#highest-valuable-report}

De stier, der genererer den højeste [engagement-værdi](#value).

### Højeste antal besøg og værdi {#highest-visitsvalue-report}

De stier, der genererer den højeste [engagement-værdi](#value) og det
højeste antal [besøg](#visits).

### Højeste værdi pr. besøg {#highest-valuepervisit-report}

De stier, der genererer den højeste [værdi pr. besøg](#value-per-visit).

### Stier uden værdi {#paths-without-value-report}

De stier, som kunderne forlod uden at generere nogen
[engagement-værdi](#value).

### Højeste udgangsværdipotentiale {#highest-evp-report}

De stier, der genererer den højeste
[udgangsværdipotentiale](#exit-value-potential).

### Højeste resultater {#highest-outcomes-report}

De stier, der genererer de højeste [resultater](#outcomes).

### Højeste pengeværdi {#highest-monetaryvalue-report}

De stier, der generer den højeste samlede [pengeværdi](#monetary-value),
som kommer fra resultater.

## Kanaler {#funnels}

En kanal er en veldefineret sekvens af trin, som kunderne forventes at
foretage på deres vej til at opnå et virksomhedsmål. Virksomheder
definerer deres egen kanal. For en e-handelsside er det sandsynligvis en
udtjeknings- kanal, der kan repræsenteres som en række sider,
side-events eller mål, afhængig af implementering af specifikationer.

Kanaler i Path Analyzer gør det mulig at analysere de handlinger og
stier, som kunderne tager på deres vej til at konvertere mål og
resultater. Derefter kan du optimere stierne for at forbedre
konverteringsrater, f.eks. ved at implementere
[brugertilpasning](https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/personalization),
[M/V-test](https://doc.sitecore.net/sitecore_experience_platform/analyzing__reporting/experience_optimization__content_testing/ab_and_multivariate_testing),
eller
[indholdstest](https://doc.sitecore.net/sitecore_experience_platform/analyzing__reporting/experience_optimization__content_testing).

Der er adgang til kanalfunktionen fra kontekstruden, hvor du kan
undersøge en kanal, der er defineret i marketingkontrolpanelet.

Når en kanal er valgt, kan du vise en grafisk repræsentation af de
sporede trin fra en kanal i Path Analyzer i form af et søjlediagram.
Diagrammet giver oplysninger om antallet af kunder, der gennemfører
hvert enkelt kanal, samt hvor mange kunder, der fortsætter til næste
trin. Du kan også skifte mellem metrikker, som f.eks. [besøg](#visits),
[værdi](#value) og [værdi pr. besøg](#value-per-visit). Under
diagrammet, vises listen over alle andre metrikker, der giver
KPI-indikatorerne for kanalen. Disse metrikker tages fra det sidste trin
i kanalen. Dataene er beregnet på basis af målet for en interaktion i
forhold til en Customer lifetime Value (CLV).

En kanal kan markeres som foretrukken ved at klikke på stjerne-ikonet
ved siden af kanalnavnet. Denne handling gør kanalen synlig på
[Dashboard-visningen](#dashboard).

Hvis du vil gemme en valgt sti som en kanal, skal du klikke på Gem som
kanal i sidefodsområdet på kontekstruden.

## Kortfiltre {#map-filters}

Der er adgang til to typer filtre, så du kan fokusere på bestemte stier.

### Stifilter {#path-filter}

Med stifiltre kan du filtrere et kort, baseret på navnet af en node, der
enten kan være en side, et mål, eller en anden markedsføringsattribut,
afhængig af typen af det aktuelle kort. Du kan f.eks. anvende
stifilteret til at finde ud af, hvordan kunder kommer til den pågældende
side. Du indstiller ganske enkelt en bestemt side som et element af
stifilteret, og klikker på Anvend. Kortet justeres i overensstemmelse
hermed.

Med stifilteret kan du også opbygge et kortfilter fra side A til side B.
Normalt skal du ikke anvende mere end tre elementer i stifilteret, men
du kan angive et hvilket som helt antal elementer der. Stifilteret
indsnævrer listen over indstillinger, baseret på de tilgængelige data i
det aktuelle kort.

### Metrik-filter {#metrics-filter}

Dette filter fokuserer på filtrering af noder efter deres
nøglemetrikker: [besøg](#visits), [værdi](#value), [værdi pr.
besøg](#value-per-visit) og
[udgangsværdipotentiale](#exit-value-potential).

På grund af dets sekundære natur i forhold til hoved-
[stifilteret](#path-filter) kan metrik-filteret vise, hvor mange
matches, for det aktuelle [stifilter](#path-filter), der er, samt
sammenhængen mellem forskellige metrikker. Du kan også anvende
metrik-filteret uden [stifilteret](#path-filter) og filtrere de mindre
besøgte noder, der reducerer støj på det aktuelle kort.

Endelig kan du med metrik-filteret finde interessante sammenhænge mellem
forskellige metrikker og til at finde stioptimeringskandidater, f.eks.:

-   Højt antal [besøg](#visits), men lav [værdi](#value).

-   Høj [værdi pr. besøg](#value-per-visit), men lavt antal
    [besøgs](#visits).

-   Højt [udgangsværdipotentiale](#exit-value-potential).

## Eksporter et kort {#export-map}

Du kan eksportere data til et hvilket som helst kort som et
kommasepareret datasæt vha. følgende to kommandoer fra handlingsmenuen:

-   Download som CSV

-   Kopier til udklipsholder

Begge kommandoer anvender samme format, og findes for at gøre det muligt
at eksportere forskellige workflows.

## Applikationsmeddelelser {#application-messages}

Når applikationen anvendes, kan du se forskellige meddelelser i
meddelelsesbjælken.

### "Tabelvisningen viser top X-stier ud af i alt Y." {#table-top}

Denne meddelelse kan ses, når [tabelvisning](#table-view) gengiver
ekstremt store kort. [Tabelvisning](#table-view) kan kun vise top 500
[fulde stier](#path). Anbefalede handlinger for denne meddelelse er: Anvend
enten] [stifilteret](#path-filter) eller
[metrik-filteret](#metrics-filter) for at sænke antallet af synlige
række; gør datoområdets interval mindre for kortet; eller
[opret](#how-to-create-a-new-map), eller [vælg](#map-selector) et
filtreret kort, der har mindre data.

### "X mindre vigtige noder er grupperet sammen med andre noder." {#other-nodes-message}

Denne meddelelse kan ses vha. enten radial, vandret eller lodret visning
på store kort med ekstremt meget indhold. For at sikre, at kortet er
læsbart, er mindre betydelige noder, der ikke kan passe ind i et bestemt
visualiseringsniveau kombineret i en speciel 'anden' node. Bemærk, at
[tabelvisning](#table-view) ikke har denne begrænsning. Foreslåede
handlinger for denne meddelelse er: Anvend either the
[stifilteret](#path-filter) eller [metrik-filtret](#metrics-filter) for
at mindske antallet af synlige noder; gør datointervallet for kortet
mindre; eller [opret](#how-to-create-a-new-map) eller
[vælg](#map-selector) et filtreret kort, der har mindre data.

### "Det valgte kort opbygges. Du ser måske delvise data." {#partial-map}

Denne meddelelse ses, hvis det aktuelt valgte kort lige er installeret,
men processen med opbygning af data endnu ikke er fuldført. Data for det
nyinstallerede kort bør være tilgængelig ca. 30 minutter, efter kortet
er installeret.

## Applikationsindstillinger {#application-settings}

Nedenfor findes en liste over applikationsindstillinger, du kan ændre
for at brugertilpasse din oplevelse af Path Analyzer-applikationen:

-   Aktiver/deaktiver overgangseffekter

-   Vis/skjul etiketter som standard

-   Vis/skjul forklaring som standard

-   Vis/skjul resultat-metrikker

-   Vis/skjul hjælp ved opstart

-   Tillad valg af datoer med manglende data

Der er adgang til disse data fra Handlingsmenu under Indstillinger.

## Ordliste {#glossary}

### Kort {#map}

En særlig markedsføringsdefinition, der beskriver, hvordan data til stianalyser oprettes.
Ethvert kort, der anvendes, har et [træ](#tree), der er gemt i rapporteringsdatabasen.

### Træ {#tree}

Den samlede datastruktur til stianalyser, der er gemt i en rapporteringsdatabase for hvert
anvendte kort, og som består af et hierarki af [noder](#node).
Alle træer skal have en særlig rodnode, som kaldes en [internetnode](#internet-node).

### Node {#node}

Det centrale element i [træet](#tree).
Alle noder, bortset fra [internetnoden](#internet-node), har en overordnet node og kan have underordnede noder.
Afhængigt af [korttypen](#map-types) kan en node enten repræsentere en side (på et [sidekort](#page-maps)),
et mål eller en anden markedsføringsattribut (kanal, kampagne osv.) på et [oplevelseskort](#experience-maps).

Hver node har et entydigt numerisk ID, et navn og et GUID, der svarer til et element fra indholdsdatabasen.

Forskellige typer metrikker er gemt i hver node:

- **Samlede metrikker**, bl.a. [værdi](#value), [besøg](#visits), [gennemsnitlig tid brugt](#average-time-spent), [resultater](#outcomes) og [pengeværdi](#monetary-value).
Disse metrikker omfatter værdier fra alle underordnede noder.

- **Udgangsmetrikker**, bl.a. [udgange](#exits) og [udgangsværdi](#exit-value).
Disse metrikker omfatter ikke værdier fra alle underordnede noder og beregnes kun, hvis den aktuelle node er en [udgangsnode](#exit-node).

- **Beregnede metrikker**, bl.a. [værdi pr. besøg](#value-per-visit), [udgangsværdi pr. besøg](#exit-value-per-visit), [gennemsnitlig pengeværdi](#average-monetary-value) og [udgangsværdipotentiale](#exit-value-potential).

### Udgangsnode {#exit-node}

Node med [udgange](#exits), der er større end nul, og som angiver det antal [besøg](#visits), som sluttede på denne node.

### Internetnode {#internet-node}

Den særlige [rodnode](#node), der fungerer som en startnode for alle [stier](#path),
og som samler alle metrikker fra alle stier på det pågældende [kort](#map).

### Sti {#path}

En række [noder](#node) udgør en sti. Eftersom
[træet](#tree) består af samlede data, er det vigtigt at skelne mellem to slags stier:
**indgangssti** og **fuld sti**.

En **fuld sti** består af et komplet besøg fra indgangsnode til [udgangsnode](#exit-node).
En **indgangssti** behøver dog ikke at slutte med en udgang.
Det er vigtigt at forstå forskellen mellem de to slags stier,
fordi [tabelvisningen](#map-views) og [rapportfunktionen](#reports) kun fungerer sammen med fulde stier.

### Besøgsmetrik {#visits}

Det samlede antal besøg for en given node. Denne værdi omfatter besøgsmetrikker fra alle underordnede noder.

### Værdimetrik {#value}
Den samlede engagementsværdi for en given node. Denne værdi omfatter værdimetrikker fra alle underordnede noder.

### Værdi pr. besøgsmetrik {#value-per-visit}

Den samlede [engagementsværdi](#value) divideret med [besøg](#visits) for en given node.
Nogle gange defineres denne metrik som **effektivitet**.
Denne metrik er med til at beregne [udgangsværdipotentiale](#exit-value-potential).

### Udgangsmetrik {#exits}

Det samlede antal udgange for en given node.
Denne metrik identificerer, om en given node består af en fuld sti eller en indgangssti.
En node med flere udgange end nul udgør en fuld sti.
Denne metrik er med til at beregne [udgangsværdipotentiale](#exit-value-potential).

### Udgangsværdimetrik {#exit-value}

Den samlede engagementsværdi for en given node før udgang.
Kun de noder, hvor der opstod udgang, har denne metrik.
Forskellen mellem denne og [værdimetrikken](#value) er, at udgangsværdimetrikken ikke tager højde for engagementsværdien for de underordnede noder.

### Udgangsværdi pr. besøgsmetrik {#exit-value-per-visit}
Den samlede [engagementsværdi](#value) divideret med [besøg](#visits) for en given node [udgangsnode](#exit-node). Metrik beregnes kun for de noder,
hvor der opstod udgang. Forskellen mellem
denne metrik og metrikken [værdi pr. besøg](#value-per-visit) er, at denne metrik ikke
tager højde for engagementsværdi pr. besøg for de underordnede noder.
Denne metrik er med til at beregne [udgangsværdipotentiale](#exit-value-potential).

### Metrik for udgangsværdipotentiale {#exit-value-potential}

Udgangspotentialet angiver en forventet [engagementsværdi](#value), som i gennemsnit kan
opnås gennem optimering. Den beregnes kun for [udgangsnoder](#exit-node).
Du kan betragte det som en avanceret bounce-metrik, hvor der også tages højde for tab på engagementsværdien eller værdilækagen
og ikke kun [udgange](#exits). Hvis du ved, hvor megen [værdi pr. besøg](#value-per-visit), der
samles for alle stier længere nede i hierarkiet, og hvor megen [værdi pr. besøg](#value-per-visit), der gemmes for [udgangsnoden](#exit-node), kan denne metrik
beregnes ved at tage deltaet mellem de to og gange med antallet af udgange ved at benytte følgende formel:

(værdi pr. besøg - udgangsværdi pr. besøg) * udgange

### Resultatmetrik {#outcomes}

Det samlede antal resultater for en given node. Denne værdi omfatter
resultater fra alle underordnede noder.
Læs mere om resultater <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">her</a>.

### Pengeværdimetrik {#monetary-value}

Den samlede pengeværdi for en given [node](#node). Pengeværdien
hentes fra de realiserede resultater. Denne værdi omfatter pengeværdien
fra alle underordnede noder.
Læs mere om resultater <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">her</a>.

### Metrik for gennemsnitlig pengeværdi {#average-monetary-value}

Den gennemsnitlige pengeværdi opnået pr. resultat for en given [node](#node). Pengeværdien
hentes fra de realiserede resultater. Denne værdi omfatter
den gennemsnitlige pengeværdi fra alle underordnede noder.
Læs mere om resultater <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">her</a>.

### Metrik for gennemsnitlig tid brugt {#average-time-spent}

Den gennemsnitlige mængde tid, kunder har brugt på en given [node](#node) i sekunder.
