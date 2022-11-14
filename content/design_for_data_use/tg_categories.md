# Trainer’s Guide to the Category Model

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session "The correct way to work with the category model." This session follows the standard Academy training approach with 

1. a live demo session where the trainer demonstrate and explain the features, and 
   
2. a hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## Learning objectives for this session

1. Define the DHIS2 category model
2. Use categories to disaggregate data in analysis apps
3. Create category options, categories and category combinations following a standard operating procedure
4. Demonstrate how to verify the creation of category option combinations using the API
5. Descrbie the relationship between categories, data dimensions and anlaytics
6. Apply category combinations to data elements

## Time Requirements

- Live Demo: 
- Hands-on Exercises: 
- Assignment: 

## Background



## Preparations



## Best Practices



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

### Create a chart using data elements within a data element group

### Create a chart using data element groups within a data element group set

#### STOP - Perform Exercise 1

### Show how to manage DE Groups and DE Group Sets in Maintenance

#### STOP - Perform Exercise 2

### Review the process of creating DE Groups and Group Sets via the API

### Retrieve the list of data elements via the API

#### STOP - Perform Exercise 3

### Create DE groups via maintenance

### Import the DE groups into DHIS2 via the Import/Export app

#### STOP - Perform Exercise 4

### Create the DE group sets via maintenance

### Explain connection of data dimensions to analytics and use created groups in visualizer

#### STOP - Perform Excercise 5