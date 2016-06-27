# Getting started with Page Analyzer {#intro}
While the main Path Analyzer application available via Launchpad focuses on advanced path analysis, the Page Analyzer is focusing only on the paths leading to and from a specific page. The main goal of the application is to understand how customers get to a certain destination (a page) and what they do after. The data visualization cues help understand the paths with the most traffic (visits) and most engagement value per visit, allowing pinpointing good and bad paths. You can drill down to a particular path and explore path details.

## How to read the visualization {#map-key}
The visualization places the currently selected page at the center (shown as a large circle with the page icon) and shows all paths leading in and out of it.

The Landings area shows how many paths started with the currently selected page.

The Exits area shows the number of exits at the currently selected page and total accumulated [Exit value potential](#exit-value-potential).

The horizontal lines that are flowing into the currently selected page represent the incoming paths. The circles placed on top of the lines represent [nodes](#node) on that path. Nodes generally translate to pages.

The horizontal lines that are flowing from the currently selected page to the right represent the outgoing paths.

The circles placed on top of the lines represent [nodes](#node) on that path. Nodes generally translate to pages. In order to simplify the visualization, only the first page is shown on outgoing paths.

The linethickness defines the total [visits](#visits) to the currently selected page from the path. The thicker the path, the more visits are going to the selected page for a given path.

The line color defines the [value per visit](#value-per-visit) on this path to the currently selected page. The greener the path, the higher value per visit is comparing to other paths leading into the currently selected page. Paths with the least value per visit are shown in red color.

The size of the circle defines the total engagement value on the path that leads to the currently selected page. The larger the circle, the higher the [engagement value](#value) is.

The Context Pane area shows the aggregated totals for the visits, value and value per visit metrics, as well as the total path count. If you are hovering over a particular path, the totals area will show the metrics from that path.

## Map selector {#map-selector}
You can select various [maps](#map) using the Map selector control. You can also
choose to see more map metadata, and add a map to your favorites list,
which will automatically be saved to your profile.

### Group map data {#group-map-data}

Since each node has a corresponding item in the content (master) database,
using the Map selector's Group map data checkbox, you can request a map
having nodes grouped by the Sitecore data template (i.e. item type) from
which they were created.

For example, you can group these two paths:

- Home -&gt; TVs -&gt; 50" flat screen TV

- Home -&gt; Tablets -&gt; 12" tablet

into a single path by selecting **Group map data** in the **Map
selector** dialog.

- Landing Page -&gt; Product Category Page -&gt; Product Detail page

Grouping map data is useful when you'd like to perform path analysis on
page category level vs. individual page level.

## Date range selector {#date-selector}
You can select a date range using the date range selector either by
selecting individual start and end dates from the calendars or by
choosing one of the pre-defined date ranges.

### Dates missing data {#date-selector-missing-dates}
There may be cases where a map has no available data for some dates,
even if there are available data before or after these dates. This may
be due to no interactions recorded for a date, or an error occurred
during data processing and dates involved in the error were skipped. The
date range selector highlights dates for which no data are available.
Please contact your system administrator if you encounter many dates in
the calendar with no available data.

### Unavailable dates {#date-selector-unavailable-dates}
Depending on the date range that you have selected, some dates can be
marked as unavailable for selection. For example, when you select an end
date, all dates prior to the current start date are marked as
unavailable.

## Metrics filter {#metrics-filter}

Focuses on filtering nodes by their key metrics: visits, value, value
per visit and exit value potential. You can use the Metrics filter to reduce the noise or to find interesting
correlations between different metrics and for finding path optimization
candidates, for example:

- High value per visit, but low visits (more engagement value to be gained)
- High [Exit value potential](#exit-value-potential), but low visits (more engagement value to be gained)
- High visits, but low value (indicative of engagement value leakage)

## Application messages {#application-messages}
Throughout application usage, you may see various messages in the
message bar.
### "Some paths are hidden. Use filter to see other paths." {#page-analyzer-hidden-paths}
The application only shows 10 paths at once. You can use Metrics filter to reduce the number of paths based on any metrics criteria.
### "Based on 500 paths out of X total." {#page-analyzer-maximum-paths}
Some pages like Home may have a massive amount of unique paths going through it. For the efficiency, the application only processes top 500 paths. You can pick a more segmented map or select a smaller date interval to address this.

### "The selected map is being built. You may see partial data." {#partial-map}
This message can be seen if the currently selected map was recently deployed but the process of building data for this map hasn't completed. Data for the newly deployed map should be available approximately 30 minutes after map deployment.

## Glossary {#glossary}

### Map {#map}

A map is a special marketing definition that describes how to build the data for path analysis. Page Analyzer uses map data, filters all paths to show only the ones that are going through the currently selected page. This filtered dataset is used for visualization.
You can switch to another map using [map selector](#map-selector). 

### Path {#path}

A path is a sequence of nodes. All paths shown in Page Analyzer are going through the currently selected page.

### Node {#node}

Nodes are elements on a path. For most maps, nodes essentially translate to other pages. There is a set of metrics that are stored on each node: value, visits, value per visit, exits, exit value, exit value per visit, average time spent and average monetary value.

### Visits metric {#visits}

The total aggregated visits on a given node. This includes visits metrics from all descendant
nodes.

### Value metric {#value}
The total aggregated engagement value on a given node. This includes value metrics from all descendant nodes.

### Value per visit metric {#value-per-visit}

The aggregated engagement value per visit on a given node. This metric
is instrumental in calculating Exit value potential.

### Exits metric {#exits}

The total amount of exits on a given node. This metric identifies
whether a given node comprises a full path vs. entry path. Any node with
Exits greater than zero comprises a full path. This metric is
instrumental in calculating Exit value potential.

### Exit value metric {#exit-value}

The aggregated engagement value on a given node before exiting. Only nodes where exits
occurred have this metric. The difference between this metric and Value
metric, is that this metric doesn't take into account engagement value
of the descendant nodes.

### Exit value per visit metric {#exit-value-per-visit}
The aggregated engagement value per visit on a given node before exiting. Only nodes
where exits occurred have this metric calculated. The difference between
this metric and Value per visit metric, is that this metric doesn't
account for engagement value per visit of the descendant nodes. This
metric is instrumental in calculating Exit value potential.

### Exit value potential metric {#exit-value-potential}

The exit potential indicates projected engagement value that could be
gained on average through optimization. Consider it an advanced bounce
metric, where the engagement value loss (value leakage) is also taken
into account besides just exits. Knowing how much value per visit is
aggregated on all paths further down (Value per visit metric) and how
much value per visit is stored on the exit node, this metric can be
calculated by taking the delta between the two and multiplying by the
number of exits, using the following formula:

(Value per visit - Exit value per visit) \* Exits