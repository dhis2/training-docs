# Trainer’s Guide to Event Visualizer

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session “Event Visualizer.” This session follows the standard Academy training approach with 

1. a live demo session where the trainer demonstrate and explain the features, and 
   
2. a hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup
guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps
and the flow of the demo.

## Learning objectives for this session

1. Describe the functions of the event visualizer app
2. Describe the event visualizer interface
3. Create visualizations using tracker data
4. Describe the limitations of event visualizer when working with tracker data


## Time Requirements

- Live Demo: 3 demos, ~15 minutes each
- Hands-on Exercises: 3 exercises, ~10 minutes each

## Background

This session is more or less a review of what the participants have learned during the event fundamentals course. This is because event visualizer does not introduce any new concepts around the management of tracker data and does not have any enrollment type outputs built in. This session will therefore discuss this constraint as it is applied to tracker data and review some of the features available in event reports quickly.

## Preparations

This session will see you creating a number of visualizations. Ensure that you have run analytics in the demo database you are using and that all the data is being populated correctly. If you find that data is not present for the correct period or year, please contact the training content team so we can advise how to move the data correctly.

You should consider running through the entire demo prior to presenting it. After this, you should take the quick guide and supplement it with any additional notes you made while running through the demo. If you identify any changes that may be required or additional explanation that would be helpful within the session, please content the training content team in order to allow us to evaluate how to best integrate this feedback into the material.

Every visualization that you are asked to create has been saved and should be shared for public view. You can open each one up and review how it is has been made if you are unsure about any of the visualizations contents.

Also, the learner's guide and session summary are the main material that will be provided to the learner's with both detailed steps for ungraded exercises as well as the key messages from the session. Review these as well to ensure you are able to get these key points across during your demonstration.

## Best Practices

Before starting the demonstration, please keep in mind that the most important thing is that the audience is following, so make sure to ask questions to the audience to verify that they are following. If something is unclear, go back and go through it slowly. If you don’t have time for all the steps, it is better to cut some steps, than to go fast while nobody understands.

In an online setting, you will be breaking regularly to allow them to perform various ungraded exercises in order to keep them engaged.

In an in-person setting, the participants may be doing the demo with you at the same time. In this scenario, it is ideal if there are other trainer's moving around the room to support participant's as it will be difficult for the trainer leading the session to answer many individual questions during the demonstrations. 

## Quick Guide

1. Review the event visualizer interface

2. Review and create a bar chart showing EIR - BCG 0.05 ml dose by Location using the Electronic Immunization Registry program. 

   - Program : Electronic Immunization Registry, Stage: Immunization
   - Data Element: BCG 0.05 ml
   - Period : This Year
   - Org Unit : All level 3 OUs
   
   Discuss how this data is being pulled from all the events within the stage, meaning repeated event data will be included. This is not really a concern when using data from a non-repeatable stage.

   - Review saving and downloading the chart if needed

STOP - Exercise 1

3. Create a chart using option sets. 

   - Open the chart "MAL CS - Case Outcome by location."
   - Program : Malaria case notification, investigation and response
   - Stage: Case outcome 
   - Data items : MAL-CS - Outcome of illness
   - Periods : This Year
   - Org units : user sub-units

Discuss how this chart is quickly seperating options in an option set.

STOP - Exercise 2

4. Review the chart "CBS - Measles Virus Detection - PCR" and discuss the difference between the output type options "Event" and "Tracked entity instance"

STOP - Exercise 3

5. Review the recap slide

6. Have them perform the assignment

## Live Demo step by step

### Review the event visualizer interface

![ev_interface](resources/images/event_visualizer/ev_interface.png)

#### Periods in Event Visualizer

In event visualizer, similar to event reports, Periods can be selected as either Fixed or relative periods (same as aggregate) or with specific start/end dates (specific to event/tracker data)

![period_type](resources/images/event_reports/period_type.png)

If choosing the start/end dates than you can select exact dates to filter events based on the report date that was entered during event or tracker capture.

![start_end_date](resources/images/event_reports/start_end_dates.png)

### Review and create the chart "EIR - BCG 0.05 ml dose by Location" (a chart using yes/no data elements)

Open the chart "EIR - BCG 0.05 ml dose by Location" within event visualizer.

Event visualizer is particular adept at supporting outputs within both event and tracker programs as it relates to the visualization of data elements using option sets. We can quite easily combine various filters across different data elements and option sets to see an aggregate representation of the cross section of these filters as applied to our data.

This is the scenario we see with the chart that we are reviewing.

Review the Data Panel in particular.

![chart1_data_table](resources/images/event_visualizer/eventnew1.png)

We see here there is "Yes" output type selection here, just the program and the program stage. We are able to actually output a count of TEIs by using the options and this will be shown. We can not however combine data from multiple stages in event visualizer; charts using data from multiple program stages must be handled through the use of program indicators and data visualizer.

As a review, you can re-create this chart. It has the following inputs:

- Chart Type : Column
- Program : Electronic Immunization registry, Stage:Immunization
- Data : Data Element : BCG 0.05 mL
- Period : This Year
- Org Unit : All level 3 OUs

1. Favorites -> New
2. Select the program (Electronic Immunization Registry) and stage (Immunization)
   1. Note here again there is no enrollment output type , event visualizer is using the "event" output type by default; meaning all events in across all stages are counted in the totals being displayed
3. Select the data (Data Element : BCG 0.05 mL)
4. Select "Yes" only.

![chart1_data_table](resources/images/event_visualizer/eventnew1.png)

3. Select the Period (This Year)

![chart1_period](resources/images/event_visualizer/evnew2.png)

4. Select the org unit (All provinces, or user sub-2units)

![chart1_OU](resources/images/event_visualizer/chart1_OU.png)

5. Modify the layout

![chart1_layout](resources/images/event_visualizer/evnew3.png)

6. Go to options and Hide all empty categories

![chart1_layout](resources/images/event_visualizer/evnew4.png)

Update the chart to review your output.

![chart1_output](resources/images/event_visualizer/evoutput1.png)

The chart is not sorted and does not have a title as is the case with the saved chart reviewed earlier. You can open up the options panel and add in these details.

![chart1_options](resources/images/event_visualizer/evsort1.png)

Then proceed to update your chart to view the final output.

![chart1_final](resources/images/event_visualizer/evfinal1.png)

#### Other features as a refresher

You can also show them how to save the chart using the favorites menu

![ev_save](resources/images/event_visualizer/ev_save_menu.png)

and download the chart

![ev_download](resources/images/event_visualizer/ev_download_menu.png)

#### STOP! Have them perform *Exercise 1* in the learner's guide.

### Create a chart using option sets

Open the chart "MAL CS - Case Outcome by location." This chart is showing malaria case outcomes as a stacked bar chart. While some functions of the event visualizer are not as useful as they could be, the event visualizer is very good at visualizing event data from option sets.

Let us quickly make this chart.

1. Chart Type : Stacked bar chart
2. Program : Malaria case notification, investigation and response
3. Stage: Case outcome
4. Data items : MAL-CS - Outcome of illness
5. Periods : This Year
6. Org units : user sub-units

Layout : 

![option_set_chart_layout](resources/images/event_visualizer/option_set_chart_layout.png)

After updating, this should be your final output:

![option_set_chart](resources/images/event_visualizer/option_set_chart.png)

You can quickly modify which options appear on the chart by filtering the data element in the data selection window

![option_set_chart_filter](resources/images/event_visualizer/option_set_filter.png)

You can modify these options and update the chart to see how it affects what data is shown.

#### STOP! Have them perform *Exercise 2* in the learner's guide.

### Review and modify the chart "CBS - Measles Virus Detection - PCR"

Open the chart "CBS - Measles Virus Detection - PCR" Nothing so unique about this chart; however we can note that it using data from Stage 4 - Lab Results in the surveillance program. This stage is repeatable, and by default we are seeing all of the events in this program stage being displayed on the chart.

Rather then counting the total number of tests with these results, what if we wanted the number of unique people with these test results? In event reports, we were able to use the enrollment type output to both count enrollments as well as combine data from multiple stages in one list. We do not have that option here, but we can count the number of tracked entities.

Open the chart options and review the output type

![chart2_options](resources/images/event_visualizer/chart2_options.png)

We can see there are 3 options:
1. Event
2. Enrollment
3. Tracked Entity Instance

***NB***: Enrollment does not work as we can not pull data from multiple stages in event visualizer. It seems to be there incorrectly. Please ask the participant's to ignore this option.

Select the option "Tracked entity instance" and update the chart. You should see a a few less positive cases identified within this org unit when compared to the previous chart, as it is counting the number of TEI's uniquely, rather then counting the number of events matching the criteria of your filter(s).

![chart2_final](resources/images/event_visualizer/evnew5.png)

> Note: Why the different language between event reports and event visualizer regarding the output type? The Enrollment output type in event reports allows you to display information unique to an enrollment, as well as obtain data across an entire enrollment (meaning you can review data from multiple program stages together in the line list; and obtain unique counts via the pivot table). The "Tracked entity instance" output type in event visualizer is much more limiting. It does not allow you to pull data from multiple program stages; it just let's you count the number of unique tracked entities (in this case individual people) that meet the criteria you have set via your filters within a program stage 1 or more times. This can be useful but it is important to identify this distinction.

In explaining the concept above to the participant's, you can refer back to slide 4 in the presentation. 

#### STOP! Have them perform *Exercise 3* in the learner's guide.

## Recap

Review the recap slide with them at the end of the session before they perform the assignment

## Assignment

After you have completed all demos and they have finished the exercises, have them complete the graded assignment for this session. If you find you are running out of time, assign the graded assignment to them and ask them to complete it outside of the live scheduled session.