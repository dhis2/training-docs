# Trainer’s Guide to Data Element Groups and Group Sets

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session "Organisation Unit Groups and Group Sets." This session follows the standard Academy training approach with 

1. a live demo session where the trainer demonstrate and explain the features, and 
   
2. a hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## Learning objectives for this session

1. Describe what organisation unit groups are
2. Describe what organisation unit group sets are
3. Use organisation unit groups in analysis apps
4. Use organisation unit group sets in analysis apps
5. Configure organisation unit groups in maintenance
6. Configure organisation unit group sets in maintenance

## Time Requirements

- Live Demo: 
- Hands-on Exercises: 
- Assignment: 

## Background

Program Indicators offer a flexible way of interacting with tracker data and allow for a number of advanced functionality as it relates to aggregating or summarizing individual tracker data. This session will focus on how program indicators can be used in data visualizer, maps and event reports to both display information related to a single tracked entity as well as summarize data for many tracked entities based on the org unit and period you are working with. 

## Preparations

This session will see you creating a number of visualizations. Ensure that you have run analytics in the demo database you are using and that all the data is being populated correctly. If you find that data is not present for the correct period or year, please contact the training content team so we can advise how to move the data correctly.

You should consider running through the entire demo prior to presenting it. After this, you should take the quick guide and supplement it with any additional notes you made while running through the demo. If you identify any changes that may be required or additional explanation that would be helpful within the session, please content the training content team in order to allow us to evaluate how to best integrate this feedback into the material.

Every visualization that you are asked to create has been saved and should be shared for public view. You can open each one up and review how it is has been made if you are unsure about any of the visualizations contents.

Also, the learner's guide and session summary are the main material that will be provided to the learner's with both detailed steps for ungraded exercises as well as the key messages from the session. Review these as well to ensure you are able to discuss these key points during your demonstration.

## Best Practices

Before starting the demonstration, please keep in mind that the most important thing is that the audience is following, so make sure to ask questions to the audience to verify that they are following. If something is unclear, go back and go through it slowly. If you don’t have time for all the steps, it is better to cut some steps, than to go fast while nobody understands.

In an online setting, you will be breaking regularly to allow them to perform various ungraded exercises in order to keep them engaged.

In an in-person setting, the participants may be doing the demo with you at the same time. In this scenario, it is ideal if there are other trainer's moving around the room to support participant's as it will be difficult for the trainer leading the session to answer many individual questions during the demonstrations. 

## Quick Guide

1. In data visualizer, create a pivot table using an event program indicator from COVID-19 Vaccination Registry program
- Visualization Type : Pivot Table
 - Data 
   - Data Type : Program Indicator
   - Program : COVID-19 Vaccination Registry program
   - Program Indicator : Underlying conditions
 - Period : Last 6 months
 - Org Unit : All Level 2 OUs

2. Create a chart using program indicators from different program stages from COVID-19 Case-based Surveillance Program
   1. Create the chart using
      - Visualization Type : Line Chart
       - Data 
         - Data Type : Program Indicator
         - Program : COVID-19 Case-based Surveillance Program
         - Program Indicators : 
           - COVID-19 Symptoms present
           - COVID-19 Symptoms present - death
           - COVID-19 Symptoms present - recovered
       - Period : This Year
       - Org Unit : All Level 2 OUs
   2. Explain the visualization and where the data is coming from. Note that this type of chart can not be made in event visualizer.
   3. Convert the chart to a pivot table. Note that this type of table can not be made in event reports.
   4. Convert the table to a map. Note that you are now using the thematic layer to display your data, which has different options available compared to the event and TEI layer.

STOP! Have them perform *Exercise 1* in the learner's guide.

3. Create a map using a program indicator from the COVID-19 Case-Based Surveillance program
   1. Create the chart using
      - Layer Type : Thematic 
      - Data:
        - Item Type : Program Indicators
        - Program : COVID-19 Case-Based Surveillance
        - Program Indicator : COVID-19 Suspected Cases
        - Leave the aggregation type as default
      - Period:
        - Period Type : Relative
        - Period : Last 12 months
        - Display Periods : Timeline
      - Org Units : All Level 2 OUs
      - Filter : None
      - Style : Bubble Map, Single Color Legend
   2. Highlight the additional options available when using the thematic layer via program indicators 

STOP! Have them perform *Exercise 2* in the learner's guide.

4. Create an event report showing the number of relationships by TEI from the COVID-19 Case-based Surveillance Program
   1. Create the linelist using
      - Table Style : Line, Output Type : Enrollment
      - Program : COVID-19 Case-based Surveillance
      - Stage : Stage 1 - Clinical examination and diagnosis
      - Data
        - First Name, Surname
        - Sign/Symptoms Present
        - PI COVID-19 Contacts
      - Period : This year
      - Org Unit : CHW Mahosot
   2. Explain the report and the program indicator you have added to this report
   3. Add the program indicator for days between symptoms onset and consultation
   4. In data visualizer, create a bar chart showing the average days between onset and consultation across all level 3 OUs within Savannakhet
      1. Create the chart using
       - Visualization Type : Bar Chart
       - Data 
         - Data Type : Program Indicator
         - Program : COVID-19 Case-based Surveillance Program
         - Program Indicator : COVID-19 days between onset and consultation
       - Period : This Year
       - Org Unit : Level 3 OUs within Savannakhet
      2. Explain the chart and based on what the program indicator is showing

STOP! Have them perform *Exercise 3* in the learner's guide.

5. Review the recap slide
6. Have them perform the assignment

## Live Demo step by step

### Create a chart using data element within a data element group

#### STOP - Perform Exercise 1

### Create a chart using data element groups within a data element group set

#### STOP - Perform Exercise 2

### Show how to manage DE Groups and DE Group Sets in Maintenance

#### STOP - Perform Exercise 3

### Review the process of creating DE Groups and Group Sets via the API

### Retrieve the list of data elements via the API

#### STOP - Perform Exercise 4

### Create DE groups via maintenance

#### STOP - Perform Exercise 5

### Import the DE groups into DHIS2 via the Import/Export app

#### STOP - Perform Exercise 6

### Create the DE group sets via maintenance

#### STOP Perform Exercise 7

### Explain connection of data dimensions to analytics and use created groups in visualizer

#### STOP - Perform Excercise 8