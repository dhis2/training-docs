# Event Reports - Session Summary

The event visualizer app allows you to create charts based on tracked data. It is particularly well suited for visualizing standardized responses (ie. option set information).

When creating a visualization that uses event as the output type, both event and tracker data are handled the same way as you can only select one program stage to work with within event visualizer. The “enrollment” output type does not work within this app.

There is a “tracked entity instance” output type within event visualizer. This will only work with tracker data (not event data) as it counts the number of unique tracked entity instances that meet given criteria within a single program.

## Create an event visualization

1. Select your chart type
2. Select your program and program stage
3. Select your data
4. Define your filters for the data selected
5. Select your period
6. Select your organisation unit
7. Modify your layout
8. Update your visualization

By default, an event visualization will use event as its output type. This means these visualizations are summarizing **all events** within a ***single*** program stage, including any repeated events within the stage you have selected.

## Tracked entity output type

We can modify our charts to use the output type "Tracked entity instance." In order to do this, we select the chart options menu and modify the output type. This will count the number of TEI's that meet your criteria. Repeated event data would therefore be excluded from this output. 

Unlike enrollment type outputs however, we are not able to review data from multiple stages when using the TEI output type in event visualization.

Note that while enrollment exists within this output type list, it will not work and should be ignored.

## Enrollment outputs vs. tracked entity instance outputs

Why the different language between event reports and event visualizer regarding the output type? The Enrollment output type in event reports allows you to display information unique to an enrollment, as well as obtain data across an entire enrollment (meaning you can review data from multiple program stages together in the line list; and obtain unique counts via the pivot table). The "Tracked entity instance" output type in event visualizer is much more limiting. It does not allow you to pull data from multiple program stages; it just let's you count the number of unique tracked entities (usually people) that meet the criteria you have set via your filters within a program stage 1 or more times. This can be useful but it is important to identify this distinction.

## Saving an event visualization

1. Select the favorites menu
2. Select "Save as"
3. Provide your report with a name and save it

## Downloading an event visualization

1. Select the downloads menu
2. Select the format you want to download the report it
3. Open the downloaded report by retrieving it from your downloads folder