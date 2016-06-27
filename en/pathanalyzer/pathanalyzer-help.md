# Getting started with Path Analyzer {#intro}
The Path Analyzer lets you analyze the paths that customers take as they
interact with your brand, focusing on identification of the most
efficient and least efficient paths and paths with potential for
optimizations. You can analyze the paths that customers take while
interacting with campaigns, and on their way to converting on business
critical activities such as goals and outcomes.

## Key scenarios {#scenarios}

### 1. Exploring the map {#scenario1}

[Understanding the key visualization cues](#map-key) and data behind
those cues is important to be able to read any map effectively and spot
patterns. The features listed below will be useful as you begin your
path analysis, especially if it's your first time using the application
and you are not sure where to start.

Reports feature, available from the Context Pane, helps quickly
highlight paths in any given report category. For example, if you'd like
to see all paths that don't generate any engagement value, simply pick
the "Paths without value" category and page through the top 10 paths.
There are [8 total report categories](#reports) to explore.

[Dashboard view](#dashboard) can be useful if you are just getting
started with path analysis and are not comfortable with [other map
views](#map-views) yet. In the Dashboard view, you can see: [map
KPIs](#map-kpis); [top path entries](#top-path-entries); [Featured
path](#featured-path); and access [Reports](#reports) and
[Funnels](#funnels) features.

Table view is another great way to start with path analysis. It uses a
very familiar Excel-like visualization showing all paths and their key
metrics, and allows sorting and filtering.

[Metrics filter](#metrics-filter), available from all views except for
the Dashboard, allows focusing on paths based on a particular set of
metrics. You can use the filter to display a map of paths with high
[value](#value) but low [visits](#visits), paths with
high [value per visit](#value-per-visit), or paths with high [Exit
value potential](#exit-value-potential). This way you can filter the
map to show good paths, bad paths, and paths for optimization.

### 2. Exploring paths from or to a particular page {#scenario2}

If you know the name of a particular page, Path Analyzer can easily show
all paths leading in and out of this page by using the [Path
filter](#path-filter) to build a path based on the name of the page. If
you have a destination page in mind, you can include it in the path
filter in order to get all paths from page A to page B. Page is used as
an example here. For [Experience maps](#experience-maps), you can use
this technique to filter paths leading to a goal.

Optionally, you can use the Metrics filter described in [Scenario 1](#scenario1) to
further refine a filtered map based on any combination of key metrics.
After you apply a path filter, you can either explore various views by
reading the filtered map, or leverage the Reports feature to quickly
navigate top 10 paths in any given [report category](#reports). The
reports will only show paths that match the applied path filter.

### 3. Macro-level path analysis (goals, events, outcomes) {#scenario3}

When page-level maps provide too much detail, [Experience
Maps](#experience-maps) are often helpful to understand path analysis
at a macro-level, focusing on channels, campaigns, goals, page events or
outcomes.

### 4. Exploring a campaign or channel traffic {#scenario4}

If you'd like to understand how your customers interact with your brand
via a particular channel or campaign, you can pick one of the standard
[Channel maps](#channel-maps) using the [Map selector](#map-selector),
or [create and deploy](#how-to-create-a-new-map) a new [Campaign
map](#campaign-maps) focusing on the campaign of interest. You can also
use Experience maps like in scenario 3, and use the [Path
filter](#path-filter) to show only the paths from a particular channel
or campaign.

### 5. Exploring map focused on particular segment {#scenario5}

In order to explore paths from a particular customer segment, create a
new map then specify your segment rules in the Filter field using the
familiar Rule Editor interface. After the new map is deployed, you will
be able to see it in the Map selector and explore it the same way you
would explore the default maps. Learn more about the process of creating
and deploying a new map [here](#how-to-create-a-new-map).

### 6. Exploring paths leading to a goal {#scenario6}

One way to explore paths leading to a goal is to use the default
[Experience map with goals](#experience-maps) map and specify the goal
in [Path filter](#path-filter) to see paths towards a given goal.
Another way is to [create and deploy](#how-to-create-a-new-map) a new
[Goal map](#goal-maps), which will focus only on the paths towards the
specified goal. You can use the same technique to explore paths to
certain assets or outcomes.

## Maps {#maps}

A map is a special marketing definition for path analysis that has two
key attributes: map type and map filter. Map type describes how to build
data that powers the map, and is covered in more detail
[here](#map-types). Map filter, an optional but important attribute,
helps define a segmented map using the Rule Editor based on a rich set
of conditions.

Besides these two key attributes, each map has a unique identifier, name
and type. You can also include other optional attributes, such as
description.

You create a map in Marketing Control Panel and, similar to other
marketing definition items, must deploy it by using a workflow. After
the map is deployed, Path Analyzer will start building data for the map,
which will result in aggregated tree datasets available for further
analysis within the application.

Maps are visualized via [Map views](#map-views).

## Map types {#map-types}

Map type prescribes how the interaction data from xDB will be
transformed into a tree structure for path analysis. There are different
map types available by default.

### Page maps {#page-maps}

These maps are built from sequences of page visits within a given
interaction. There are a few sub-types for Page maps available by
default. These map sub-types exist for convenience - quickly allowing
the creation of a map focused on a particular interaction attribute and
simplifying the process of map creation.

### Goal maps {#goal-maps}

Goal maps allow for the creation of a page map leading to a particular
goal. Goal maps will disregard pages that were visited after a
particular goal was reached.

Goal maps can be built in reverse mode by toggling the Reverse checkbox
on the Goal map definition item in Marketing Control Panel. A reverse
goal map will flip the sequence of pages leading to a particular goal
and use the selected goal as the starting point of the map instead of
the conventional Internet node.

### Asset maps {#asset-maps}

Asset maps allow for the creation of a page map leading to a particular asset download. Asset
maps will disregard pages that were visited after a particular asset was
downloaded.

Asset maps can be built in reverse mode by toggling tge Reverse checkbox
on the Asset map definition item in Marketing Control Panel. A reverse
asset map will flip the sequence of pages leading to a particular asset
download and use the selected asset as the starting point of the map
instead of the conventional Internet node.

### Campaign maps {#campaign-maps}

Campaign maps allow for
the creation of a page map for all interactions from a particular
campaign.

### Channel maps {#channel-maps}

Channel maps allow for the creation of a page map for all interactions
from a particular channel.

### Outcome maps {#outcome-maps}

Outcome maps allow for
the creation of a page map leading to a particular outcome. Outcome maps
will disregard pages that were visited after a particular outcome was
realized.

### Experience maps {#experience-maps}

Experience maps can include multiple interaction attributes such as
channels, campaigns, goals, page events and outcomes. Interaction
attributes can be selected using the checkbox options on the Experience
map definition item in the Marketing Control Panel.

Three Experience maps are available by default:

- Experience map with goals. Includes channel, campaign (if available), all goals and outcomes.

- Experience map with value goals only. Same as above except that only goals with engagement value are added.

- Experience map with page events. Includes channel, campaign (if available), only the entry and exit page, all page events and outcomes.

You can easily [create a new map](#how-to-create-a-new-map) based on any existing map using Marketing Control Panel.

In addition to map types, maps can either be global
or site-specific. Global maps are built for all sites, while
site-specific maps are only built for a particular site. Whether a
map is global or site-specific is determined by the location of the
map within the Sitecore content tree. All global maps are placed
under /Maps/Default maps/Global maps and all site-specific maps are
placed under /Maps/Default maps/Site maps.

Custom maps may also be present in your Sitecore implementation,
depending on whether or not there were any custom maps registered -
which typically requires minor development effort.

### How to create a new map {#how-to-create-a-new-map}

Open Marketing Control
Panel from Launchpad and navigate to the Path Analyzer item. Expand the
Maps item underneath Path Analyzer, then select the appropriate folder
for your new map based on the available map types described above and
create a new map item. After specifying the required attributes and any
optional attributes for your map, save the map then deploy it via the
Deploy workflow command (available from the Review tab). Approximately
30 minutes after deployment, historic and live data for the map will
begin building.

## Map selector {#map-selector}

You can select various maps using the Map selector control. You can also
choose to see more map metadata, and add a map to your favorites list,
which will automatically be saved to your profile.

### Group map data {#group-map-data}

Maps are powered by tree data structures that consist of nodes. Because
each node has a corresponding item in the content (master) database,
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
selecting individual start and end dates from the calendars, or by
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

## Map key {#map-key}

The following keys apply to the Radial, Horizontal and Vertical views.

When you read a map, the size and color of the circles and the lines
between nodes on the map provide you with information about which paths
provide higher engagement value, provide higher value per visit or are
most visited.

Circles represent nodes. Depending on the selected map type, nodes may
represent pages, goals or other marketing activities. Circles have
visual properties providing information about the node.

Size of a circle indicates the total engagement value of a node and all
descendants of the node. In other words, a larger node represents larger
total engagement value.

Color of a circle indicates the value per visit of a node as compared to
the value per visit of its parent and helps spot the change in this
metric when looking further down the path. If a circle becomes red, then
the value per visit has decreased at this node. If a circle is a darker
shade of green than its parent, then value per visit has increased at
this node. Circle color also helps compare the value per visit metric
between sibling nodes and determine where highest value per visit paths
continue from a given node.

Circles with a thick dark grey border represent special "[Other
nodes](#other-nodes)".

Lines connecting the map nodes represent paths between node A and node
B. Lines have visual properties providing information about the path.

Thickness of a path line indicates how many visits (i.e. traffic) went
from node A to node B as compared to the siblings of node B, which
allows for easy identification of high traffic paths.

Partial shading of a path line is complementary to path thickness and is
used to represent path visits at deeper map levels where it may be more
difficult to see differences in line thickness.

As a general guideline, look for thick paths with either small or red
nodes, indicating a high volume of visits to paths that have low
engagement value and low value per visit, respectively.

### Other nodes {#other-nodes}

Due to the limitations of tree views (Radial, Horizontal and Vertical)
when visualizing large maps with extreme fan outs, less significant
nodes that cannot fit at a particular level of the tree are combined
into a special "other" node. The Table view does not have this
limitation.

You can see the list of nodes that were combined into "Other nodes" by
selecting the Next tab within the Context Pane or selecting the Others
tab within the node popover.

Applying either Path filter or Metrics filter usually helps reduce the
number of "Other nodes" shown on a map.

## Map views {#map-views}

Five views are available to choose from for analyzing your maps.

-   Radial

-   Vertical

-   Horizontal

-   Table

-   Dashboard

Radial view has an advantage of being able to fit more map data on the
screen but is not ideal for smaller maps or filtered maps.

Vertical and Horizontal map views are much better at representing
smaller maps or filtered maps and usually provide better readability
compared to the Radial view.

Table view is rather different as it only shows only [full
paths](#path), which is due to map data being a tree structure that
isn't represented well by a flat table.

Dashboard is a special view described separately [below](#dashboard).

## Dashboard {#dashboard}

Dashboard is a special view that provides introductory insights to path analysis.

### Map KPIs  {#map-kpis}
There are 6 Key Performance Indicators (KPI) available on the dashboard
by default for the following metrics: visits, value, value per visit and
optional outcome metrics: monetary value, outcomes and average monetary
value.

Outcome metrics are not shown by default, and can be enabled from [Application
Settings](#application-settings).

Each map KPI has a trend indicator showing the increase or decrease of a
metric compared with the same metric over the same date interval for the
same map in the past. For example, if the currently selected date range
is today, the trend indicator will be based on the data from yesterday.

### Top path entries {#top-path-entries}

This list shows the top 10 path starting points on the current map. In Path Analyzer
terminology, these are the top 10 [nodes](#node) on the first level, sorted by combined value plus visits metrics.

### Featured path {#featured-path}

Shows the path from the currently selected map with the most interesting
set of key marketing metrics. Featured path selection is based on an
algorithm that takes into account either [exit value
potential](#exit-value-potential) or combined value and visits, then
selects the top path in either metric category. Because the opportunity
for optimization is relatively limited for short paths, the longest
paths in the selected metric category will be prioritized over short
paths.

### Favorite funnel {#favorite-funnel}

A funnel that was favorited on a particular map. This can be changed at any time from Context Pane /
Funnels. A Favorite funnel is saved in your user profile and is associated with the map from which it was favorited.

## Reports {#reports}

The Path Analyzer reports show top paths in various categories. Reports
provide an introduction to the most interesting paths in the currently
selected map, allowing for quick identification of good and bad paths.
By default, there are 8 report categories available. Up to 10 paths are
available for selection in each category.

### Highest visited {#highest-visited-report}
The paths with the highest visits

### Highest valuable {#highest-valuable-report}
The paths that generate the highest engagement value

### Highest visits and value {#highest-visitsvalue-report}
The paths that generate the highest engagement value and the highest visits

### Highest value per visit {#highest-valuepervisit-report}
### The paths that generate the highest value per visit

### Paths without value {#paths-without-value-report}
The paths where customers exited without any [engagement value](#value) generated.

### Highest exit value potential {#highest-evp-report}
The paths that generate the highest [exit value potential](#exit-value-potential).

### Highest outcomes {#highest-outcomes-report}
The paths that generate the highest number of [outcomes](#outcomes).

### Highest monetary value {#highest-monetaryvalue-report}
The paths that generate the highest total [monetary value](#monetary-value), which comes from outcomes

## Funnels {#funnels}

A funnel is a well-defined sequence of steps that customers are expected
to take on their way to realizing a business objective. Businesses
define their own funnel. For an e-commerce site, it is likely a checkout
funnel, which could be represented as a sequence of pages, page events
or goals, depending on the implementation specifics.

Funnels in Path Analyzer enable you to analyze the actions and paths
that customers take on their way to converting goals and outcomes. You
can then optimize the paths to improve conversion rates, for example, by
implementing personalization, M/V testing, or content testing.

The Funnels feature is available from within the Context Pane, and
allows selection and exploration of a funnel defined in Marketing
Control Panel.

After a funnel is selected, you can view a graphical representation of
the tracked steps from a funnel within Path Analyzer in the form of a
bar chart. The chart provides you with information about the number of
customers who complete each step in the funnel, as well as how many
customers continue to the next stage. Below the chart, the list of
metrics is shown, providing the key performance indicators for the
funnel. These metrics are taken from the last step of the funnel.

Any funnel can be marked as a favorite funnel for the currently selected
map by clicking the star icon next to the funnel name.

You can save any selected path as a funnel by clicking the "Save as
funnel" button in the footer area of the Context Pane.

## Map filters {#map-filters}

There are two types of filters available that allow you to focus on
certain paths.

### Path filter {#path-filter}

Allows you to filter a map based on the name of a node, which could
either be a page, a goal or any other marketing attribute depending on
the type of the current map. For example, you can use Path filter to
learn how customers move to a page of interest. Simply select a page in
path filter and click Apply. The map will adjust accordingly.

### Metrics filter {#metrics-filter}

Focuses on filtering nodes by their key metrics: visits, value, value
per visit and exit value potential. Because of its secondary nature to
the main Path filter, Metrics filter is able to show how many matches
for the current Path filter there are as well as the correlation between
different metrics. Also, you can use the Metrics filter without Path
filter and filter out less visited nodes, thus reducing noise on the
current map. Finally, Metrics filter allows for finding interesting
correlations between different metrics and for finding path optimization
candidates, for example:\
- High value per visit, but low visits (more engagement value to be
gained)

- High [Exit value potential](#exit-value-potential), but low visits
(more engagement value to be gained)

- High visits, but low value (indicative of engagement value leakage)

## Export a map {#export-map}

You can export data from any map as a comma separated dataset via the
following two commands from Action Menu:

- Download as CSV

- Copy to clipboard

Both commands operate using the same format and exist to enable
different export workflows.

## Application messages {#application-messages}

Throughout application usage, you may see various messages in the
message bar.

### "Table view shows top X paths out of Y total." {#table-top}
This message can be seen when the Table view is rendering extremely
large maps. The Table view is able to show only the top 500 [full
paths](#path). Suggested actions for this message are: use either the
Path filter or the Metrics filter to decrease the number of visible
rows; decrease the date range interval for the map; or create/use a
filtered map that has less data.

### "X less significant nodes were grouped together with other nodes." {#other-nodes-message}
This message can be seen using either the Radial, Horizontal or Vertical
view on large maps with extreme fan outs. To ensure the map is readable,
less significant nodes that cannot fit at a particular level of the tree
are combined into a special 'other' node. Note that the Table view does
not have this limitation. Suggested actions for this message are: use
either the Path filter or the Metrics filter to decrease the number of
visible rows; decrease the date range interval for the map; or
create/use a filtered map that has less data.

### "The selected map is being built. You may see partial data." {#partial-map}
This message can be seen if the currently selected map was recently deployed but the
process of building data for this map hasn't completed. Data for the newly deployed map should be available approximately 30 minutes after map deployment.

## Application settings {#application-settings}

Below is a list of application settings you can change in order to
customize your Path Analyzer application experience:

- Enable/disable transition effects

- Show/hide labels by default

- Show/hide legend by default

- Show/hide outcome metrics

- Show/hide help on startup

- Allow selection of dates missing data

These settings are available from the Action Menu -&gt; Settings.

## Glossary {#glossary}

### Map {#map}

Marketing definition that describes how to build data for path analysis.
Each deployed map has a tree stored in the database.

### Tree {#tree}

The aggregated data structure for path analysis that is stored for each
deployed map consisting of nodes and paths.

### Node {#node}

Nodes are the key elements of the tree. Depending on the map type, a
node can either represent a page (on a Page map), or a goal, or any
other marketing attribute (channel, campaign, etc.) on an Experience
map.

Each node has a unique id, name and a GUID that corresponds to an item
from the content database.

There is a set of metrics that are stored on each node: value, visits,
value per visit, exits, exit value, exit value per visit, average time
spent, outcomes, monetary value, and average monetary value.

### Path {#path}

A sequence of nodes make up a path. Because of the aggregated nature of
the tree, it's important to differentiate between two kinds of paths:
entry path and full path.

While a full path consists of an entire visit from the entry node to the
[exit node](#exit-node), an entry path doesn't necessarily terminate
with an exit node (node with Exits metric greater than 0).

### Internet node {#internet-node}

The special root node that serves as a starting node for all paths and
aggregates all key metrics from all paths on the given map.

### Exit node {#exit-node}

Node with Exits metric greater than zero, indicating the number of
visits that terminated on this node.

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

### Outcomes metric {#outcomes}

The total number of outcomes realized on a given node. This includes
outcomes from all descendant nodes.

### Monetary value metric {#monetary-value}

The total amount of monetary value gained on a given node. The monetary
value is retrieved from realized outcomes. This includes monetary value
from all descendant nodes.

### Average monetary value metric {#average-monetary-value}

The average monetary value gained per outcome on a given node. The
monetary value is retrieved from realized outcomes. This includes
average monetary value from all descendant nodes.

### Average time spent metric {#average-time-spent}

The average amount of time customers spent on a given node in seconds.