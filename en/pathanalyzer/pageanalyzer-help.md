# Getting started with Page Analyzer {#intro}
While the main Path Analyzer application available via Launchpad focuses on advanced path analysis, 
the Page Analyzer focuses only on the paths leading to and from a specific page.
The main goal of the application is to understand how customers get to a certain destination (a page) and what they do afterwards.
The data visualization cues help you to understand the paths with the most traffic (visits) and most engagement value per visit, 
allowing you to pinpoint good and bad paths.
You can drill down to a particular path and explore path details.

## How to read the visualization {#map-key}
The visualization places the currently selected page at the center (shown as a large circle with the page icon) and shows all paths leading in and out of it.

The Landings area shows how many paths started with the currently selected page.

The Exits area shows the number of exits at the currently selected page and the total accumulated [exit value potential](#exit-value-potential).

The horizontal lines that are flowing *into* the currently selected page represent incoming paths.
The circles placed on top of the lines represent [nodes](#node) on that path. Nodes generally translate to pages.

The horizontal lines that are flowing *from* the currently selected page to the right represent outgoing paths.

The circles placed on top of the lines represent [nodes](#node) on that path. Nodes generally translate to pages.
To simplify the visualization, only the first page is shown on outgoing paths.

The line thickness defines the total [visits](#visits) to the currently selected page from the specific path.
The thicker the path, the more visits are going to the selected page for a given path.

The line color defines the [value per visit](#value-per-visit) on this specific path to the currently selected page.
The greener the path, the higher the [value per visit](#value-per-visit) is compared to other paths leading into the currently selected page.
Paths with the least value per visit are shown in red.

The size of the circle defines the total engagement value on the path that leads to the currently selected page.
The larger the circle, the higher the [engagement value](#value).

The Context Pane area shows the aggregated totals for the visits, value, and value per visit metrics, as well as the total path count.
If you hover over a particular path, the totals area shows the metrics from that path.

## Map selector {#map-selector}

You can select various maps using the Map selector control.
You can also see more map meta-data and add a map to your favorites list, which will automatically be saved to your profile.

### Group map data {#group-map-data}

Maps are powered by tree data structures that consist of [nodes](#node).
Because each [node](#node) is expected to have a corresponding item in the content (master) database, 
if you select the Map selector's Group map data checkbox, the nodes will be grouped by the Sitecore data template from which they were created.

For example, you can group these two paths:

- Home -&gt; TVs -&gt; 50" flat screen TV

- Home -&gt; Tablets -&gt; 12" tablet

into a single path:

- Landing Page -&gt; Product Category Page -&gt; Product Detail page

Grouping map data is useful when you'd like to perform path analysis on a page category level compared to an individual page level.

## Date range selector {#date-selector}

You can select a date range using the date range selector either by
selecting individual start and end dates from the calendars, or by
choosing one of the predefined date ranges.

### Dates missing data {#date-selector-missing-dates}

There may be cases where a map has no available data for some dates, even if there are available data before or after these dates.
This may be because there are no interactions recorded for a date, or because an error occurred during data processing and the dates involved in the error were skipped.
The date range selector highlights dates for which no data are available.
Please contact your system administrator if you encounter many dates in the calendar with no available data.

### Unavailable dates {#date-selector-unavailable-dates}

Depending on the date range that you have selected, some dates can be
marked as unavailable for selection. For example, when you select an end
date, all dates prior to the current start date are marked as unavailable.
All future dates are also marked as unavailable.

## Metrics filter {#metrics-filter}

This filter focuses on filtering nodes by their key metrics: visits, value, value per visit, and exit value potential.
You can use the Metrics filter to reduce the noise or to find interesting correlations between different metrics and for finding path optimization candidates, for example:

- High [visits](#visits), but low [value](#value).

- High [value per visit](#value-per-visit), but low [visits](#visits).

- High [exit value potential](#exit-value-potential).

## Application messages {#application-messages}
When using the application, you can see various messages in the message bar.

### "Some paths are hidden. Use filter to see other paths." {#page-analyzer-hidden-paths}
The application shows only 10 paths at once.
You can use the Metrics filter to reduce the number of paths based on any metrics criteria.

### "Based on 500 paths out of X total." {#page-analyzer-maximum-paths}
Some pages, such as the Home page, can have a massive amount of unique paths going through them.
For efficiency, the application processes the top 500 paths only.
You can pick a more segmented map or select a smaller date interval to address this.

### "The selected map is being built. You may see partial data." {#partial-map}
This message can be seen if the currently selected map was recently deployed but the
process of building data for this map hasn't been completed. Data for the newly deployed map should be available approximately 30 minutes after map deployment.

## Glossary {#glossary}

### Map {#map}

A special marketing definition that describes how to build the data for path analysis.
Page Analyzer uses map data and filters all paths to show only the ones that are going through the currently selected page.
This filtered dataset is used for visualization.
You can switch to another map using [map selector](#map-selector). 

### Path {#path}

A sequence of [nodes](#node) make up a path. All paths shown in Page Analyzer go through the currently selected page.

### Node {#node}

An element on a [path](#path). For most maps, nodes essentially translate to other pages.
There is a set of metrics that are stored on each node: [value](#value), [visits](#visits),
[value per visit](#value-per-visit), [exits](#exits), [exit value](#exit-value), [exit value per visit](#exit-value-per-visit), and [average time
spent](#average-time-spent).

### Exit node {#exit-node}

Node with [exits](#exits) greater than zero, indicating the number of [visits](#visits) that terminated on this node.

### Visits metric {#visits}

The total aggregated visits on a given node. This includes visits metrics from all descendant nodes.

### Value metric {#value}
The total aggregated engagement value on a given node. This includes value metrics from all descendant nodes.

### Value per visit metric {#value-per-visit}

The aggregated [engagement value](#value) divided by [visits](#visits) on a given node.
Sometimes, this metric is defined as **efficiency**.
This metric is instrumental in calculating [exit value potential](#exit-value-potential).

### Exits metric {#exits}

The total amount of exits on a given node.
This metric identifies whether a given node comprises a full path or an entry path.
Any node with exits greater than zero comprises a full path.
This metric is instrumental in calculating [exit value potential](#exit-value-potential).

### Exit value metric {#exit-value}

The aggregated engagement value on a given node before exiting.
Only nodes where exits occurred have this metric.
The difference between this and the [value metric](#value) is that the exit value metric doesn't take into account engagement value of the descendant nodes.

### Exit value per visit metric {#exit-value-per-visit}
The aggregated [engagement value](#value) divided by [visits](#visits) on a given [exit node](#exit-node). Only nodes
where exits occurred have this metric calculated. The difference between
this metric and the [value per visit](#value-per-visit) metric, is that this metric doesn't
account for engagement value per visit of the descendant nodes.
This metric is instrumental in calculating [exit value potential](#exit-value-potential).

### Exit value potential metric {#exit-value-potential}

The exit potential indicates a projected [engagement value](#value) that could be
gained on average through optimization. It is only calculated for the [exit nodes](#exit-node).
You can consider it an advanced bounce metric, where the engagement value loss or value leakage is also taken
into account besides just [exits](#exits). If you know how much [value per visit](#value-per-visit) is
aggregated on all paths further down, and how much [value per visit](#value-per-visit) is stored on the [exit node](#exit-node), then this metric can be
calculated by taking the delta between the two and multiplying by the number of exits, using the following formula:

(value per visit - exit value per visit) * exits