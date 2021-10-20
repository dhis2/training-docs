# Program Indicators - Session Summary

- A program indicator is derived from individual level event or tracker data
- We can use program indicators in data visualizer, maps and event reports by selecting them as a data item
- There are two types of program indicators:
  - Event : will perform an operation based on all of the events within a single program stage
  - Enrollment : Uses data from the most recent event; can combine data from multiple program stages
- Program indicators can function on two levels:
  - Showing data for one event/tracked entity instance
  - Showing summary data (counts, sums, averages, etc.) for all of the events/tracked entity instances within a specified org unit/period

Program indicators allows us to address limitations/gaps in other apps when reviewing tracker data as they can be used to summarize data across multiple stages (keeping in mind they will use the most recent event's data in their output). This includes:

1. Creating "enrollment" type summaries of data from multiple stages in data visualizer for both charts and tables (not possible in event visualizer and event reports)
2. Creating "enrollment" type summaries of data from multiple stages in maps (not possible in the event or tracked entity layer)

These other apps (event visualizer, reports, event layer) are still useful, particularly when working event data as users can modify the filters for the data they want to see in real time. When working with a program indicator, these must be pre-configured and are not as easily modified by the person reviewing the data.

