# Trainer’s Guide to Event Reports and Line List

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session “Event Reports and Line List.” This session follows the standard Academy training approach with 

1. a live demo session where the trainer demonstrate and explain the features, and 
   
2. a hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a  detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps
and the flow of the demo.

## Learning objectives for this session

The overall objective of this session is to use the DHIS2 event reports app to review ***tracker*** aggregate data and the Line Listing app to review ***tracker*** individual level data. Detailed objectives include:

1. Describe the functions of the event reports app
2. Explain the difference between event and enrollment type reports
3. Describe the functions of the line listing app
4. Design line listing reports using tracker data
5. Describe the differences between how repeated and non-repeated stage data is displayed
6. Design line listing reports showing data from multiple tracker program stages

## Time Requirements

Live Demo: 
Hands-on Exercises:
Assignment: 

## Background

This session build on concepts introduced during the event fundamentals course. In the events fundamentals course, the learner would review how to create an event reports for a single event, creating both line-lists as well as aggregated reports. While this will be quickly reviewed within this session, a number of additional concepts not discussed (as outlined in the learning objectives) will also be covered. For this reason, the beginning part of the guide is brief as is assumed the learner is familiar with these concepts. If this is not the case, you will need to slow down on the explanation of the interface and create some initial reports together.

## Preparations

This session will see you creating a number of reports. Ensure that you have run analytics in the demo database you are using and that all the data is being populated correctly. If you find that data is not present for the correct period or year, please contact the training content team so we can advise how to move the data correctly.

You should consider running through the entire demo prior to presenting it. After this, you should take the quick guide and supplement it with any additional notes you made while running through the demo. If you identify any changes that may be required or additional explanation that would be helpful within the session, please content the training content team in order to allow us to evaluate how to best integrate this feedback into the material.

Every visualization that you are asked to create has been saved and should be shared for public view. You can open each one up and review how it is has been made if you are unsure about any of the visualizations contents.

Also, the learner's guide and session summary are the main material that will be provided to the learner's with both detailed steps for ungraded exercises as well as the key messages from the session. Review these as well to ensure you are able to get these key points across during your demonstration.

## Best Practices

Before starting the demonstration, please keep in mind that the most important thing is that the audience is following, so make sure to ask questions to the audience to verify that they are following. If something is unclear, go back and go through it slowly. If you don’t have time for all the steps, it is better to cut some steps, than to go fast while nobody understands.

In an online setting, you will be breaking regularly to allow them to perform various ungraded exercises in order to keep them engaged.

In an in-person setting, the participants may be doing the demo with you at the same time. In this scenario, it is ideal if there are other trainer's moving around the room to support participants as it will be difficult for the trainer leading the session to answer many individual questions during the demonstrations. 

## Quick Guide

1. Review the events reports interface

   Create an aggregate/pivot table using Malaria Case Notification program in Event Report App

   - Table Style : Pivot, Output Type : Event
   - Program : Malaria Case Notification program
   - Stage : Stage  - Case Outcome
   - Data : Malaria Final Classification (select Indigenious (local) as the filter), Age , Sex
   - Period : This year
   - Org Unit : Country

   STOP - Perform Exercise 1

2. Review event vs enrollment outputs in event reports

- Table Style : Pivot Table, Output Type : Enrollment
- Program : Electronic Immunization Registry
- Stage : Immunization
- Data: GEN - Sex
- Periods : This year
- Org Units : Country

Review and explain the output. Update the output type to events. Explain the difference between event vs enrollment in relation to this table.

STOP - Perform Exercise 2

1. Review the line list functionality in Event Reports

- Table Style : Line list, Output Type : Event
- Program : Electronic Immunization Registry
- Stage : Immunization
- Data
  - Given Name, 
  - Family Name,
  - Unique System Identifier, 
  - Sex
  - EIR - BCG 0.05 mL
- Period : This year
- Org Unit : Country

  Demo how to download the table, save the table

STOP - Perform Exercise 3

3. In the Line List app, review the Line List interface with the table. You can open the existing line list "MAL CS - Temp Evalulation/Travel History"

- Input - Event 
- Program : Malaria case notification , investigation and response
- Stage: Diagnosis and treatment
- Program Dimension: For this we will select the following program dimensions
    - Given Name
    - Family Name
    - Date of Birth
    - Local Case ID
    - Temperature
    - Recent travel within the country
    - Travel outside the country
- Period: Last 3 months
- OU: 01 Vientiane Capital
    
STOP - Perform Exercise 4

4. Create a list type event report for a repeatable stage using the Electronic Immunization Registry

- Input : Event
- Program : Electronic Immunization registry, Stage : Immunization
- Program Dimension :
  * Unique System Identifier (EPI) : EPI_12581
  * Given Name
  * Family name
  * Diagnosed with HIV and severe immunodeficiency
- Registration Date : This Year
- Org Unit : 0001 CH Mahosot

  Update the report using enrollment as the output type to compare and explain the differences in whats shown

STOP - Perform Exercise 5

5. Create a line list program using repeated event data linked together


- Input - Select Enrollment
- Program - Electronic Immunization registry
- Program Dimensions
  - Family name
  - Given name
  - Data Element "Diagnosed with HIV and severe immunodeficiency," where you will be able to see conditions and Repeated event tabs.
  - Filter - Select Yes HIV+,not on ART as your filter in the conditions tab.
  - Repeated Events tab - select the values for the most recent and oldest events
- Period : Date of Registration: Last 12 months
- OU : user org unit

STOP - Perform Exercise 6

6. Create a line list program using Input : Enrollment

- Input - Enrollement
- Program: Case based Surveillance
- Program dimensions
  - Data elements.To evaluate data across the stages we will select the following data dimensions:
  - Stage 1 : Diagnostic and clinical information
    - Cough
    - Fever
    - Difficulty in breathing
    - Temperature at admission

   - Stage 2: Lab Request
     - Date Specimen collected
     - Date Specimen sent to laboratory
     - Type of Specimen

   - Stage 4: Final Classification
     - Final classification

- OU : Lao PDR, Facility - Level 3
- Period : Date of notification: This Month and Last 3 Month

STOP - Perform Exercise 7

7. Create a line list program using legends

- Input : Event

- Program : Case-based Surveillance

- Stage : Diagnostic and Clinical Information
- Program dimensions tab
  - Select the Attributes:
    - Given Name
    - Family Name
    - Date of Birth
    - CBS_Clinical Diagnosis
  - Select Data Elements:
    - Temperature at Admission
- Options : Go to Legend 
- Organization unit : 0201 DH Phongsali
- Date of notification: Last 3 months

STOP - Perform Exercise 8
  
8. Review the recap slide

9.  Have them perform the assignment

Once they have completed all of the ungraded exercises, they should then complete the graded assignment

## Live Demo step by step

### Review the events reports interface

Access the event reports app and review the interface

![interface](resources/images/event_reports/interface.png)

#### Periods in Event Reports

In event reports, Periods can be selected as either Fixed or relative periods (same as aggregate) or with specific start/end dates (specific to event/tracker data)

![period_type](resources/images/event_reports/period_type.png)

If choosing the start/end dates than you can select exact dates to filter events based on the report date that was entered during event or tracker capture.

![start_end_date](resources/images/event_reports/start_end_dates.png)

### Create an aggregate/pivot table using the Malaria Case notification program in the Event Report App

Open the table "MALARIA_CS - Final Malaria Classification by Age & Sex." This is the table that you will create. You can explain the layout to the participants - including the table style, output type, data, periods and org units, before proceeding.

> Note: Event reports is currently the only app where you can make on the fly pivot tables using event/tracker data. This is not yet available in the line listing app, so the event reports and the line listing app need to be used in parrallel currently for the best results.

Clear your inputs by going to Favorites -> New.

Create an aggregate event report. You can use the following data items as an example:

- Table Style : Pivot, Output Type : Event
- Program : Malaria Case Notification program
- Stage : Stage  - Case Outcome
- Data : 
  - Malaria Final Classification (select Indigenious (local) as the filter), 
  - Age (years), Range Set = MAL-CS-Malaria age group
  - Sex
- Period : This year
- Org Unit : Country

The table should look like this after updating:

![table1_pivot](resources/images/event_reports/pivotnew1.png)

This is not exactly the table we want. We can make some adjustments to modify it.

Start with the layout. The layout can should like this

![table1_pivot_layout](resources/images/event_reports/pivotnew2.png)

Next, hide any empty rows and n/a data using the table options.

![hide_empty_rows](resources/images/event_reports/hide_empty_rows.png)

Now you should see the the table following the layout we've intended.

Note that you can modify the way data that is collected through tracker (and event) programs is aggregated. You can demonstrate this by changing the legend for the Age attribute to Age (CBS) and updating the table.

![age_selection](resources/images/event_reports/pivotnew3.png)

![table1_alternate](resources/images/event_reports/pivotnew4.png)

You will see all the totals are the same; however the disaggregation of the data is different as the data has been seperated by new categorizations.

This should be a review of concepts from the event fundamentals course; however if there are questions you can explain this concept a bit more as needed.

#### STOP - Perform Exercise 1

### Compare event vs enrollment analytics

Create a table using the following inputs:

- Table Style : Pivot Table, Output Type : Enrollment
- Program : Electronic Immunization Registry
- Stage : Immunization
- Data: GEN - Sex
- Periods : This year
- Org Units : Country

The table should look like this

![eir_enrollment](resources/images/event_reports/eir_enrollment_pivot.png)

Review the table with the participants. This table represents the total number of individuals, seperated by sex, that are enrolled in the electronic immunization registry program.

Modify the output type to event and update the table.

![eir_event](resources/images/event_reports/eir_event_pivot.png)

The values change by quite a bit, so why does this occur? 

The event output is counting all of the events in the electronic immunization registry program, seperated by sex, not the enrollments. An enrollment can consist of multiple events. This output would therefore not be very useful if we wanted to count the # of unique individuals that have been vaccinated. In that case, we should use enrollment as our output type. 

The output type is therefore an important consideration when choosing the output type when making a pivot table in event reports, depending on what you want to count.

#### STOP - Perform Exercise 2

### Review the line list functionality in Event Reports

> The line listing functions in event reports have been replaced by the **line listing app**. We will utilize the line listing app to create line lists for the remainder of the session after this example, but to compare features for those who are familiar with event reports we will just do a quick review of how line lists work in event reports. If you feel this is not needed, you can skip this section.

In this demo we will create a line list using an Electronic Immunization Registry.

Open the table "EPI - BCG Dose by Sex (List)" in the Event Report App in order to review the final output.

Create a new report by going to Favorites -> New and select the following details

- Table Style : Line list, Output Type : Event
- Program : Electronic Immunization Registry
- Stage : Immunization
- Data
  - Given Name, 
  - Family Name,
  - Unique System Identifier, 
  - Sex
  - EIR - BCG 0.05 mL
- Period : This year
- Org Unit : Country

Before updating the table, open the layout and move the items around in a logical order, noting how this will affect the output of the table.

![](resources/images/event_reports/table2new.png)

Proceed to update the table and discuss what is being shown.

The table should look like this after updating

![](resources/images/event_reports/table3new.png)

Modify the filters to see how the line list is updated

![](resources/images/event_reports/table4.png)

You will only see the data which meets this criteria

![](resources/images/event_reports/table3new.png)

### Other features as a refresher

You can also show them how to save the report using the favorites menu

![ev_save](resources/images/event_visualizer/ev_save_menu.png) 

and download the list

![ev_download](resources/images/event_visualizer/ev_download_menu.png)

#### STOP - Perform Exercise 3

### In the Line List app, review the Line List interface

> NB: We are using the line listing app version 100.15.1. Newer versions of the line listing app introduce cross program analytics, which have not yet been fully tested against our material. Please ensure you are using this version of the app.

Have the line listing app open in another tab or window with the table "CBS - Patients with Symptoms" open

![](resources/images/linelist/interfacepdnew.png)

In the Line Listing app, you can currently only make line lists. Aggregated pivot tables can not be made here unlike in the event reports app. The line listing app introduces many new features for creating line lists however, and is the recommended app for making these lists.

> Note: We will be using the line listing app to make line lists for the remainder of this session. We will only be using the "Pivot" table style in event reports to produce aggregate outputs. This is our suggested approach in live implementations as well. 

#### Input 

In the line list app, the input can be selected as either

* Event (see individual event data from an event program or within tracker program stages)

* Enrollment (see data from multiple stages in a tracker program)

If you have selected **Event**, then for tracker programs you need to select the program followed by the program stage to get all the data elements and attributes associated with that particular stage. 

To be able to select data from multiple stages you need to select "Enrollment" as the input type.

If you select **Enrollment** in the Input tab then all of the data elements associated with the program will be available from the different stages within the program for the purpose of cross stage selection of data elements. You are also able to access the program attributes using the enrollment type input.

![interface2](resources/images/linelist/imagenew1.png)

> To summarize, use event when you are only interested in data from one particular event in a program. Use enrollment when you want to review event data from multiple stages together.

#### Program dimensions

In the Line Listing app, all of the dimensions related to a tracker or an event program are present in the program dimension tab.

The line list will always be based on event or tracker programs and you can perform analysis on a range of dimensions. For programs with attribute combinations (these are programs that are disaggregate by an attribute of some kind), you can use program categories and category option group sets as dimensions.

Lets review the program dimensions tab.

![](resources/images/linelist/interfacepdnew.png)

Underneath the ***Program Dimensions*** heading we have the following:

The **organisation unit** dialog is flexible, offering essentially three ways of selecting organisation units:

1. By user org unit
2. By selecting org units directly
3. By using Org unit groups

**Event Status**
Filters data based on the event status:  Active, Completed, Scheduled.

**Program Status**
Filters data based on the event status:  Active, Complete, Cancelled.

**Program Dates**
After the program status, we will be able to select the enrollment and event dates depending on the input type we have selected. When the input is selected as enrollment, you will only be able to select the enrollment data here. When the input is event, you can select both the enrollment and event dates to be displayed.

In the ***Program data dimensions*** section we can modify the data we want to select.

In the type dropdown selector, you can filter by various parameters including:
* all types, which just shows everything
* data elements
* program attributes
* category
* category option group set

These last 2 only apply to programs that are using an attribute of some kind to dissaggregate the program.

There are multiple ways to add data dimensions to the layout. They can be added by hovering over the dimension and clicking the plus icon or by dragging and dropping a dimension straight to the layout area.

![](resources/images/linelist/datadimensionnew.png)


#### Add a data element

Lets add a data element to this table.

From the program dimensions tab, filter out the type to data elements. Search or find the data element "Other signs/symptoms" Either select the plus sign or drag the data element to the columns section above the table.

![add_de](resources/images/linelist/add_denew.png)

Update the table and you should see it added to your columns on the table.

#### Filter a data element option

To add a filter to a data element, select the data element either before or after it has been added. Select other signs/symptoms present.

![add_filter](resources/images/linelist/add_filternew.png)

This will open a dialog box. Select the items you want to include in your filter and move them over by either double clicking or using the arrow buttons.

![filter_options](resources/images/linelist/filter_optionsnew.png)

Select the Yes option and update the table. You will now only see patients that have signs/symptoms present in the table.

#### Change the org unit

To change the organisation unit, select the organisation unit option from the program dimesions tab.

![change_ou](resources/images/linelist/ou_selectnew.png)

You can select org units, relative org units levels and groups the same as in event reports.

![ou_select](resources/images/linelist/ou_selectnew1.png)

Change the org unit and update the line list to see its effect. 

#### Change the period

The period of data being shown is dependent on the type of input you have selected along with the dates associated with the program you have selected as discussed previously.

In the program dimensions tab, in this case you will see the enrollment and event date as event is the input type selected.

If you select the date of data entry and modify it.

![change_date](resources/images/linelist/change_datenew.png)

You can see how it affects the table outputs.

### Global Dimensions

This is located on the left side panel.

![global_dimensions](resources/images/linelist/global_dimensionsnew.png)

You can select the inputs for when the event or enrollment was
* Last updated on
* Created by
* last updated by

This will depend on if you selected event or enrollment as the input type.

### Create a line list program using Input : Event

In this demo we will create a line list using the Malaria case notification, investigation and response program.

You can open the existing line list "MAL CS - Temp Evalulation/Travel History"

Clear the input by going to File -> New

In this case we will be using

**Input** : Event 

>Note: If creating outputs of event type, then we can see the data from all events within a single program stage we are working with.

Select Program : Malaria case notification , investigation and response
Select Stage: Diagnosis and treatment

**Program Dimension**: For this we will select the following program dimensions

- Given Name
- Family Name
- Date of Birth
- Local Case ID
- Temperature
- Recent travel within the country
- Travel outside the country

Select OU: 01 Vientiane Capital

Enrollment date: Last 3 months

Your Dimensions should be assigned to the columns and the organisation unit to the filter.

![](resources/images/linelist/tempsingleev1.png)

Click on update. You will see the line list for a single stage.

![](resources/images/linelist/tempsingleev.png)

#### STOP! Have them perform Exercise 4 

### Create a list type event report for a repeatable stage using the Electronic Immunization Registry

Before you create this report, open up a record from capture that has repeated event data. The example used here has the following details that you can use to search for the person's record:

- Program : Electronic Immunization Registry
- Org Unit : 0001 CH Mahosot (Lao PDR - Vientiane Capital - 0101 Chanthabouli)
- Unique System Identifier (EPI) : EPI_12581
- First Name :Brent 
- Last Name : Hicks 
- Sex : Male

Open up this record and navigate to the "Immunization" stage within this program. Here you will see that there is more then one event within this program stage. Over the next several demonstrations, we will discuss the difference of event vs. enrollment report types and how repeated stage data is affected by this selection.

   ![](resources/images/linelist/tcnew.png)

Open up the different events within this stage and review the data that is there. The data will not be the same for each of these events making them easy to compare.

Keep tracker capture open on this record and open line listing in a new tab in case you need to refer to this record again.

We will now proceed to explain the how event and enrollment type reports handle this repeatable stage data.

Open the table "EIR - HIV Summary (Event)" This the table that you will create. You can explain the layout to the participants before continuing.

Clear your inputs by going to File -> New.

Create an event report with the following inputs:

- Input : Event
- Program : Electronic Immunization registry, Stage : Immunization
- Program Dimension :
  * Unique System Identifier (EPI) : EPI_12581
  * Given Name
  * Family name
  * Diagnosed with HIV and severe immunodeficiency

- Registration Date : This Year
- Org Unit : 0001 CH Mahosot

To make sure you get a specific record you need to Select EPI number and enter the ID (EPI_12581) to be used as a filter, as shown in the screenshot.

   ![](resources/images/linelist/uniquenumber.png)

This should pull up the respective information for the two events that we saw when we reviewed this record in tracker capture

The table should look like this

   ![](resources/images/linelist/eventreport.png)

> Now you can explain how the event type report selection affects our output. When we are creating reports and use "event" as the input type, ALL of the events from within a program stage will be output on our report. There is a limitation here in that we can only pull all of our event data from within one program stage, and as a result they are not really "linked" together as they are separate lines within our report.

We can further demonstrate this concept by showing more repeated event data. Modify the output so you are not filtering by any Unique System ID and update the report. Try sorting the data by surname. Scroll through the report; you should see several repeated events displayed on this report.

   ![](resources/images/linelist/eventreportmultiple.png)

In summary, when running an event report with repeatable data using "event" as the output type, all of the event data from a single program stage will be used in the report!

Update the report using enrollment as the output type.
As a reminder, here are the selections to make

- Input : Enrollment
- Program : Electronic Immunization registry, Stage : Immunization
- Program Dimension :
  * Unique System Identifier (EPI)
  * Given Name
  * Family name
  * Diagnosed with HIV and severe immunodeficiency

- Registration Date : This Year
- Org Unit : 0001 CH Mahosot

This is saved as "EIR - HIV Summary (Enrollment) Line list" in DHIS2 for reference

   ![](resources/images/linelist/enrollmentreport.png)

When we make this update, the number of records shown changes. This occurs because enrollment type reports only use the most recent event within a program stage for their output.

>Note: there is an enhanced feature in the Line list app, with the help of which you can define the most recent events and the oldest events you want in the output.

#### STOP - Perform Exercise 5

### Create a line list program using repeated event data linked together

In this example, you will be creating the following table (saved as EIR - HIV Immunodeficiency - Linked Repeated Events)

![](resources/images/event_reports/repeated_events_example.png)

In this table, repeated events all appear on one line linked to a single record, rather then in different lines or only showing the most recent event as in our previous examples.

You can explain this before moving on.

Follow these steps to create this line list. (clear the table by going to File-> New to get started.)

- Input - Select Enrollment
- Program - Electronic Immunization registry

   ![](resources/images/linelist/enrollnew5.png)

- Program Dimensions
  - Family name
  - Given name
  - Data Element "Diagnosed with HIV and severe immunodeficiency," where you will be able to see conditions and Repeated event tabs.
  - Filter - Select Yes HIV+,not on ART as your filter in the conditions tab.

  ![](resources/images/linelist/enrollnew8.png)
  - Click on the Repeated Events tab and select the values for the most recent and oldest events
  
 In this case we are selecting
- Most recent events : 2
- Oldest events : 1

   ![](resources/images/linelist/enrollnew9.png)

- Period : Date of Registration: Last 12 months
- OU : user org unit


Once you Click on update, you will see the below observation.

![](resources/images/event_reports/repeated_events_example.png)
 
The advantage of this output is that we can have information from repeated events on a single line. This is different then when using the event input type, which lists repeated events on seperate lines.

#### STOP! Have them perform Exercise 6

### Create a line list program using Input : Enrollment

You can open the already existing linelist "CBS - Patient Details (Enrollment)" and review this together. This line list takes data from multiple program stages and displays it against the record. Review this and explain prior to creating the new line list.

Follow the steps to create this line list 

1. Click on Input and Select Enrollment

   ![](resources/images/linelist/enroll1.png)

2. Choose the Program: Case based Surveillance

   ![](resources/images/linelist/enrollnew1.png)

Select the program dimensions tab.

3. Select the OU : Lao PDR, Facility - Level 3

4. Date of notification: This Month and Last 3 Month

5. Select your data elements. Note you can filter data between stages by selecting Type = Data Element, then selecting the stage you want to filter from.

   ![](resources/images/linelist/filter_by_stage.png)

To evaluate data across the stages we will select the following data dimensions:

   Stage 1 : Diagnostic and clinical information
   * Cough
   * fever
   * Difficulty in breathing
   * Temperature at admission

   Stage 2: Lab Request
   * Date Specimen collected
   * Date Specimen sent to laboratory
   * Type of Specimen

   Stage 4: Final Classification
   * Final classification

![](resources/images/linelist/enrollnew3.png)

6. Click on Update 

![](resources/images/linelist/enrollnew4.png)

#### STOP! Have them perform Exercise 7

### Create a line list program using legends

> Note: Defining Legend sets - Before using legends in a line list, you need to define the legend sets in maintenance. Legend sets categorize data into different ranges with corresponding colors.

Legends are used to create visual representations of data, such as color-coded maps or charts, to help interpret the data more easily. 

A chart with a legend applied is saved as "CBS - Patients with fever at time of admission". You can review this chart before moving on.

Follow these steps to create this line list.

- **Input** : Event

- **Program** : Case-based Surveillance

- **Stage** : Diagnostic and Clinical Information

![](resources/images/linelist/legendimagenew1.png)

In the program dimensions tab

- **Organization unit** 0201 DH Phongsali

- **Date of notification** Last 3 months

Select the Attributes:
     
* Given Name
* Family Name
* Date of Birth
* CBS_Clinical Diagnosis

 Select Data Elements:
* Temperature at Admission

![](resources/images/linelist/legendimagenew2.png)

**Options** > Go to Legend 

   * Enable use a legend for table cell colors
   * Legend style: Legend changes backgroung colour
   * Legend type: Choose a single legend for the entire visualization
   * Legend : Select pre-defined legend set "Fever"

![](resources/images/linelist/legendimage3.png)

![](resources/images/linelist/legendimage4.png)

 Click on Update to see the below table

![](resources/images/linelist/legendimage5.png)

(In this you will observe the red cell in the cases where temperature is more than 38 degree celcius)

You can also see the legend key is you select show legend key on the side bar.

![](resources/images/linelist/legendimage6.png)

#### STOP! Have them perform Exercise 8

## Assignment

After you have completed all demos and they have finished the exercises, have them complete the graded assignment for this session. If you find you are running out of time, assign the graded assignment to them and ask them to complete it outside of the live scheduled session.