# Getting started with Path Analyzer {#intro}
The Path Analyzer lets you analyze the paths that customers take as they interact with your brand, 
focusing on identifying the most efficient and least efficient paths, 
and paths with potential for optimizations.
You can analyze the paths that customers take through particular 
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels" target="_blank">channels</a> (email marketing, social, and so on), while interacting with <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity" target="_blank">campaigns</a>, 
and on their way to converting business critical activities, such as 
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals" target="_blank">goals</a>, 
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events" target="_blank">events</a>, and 
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">outcomes</a>.

## Key scenarios {#scenarios}

### 1. Exploring the map {#scenario1}

[Understanding the key visualization cues](#map-key) and data behind them is important to be able to read any map effectively and spot patterns.
The features listed below are useful as you begin your path analysis, 
especially if it's your first time using the application and you are not sure where to start.

[Reports feature](#reports), available from the Context Pane, helps to quickly highlight paths in any given report category.
For example, if you'd like to see all paths that don't generate any [engagement value](#value), 
simply pick the "Paths without value" category and click through the top 10 paths.
There are [8 total report categories](#reports) to explore.

[Dashboard view](#dashboard) is useful if you are just getting started with path analysis and 
are not comfortable with [other map views](#map-views) yet.
In the Dashboard view, you can see: [Map KPIs](#map-kpis); [Top path entries](#top-path-entries); 
and [Featured path](#featured-path); and you can access [Reports](#reports) and [Funnels](#funnels) features.

[Table view](#table-view) is another great way to start with path analysis.
It uses a very familiar Excel-like visualization showing all paths and their key metrics, 
and allows sorting and filtering.

[Metrics filter](#metrics-filter), available from all views except for the Dashboard, 
lets you focus on paths based on a particular set of metrics.
You can use the filter to display a map of paths with high [value](#value) but low [visits](#visits), 
paths with high [value per visit](#value-per-visit), 
or paths with high [exit value potential](#exit-value-potential).
In this way, you can filter the map to show good paths, bad paths, and paths for optimization.

### 2. Exploring paths from or to a particular page {#scenario2}

If you know the name of a particular page, 
Path Analyzer can easily show all paths leading in and out of this page by using the [Path filter](#path-filter) 
to build a path based on the name of the page.
If you have a destination page in mind, you can include it in the path filter in order to get all paths from page A to page B.
For [Experience maps](#experience-maps), you can use this technique to filter paths leading to a goal.

Similar to the [Scenario #1](#scenario1), you can use the [Metrics filter](#metrics-filter) 
to further refine a filtered map based on any combination of key metrics.

After you apply the filter, you can either explore various views by
[reading](#map-key) the filtered map, or leverage the [Reports feature](#reports) to quickly
navigate the top 10 paths in any given [report category](#reports).
The reports only show paths that match the applied [Path filter](#path-filter) and [Metrics filter](#metrics-filter).

### 3. Macro-level path analysis (goals, events, outcomes) {#scenario3}

When page-level maps provide too much detail, 
[Experience maps](#experience-maps) are often helpful to understand path analysis at a macro-level, focusing on
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels" target="_blank">channels</a>, <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity" target="_blank">campaigns</a>, <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals" target="_blank">goals</a>, <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events" target="_blank">events</a>, and <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">outcomes</a>.

### 4. Exploring a campaign or channel traffic {#scenario4}

If you'd like to understand how your customers interact with your brand through a particular 
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels" target="_blank">channel</a> or <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity" target="_blank">campaign</a>, you can pick one of the standard [Channel maps](#channel-maps) using the [Map selector](#map-selector), or [create and deploy](#how-to-create-a-new-map) a new [Campaign map](#campaign-maps) focusing on the campaign of interest. You can also use [Experience maps](#experience-maps) like in [Scenario #3](#scenario3), and use the [Path filter](#path-filter) to show only the paths from a particular channel or campaign.

### 5. Exploring a map focused on a particular segment {#scenario5}

In order to explore paths from a particular customer segment, [create a
new map](#how-to-create-a-new-map) then specify your segment rules in the Filter field using the familiar <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/the_rule_set_editor" target="_blank">Rule Set Editor</a> interface.
After the new map is deployed, you can select it in the Map selector and explore it the same way you would explore the default maps.

### 6. Exploring paths leading to a goal {#scenario6}

One way to explore paths leading to a given goal is to use the default
[Experience map with goals](#experience-maps) and specify the goal
in the [Path filter](#path-filter).

Another way is to [create and deploy](#how-to-create-a-new-map) a new [Goal map](#goal-maps), 
which will focus only on the paths toward the specified goal.
You can use the same technique to explore paths to certain assets or outcomes.

## Maps {#maps}

A map is a special marketing definition for path analysis that has two
key attributes: map type and map filter. Map type describes how to build
data that powers the map, and is covered in more detail
[here](#map-types). Map filter, an optional but important attribute,
helps define a segmented map using the <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/the_rule_set_editor" target="_blank">Rule Set Editor</a> and a rich set of conditions.

In addition to these two key attributes, each map has a unique identifier, name
and type. You can also include other optional attributes, such as
description.

Similar to other marketing definition items, you [create a map in the Marketing Control Panel](#how-to-create-a-new-map).

Maps are visualized using [Map views](#map-views).

## Map types {#map-types}

Map type prescribes how the interaction data from xDB will be
transformed for path analysis. There are different map types available by default.

### Page maps {#page-maps}

These maps are built from sequences of page visits within a given interaction.
There are a few subtypes for Page maps available by default.
These map subtypes are convenient because 
they quickly let you create a page map focused on a particular interaction attribute (channel, campaign, goal, asset, and so on).

#### Goal maps {#goal-maps}

Goal maps let you create a page map leading to a particular goal.
Goal maps disregard pages that were visited after a particular goal was reached.

You can build Goal maps in reverse mode by selecting the Reverse checkbox 
on the Goal map definition item in the Marketing Control Panel.
A reverse goal map flips the sequence of pages leading to a particular goal and 
uses the selected goal as the starting point of the map instead of the conventional [Internet node](#internet-node).

#### Asset maps {#asset-maps}

Asset maps let you create a page map leading to a particular asset download.
Asset maps disregard pages that were visited after a particular asset was downloaded.

You can build Asset maps in reverse mode by selecting the Reverse checkbox on the Asset map definition item in the Marketing Control Panel.
A reverse asset map flips the sequence of pages leading to a particular asset download and 
uses the selected asset as the starting point of the map instead of the conventional [Internet node](#internet-node).

#### Campaign maps {#campaign-maps}

Campaign maps let you create a page map for all interactions from a particular campaign.

#### Channel maps {#channel-maps}

Channel maps let you create a page map for all interactions from a particular channel.

#### Outcome maps {#outcome-maps}

Outcome maps let you create a page map leading to a particular outcome.

### Experience maps {#experience-maps}

Unlike the Page maps, Experience maps can include other interaction attributes, such as 
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/channels/channels" target="_blank">channels</a>, 
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/campaigns/create_and_edit_a_campaign_activity" target="_blank">campaigns</a>, 
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/campaigns/goals__events/goals" target="_blank">goals</a>, 
<a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/engagement_plans/events" target="_blank">events</a>, and 
<a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">outcomes</a>, 
in addition to pages.
You select these interaction attributes using the checkbox options on the Experience map definition item in the Marketing Control Panel.
In this way, Experience maps enable you to focus on more high level path analysis than the more detailed [Page maps](#page-maps).

Three Experience maps are available by default:

- Experience map with goals. Includes channel, campaign (if available), all goals, and outcomes.

- Experience map with value goals only. Same as above except that only goals with engagement value are added.

- Experience map with page events. Includes channel, campaign (if available), only the entry and exit page, all page events, and outcomes.

You can easily [create a new map](#how-to-create-a-new-map) based on any existing map using the Marketing Control Panel.

### Site-specific maps {#site-specific-maps}
In addition to map types, maps can either be **global** or **site-specific**. Global maps are built for all sites, while site-specific maps are only built for a particular site. Whether a map is global or site-specific is determined by the location of the
map within the Path Analyzer's content tree in the Marketing Control Panel. All global maps are placed in the */Maps/Default maps/Global maps* folder and all site-specific maps are
placed in the */Maps/Default maps/Site maps* folder.

### Custom maps {#custom-maps}

If there are any custom maps registered, which typically requires minor development effort, you can find them in the  */Maps/Custom maps* folder.

### How to create a new map {#how-to-create-a-new-map}

To create a brand new map:

1. Open the Marketing Control Panel from Launchpad.

2. Navigate to the Path Analyzer item.

3. Expand the Maps item underneath Path Analyzer.

4. Select the appropriate folder for your new map based on the available map types described above.

5. Create a new map item.

6. Specify the required attributes and any optional attributes for your map.

7. Save the map item.

8. Deploy the new map using the Deploy workflow command on the Review tab.

Historic and live data for the map will begin building approximately 30 minutes after deployment.

## Map selector {#map-selector}

You can select various maps using the Map selector control.
You can also see more map meta-data and add a map to your favorites list, which will automatically be saved to your profile.

### Group map data {#group-map-data}

Maps are powered by [tree data structures](#tree) that consist of [nodes](#node).
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

## Map key {#map-key}

The following map key applies to the Radial, Horizontal, and Vertical tree views.

When you read a map, the size and color of the circles and the lines between nodes on the map represent information about which paths provide higher [engagement value](#value), 
higher [value per visit](#value-per-visit) or are the most [visited](#visits).

Circles represent [nodes](#node). Depending on the selected map type, nodes may represent pages, goals, or other marketing activities. Circles have
the following two visual properties providing information about the node: size and color.

The size of a circle indicates the total [engagement value](#value) of a [node](#node) and all its descendants.
In other words, a larger node represents a larger total [engagement value](#value).

The color of a circle indicates the [value per visit](#value-per-visit) of a [node](#node) compared to the value per visit of its parent and 
it helps you spot the change in this metric when looking further down the path.
If a circle becomes red, then the [value per visit](#value-per-visit) has decreased at this [node](#node).
If a circle becomes greener than its parent, then the [value per visit](#value-per-visit) has increased at this [node](#node).
Circle color also helps you compare the [value per visit](#value-per-visit) metric between sibling nodes and 
determine where the highest [value per visit](#value-per-visit) paths continue from a given [node](#node).

Circles with a thick dark gray border represent special "[other nodes](#other-nodes)".

Lines connecting the map nodes represent paths between [node](#node) A and [node](#node) B. Lines have the following visual properties providing information about the [path](#path): thickness and partial shading.

The thickness of a line indicates how many [visits](#visits) (traffic) went from [node](#node) A to [node](#node) B compared to the siblings of [node](#node) B, 
which allows for easy identification of high traffic paths.

A partial shading of a line is complementary to line thickness and is used to represent path visits at deeper levels, where it is more
difficult to see differences in line thickness.

As a general guideline, look for thick lines with either small or red
circles, indicating a high volume of [visits](#visits) to paths that have low
[engagement value](#value) (size) and low [value per visit](#value-per-visit) (color), respectively.

### Other nodes {#other-nodes}

Due to the limitations of tree views (Radial, Horizontal and Vertical)
when visualizing large maps with extreme fanouts, less significant
nodes that cannot fit at a particular level of the visualization are combined
into a special "other" node. The [Table view](#table-view) does not have this
limitation.

You can see the list of nodes that were combined into "Other nodes" by
selecting the Next tab on the Context Pane or selecting the Others
tab within the node popover.

Applying either a [Path filter](#path-filter) or a [Metrics filter](#metrics-filter) usually helps reduce the
number of "Other nodes" shown on a map.

## Map views {#map-views}

There are five different views available to choose from for analyzing your maps.
Dashboard is a default view that provides introductory insights to path analysis and is described [below](#dashboard).

### Radial view {#radial-view}
Radial view has an advantage of being able to fit more map data on the screen but
is not ideal for smaller maps or filtered maps.
The [Internet node](#internet-node) is at the center on this view.

### Vertical view {#vertical-view}
Vertical view is much better at representing smaller maps or filtered maps and usually provides better readability
compared to the [Radial view](#radial-view). The [Internet node](#internet-node) can be found at the very top on this view.

### Horizontal view {#horizontal-view}
Similar to Vertical view, Horizontal view is good for smaller maps and usually provides better readability 
compared to the [Radial view](#radial-view).
The [Internet node](#internet-node) can be found at the far left side.

### Table view {#table-view}
Table view is different because it only shows [full paths](#path), 
which is due to the map data being a [tree structure](#tree) that cannot be easily viewed as a table.

## Dashboard {#dashboard}

Dashboard is a special view that provides introductory insights to path analysis.

### Map KPIs  {#map-kpis}
There are six Key Performance Indicators (KPI) available on the dashboard
by default for the following metrics: [visits](#visits), [value](#value), [value per visit](#value-per-visit), 
and optional outcome metrics: [monetary value](#monetary-value), [outcomes](#outcomes), and [average monetary value](#average-monetary-value).

Outcome metrics are not shown by default and can be enabled from [Application
Settings](#application-settings).

Each map KPI has a trend indicator showing the increase or decrease of a
metric compared with the same metric over the same date interval for the
same map in the past. For example, if the currently selected date range
is today, the trend indicator will be based on the data from yesterday.

### Top path entries {#top-path-entries}

This list shows the top 10 path starting points on the current map.
In Path Analyzer terminology, these are the top 10 [nodes](#node) on the first level,
sorted by combined [value](#value) and [visits](#visits) metrics.

### Featured path {#featured-path}

The Featured path displays the path from the currently selected map with the most interesting
set of key marketing metrics. Featured path selection is based on an
algorithm that takes into account either [exit value
potential](#exit-value-potential) or combined [value](#value) and [visits](#visits), then selects the top path in either metric category.
Because the opportunity for optimization is relatively limited for short paths, the algorithm will prioritize the longest paths.

### Favorite funnel {#favorite-funnel}

A Favorite funnel is a funnel that was marked as favorite on a particular map. This can be changed at any time on the Context Pane under Funnels. A Favorite funnel is saved in your user profile and is associated with the map from which it was marked as favorite.

## Reports {#reports}

The Path Analyzer reports show top paths in various categories.
Reports provide an introduction to the most interesting paths in the currently selected map, enabling you to quickly identify of good and bad paths.
By default, there are eight report categories available.
Up to 10 paths are available for selection in each category.

### Highest visited {#highest-visited-report}
The paths with the highest [visits](#visits).

### Highest valuable {#highest-valuable-report}
The paths that generate the highest [engagement value](#value).

### Highest visits and value {#highest-visitsvalue-report}
The paths that generate the highest [engagement value](#value) and the highest [visits](#visits).

### Highest value per visit {#highest-valuepervisit-report}
The paths that generate the highest [value per visit](#value-per-visit).

### Paths without value {#paths-without-value-report}
The paths where customers exited without generating any [engagement value](#value).

### Highest exit value potential {#highest-evp-report}
The paths that generate the highest [exit value potential](#exit-value-potential).

### Highest outcomes {#highest-outcomes-report}
The paths that generate the highest number of [outcomes](#outcomes).

### Highest monetary value {#highest-monetaryvalue-report}
The paths that generate the highest total [monetary value](#monetary-value), which comes from outcomes.

## Funnels {#funnels}

A funnel is a well-defined sequence of steps that customers are expected
to take on their way to realizing a business objective. Businesses
define their own funnel. For an e-commerce site, it is likely a checkout
funnel, which could be represented as a sequence of pages, page events
or goals, depending on the implementation specifics.

Funnels in Path Analyzer enable you to analyze the actions and paths
that customers take on their way to converting goals and outcomes. You
can then optimize the paths to improve conversion rates, for example, 
by implementing <a href="https://doc.sitecore.net/sitecore_experience_platform/digital_marketing/personalization/personalization" target="_blank">personalization</a>,
<a href="https://doc.sitecore.net/sitecore_experience_platform/analyzing__reporting/experience_optimization__content_testing/ab_and_multivariate_testing" target="_blank">M/V testing</a>,
or <a href="https://doc.sitecore.net/sitecore_experience_platform/analyzing__reporting/experience_optimization__content_testing" target="_blank">content testing</a>.

The Funnels feature is available from the Context Pane, where you can select and explore a funnel that is defined in the Marketing Control Panel.

After a funnel is selected, you can view a graphical representation of
the tracked steps from a funnel within Path Analyzer in the form of a
bar chart. The chart provides you with information about the number of
customers who complete each step in the funnel, as well as how many
customers continue to the next stage. It also lets you switch between key metrics, such as [visits](#visits), [value](#value), and [value per visit](#value-per-visit).
Below the chart, the list of all other metrics is shown, providing the key performance indicators for the funnel. These metrics are taken from the last step of the funnel.
This data is calculated based on the scope of an interaction as opposed to the lifetime customer journey.

Any funnel can be marked as favorite by clicking the star icon next to the funnel name.
This action will make the funnel visible on the [Dashboard view](#dashboard).

To save any selected path as a funnel, click Save as funnel in the footer area of the Context Pane.

## Map filters {#map-filters}

There are two types of filters available that let you focus on certain paths.

### Path filter {#path-filter}

Path filter enables you to filter a map based on the name of a node, which could either be a page, a goal, 
or any other marketing attribute depending on the type of the current map.
For example, you can use Path filter to learn how customers arrive at a page of interest.
Simply set a particular page as an element of the Path filter and click Apply.
The map will adjust accordingly.

Path filter lets you build a map filter from Page A to Page B as well.
Usually, you won't require more than three elements in the Path filter, but you can specify any number of elements there.
The Path filter narrows down the list of options based on the available data in the current map.

### Metrics filter {#metrics-filter}

This filter focuses on filtering nodes by their key metrics: [visits](#visits), [value](#value), [value
per visit](#value-per-visit), and [exit value potential](#exit-value-potential).

Because of its secondary nature to the main [Path filter](#path-filter), the Metrics filter is able to show how many matches
for the current [Path filter](#path-filter) there are, as well as the correlation between different metrics.
Also, you can use the Metrics filter without the [Path filter](#path-filter) and filter out the less visited nodes, 
which reduces noise on the current map.

Finally, the Metrics filter lets you find interesting correlations between different metrics and for finding path optimization candidates, for example:

- High [visits](#visits), but low [value](#value).

- High [value per visit](#value-per-visit), but low [visits](#visits).

- High [exit value potential](#exit-value-potential).

## Export a map {#export-map}

You can export data for any map as a comma separated dataset using the
following two commands from the Action Menu:

- Download as CSV

- Copy to clipboard

Both commands operate using the same format and exist to enable
different export workflows.

## Application messages {#application-messages}

When using the application, you can see various messages in the message bar.

### "Table view shows top X paths out of Y total." {#table-top}
This message can be seen when the [Table view](#table-view) is rendering extremely
large maps. The [Table view](#table-view) is able to show only the top 500 [full
paths](#path). Suggested actions for this message are: use either the
[Path filter](#path-filter) or the [Metrics filter](#metrics-filter) to decrease the number of visible
rows; decrease the date range interval for the map; or [create](#how-to-create-a-new-map) or [select](#map-selector) a
filtered map that has less data.

### "X less significant nodes were grouped together with other nodes." {#other-nodes-message}
This message can be seen using either the Radial, Horizontal, or Vertical
view on large maps with extreme fanouts. To ensure the map is readable,
less significant nodes that cannot fit at a particular level of the visualization
are combined into a special 'other' node. Note that the [Table view](#table-view) does
not have this limitation. Suggested actions for this message are: use
either the [Path filter](#path-filter) or the [Metrics filter](#metrics-filter) to decrease the number of
visible nodes; decrease the date range interval for the map; or [create](#how-to-create-a-new-map) or [select](#map-selector) a
filtered map that has less data.

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

These settings are available from the Action Menu, under Settings.

## Glossary {#glossary}

### Map {#map}

A special marketing definition that describes how to build data for path analysis.
Each deployed map has a [tree](#tree) stored in the reporting database.

### Tree {#tree}

The aggregated data structure for path analysis that is stored in a reporting database for each
deployed map consisting of a hierarchy of [nodes](#node).
Any tree must have a special root node, which is called an [Internet node](#internet-node).

### Node {#node}

The key element of the [tree](#tree).
All nodes, except for the [Internet node](#internet-node), have a parent node and can have child nodes.
Depending on the [map type](#map-types), a node can either represent a page (on a [Page map](#page-maps)), 
or a goal, or any other marketing attribute (channel, campaign, and so on) on an [Experience map](#experience-maps).

Each node has a unique numeric ID, name, and a GUID that corresponds to an item from the content database.

There are different kinds of metrics stored on each node: 

- **Aggregated metrics**, including [value](#value), [visits](#visits), [average time spent](#average-time-spent), [outcomes](#outcomes), and [monetary value](#monetary-value).
These metrics include values from all descendant nodes.

- **Exit metrics**, including [exits](#exits) and [exit value](#exit-value).
These metrics do not include values from all descendant nodes and are only calculated if the current node is an [Exit node](#exit-node).

- **Calculated metrics**, including [value per visit](#value-per-visit), [exit value per visit](#exit-value-per-visit), [average monetary value](#average-monetary-value), and [exit value potential](#exit-value-potential).

### Exit node {#exit-node}

Node with [exits](#exits) greater than zero, indicating the number of [visits](#visits) that terminated on this node.

### Internet node {#internet-node}

The special root [node](#node) that serves as a starting node for all [paths](#path), 
and aggregates all key metrics from all paths on the given [map](#map).

### Path {#path}

A sequence of [nodes](#node) make up a path. Because of the aggregated nature of
the [tree](#tree), it's important to differentiate between two kinds of paths:
**entry path** and **full path**.

A **full path** consists of an entire visit, from the entry node to the [exit node](#exit-node).
An **entry path**, however, doesn't have to end with an exit.
It's important to understand the difference between the two kinds of paths, 
because the [Table view](#map-views) and the [Reports feature](#reports) only work with full paths.

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

### Outcomes metric {#outcomes}

The total number of outcomes realized on a given node. This includes
outcomes from all descendant nodes.
Learn more about outcomes <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">here</a>.

### Monetary value metric {#monetary-value}

The total amount of monetary value gained on a given [node](#node). The monetary
value is retrieved from realized outcomes. This includes monetary value
from all descendant nodes.
Learn more about outcomes <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">here</a>.

### Average monetary value metric {#average-monetary-value}

The average monetary value gained per outcome on a given [node](#node). The
monetary value is retrieved from realized outcomes. This includes
average monetary value from all descendant nodes.
Learn more about outcomes <a href="https://doc.sitecore.net/sitecore_experience_platform/developing/marketing_operations/outcomes/outcomes" target="_blank">here</a>.

### Average time spent metric {#average-time-spent}

The average amount of time customers spent on a given [node](#node) in seconds.