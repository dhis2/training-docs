# Program Indicators - Session Summary

A program indicator is derived from individual level event or tracker data
We can use program indicators in data visualizer, maps and event reports by selecting them as a data item

There are two types of program indicators:

  - Event : will perform an operation based on all of the events within a single program stage
  - Enrollment : Uses data from the most recent event; can combine data from multiple program stages

Program indicators can function on two levels:
  - Showing data for one event/tracked entity instance
  - Showing summary data (counts, sums, averages, etc.) for all of the events/tracked entity instances within a specified org unit/period

Program indicators allows us to address limitations/gaps in other apps when reviewing tracker data as they can be used to summarize data across multiple stages (keeping in mind they will use the most recent event's data in their output). This includes:

1. Creating "enrollment" type summaries of data from multiple stages in data visualizer for both charts and tables (not possible in event visualizer and event reports)
2. Creating "enrollment" type summaries of data from multiple stages in maps (not possible in the event or tracked entity layer)

These other apps (event visualizer, reports, event layer, line listing) are still useful, particularly when working event data as users can modify the filters for the data they want to see in real time. When working with a program indicator, these must be pre-configured and are not as easily modified by the person reviewing the data.

We do not always use program indicators as there are pros and cons that must be weighted

***Pros***
- They offer more flexibility in creating summaries of event and enrollment tracker data
- They can be used in tools users are more familiar with (Data Visualizer, Maps)
- They offer a number of advanced functionality including boolean logic (if statements), relationship counts, difference in dates, etc.
  
***Cons***
- Each program indicator needs to be configured and this can be potentially quite time consuming
- Users can define a requirement for a program indicator but can’t modify filters in real time like they can with event reports, visualizer and the event layer
- There can be a significant performance hit in large systems

We must consider these before using program indicators in our own implementation.


