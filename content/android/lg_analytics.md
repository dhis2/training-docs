# Learner's Guide to the Offline Analytics

## What is this guide?

This guide contains all exercises and detailed steps to perform them related to the review of ***Offline Analytics*** for the Android Level 1 academy. Please perform each of the exercises when prompted to by your instructors

## Learning objectives for this session

The overall objective of this session is to demonstrate how to use 

1. Describe how analytics work in the Android app.
2. Demonstrate how to configure and display analytics in the Android app.

## Exercise 1 - Explore the automatically generated TEI analytics

In this exercise you will know how the automatically generated TEI analytics work and the information they display.

1. Open the Android app using your android user and go to your program (called "[User XX] Immunization").

2. Register a new Child.

3. Create 3 events for the stage "Immunization". Try to fill out all the fields in the form with meaningful values. They will be used in the next exercises as well.

// Some guidance about meaningful values

4. Once you have 3 events, open the Analytics tab for this Child.

// Image

5. Explore the automatically generated visualizations.


#### STOP - End Exercise 1


## Exercise 2 - Configure a table to show the evolution of temperature values

In this exercise you will create a custom TEI analytic table to show the evaluation of the particular data element. This exercise requires using the Android Settings Web App, please remember to take turns to modify it.

1. Open the Android Settings Web App.
   
2. Navigate to Analytics > TEI and click on "Add TEI Analytics".

3. Fill in the information for the TEI analytics:
    - Program: the program assigned to your user.
    - Program stage: the "Immunization" program stage (the only one in the list as it only shows repeatable stages).
    - Analytics chart title: choose a title for your table.
    - Visualization Type: pivot table.
    - Period type: daily.
    - Element type: data element.
    - Element: Temperature.

4. Click on "Add TEI analytics".

5. Click on "Save" (**it is important to Save your work**).

6. In your Android app, go to Settings and Sync configuration.

7. Once it is finished, go to an existing TEI in your program ("[User XX] Immunization") and explore the TEI analytics.

#### STOP - End Exercise 2

## Exercise 3 - Configure a WHO nutrition chart

In this exercise you will create a chart with the WHO nutrition background. This chart requires some configuration to make the relation between your existing data elements and the information expected by the WHO nutrition chart. Remember to take turns to use the Android Settings Web App.

1. Open the Android Settings Web App.

2. Navigate to Analytics > TEI and click on "Add TEI Analytics".

3. Fill in the information for the TEI analytics:
    - Program: the program assigned to your user.
    - Program stage: the "Immunization" program stage (the only one in the list as it only shows repeatable stages).
    - Analytics chart title: choose a title for your table.
    - Visualization Type: WHO nutrition
    - WHO visualization type: Weight for Height
    - **Important:** there is a bug that makes the chart title to be erased after clicking on "WHO nutrition". Make sure the title is not left blank. 
    - Gender attribute: Sex
    - Female title: F
    - Male title: M
    - Horizontal (x) axis: DataElement - NUTR - Height/Length (cm) 
    - Horizontal (y) axis: DataElement - Weight (in kg)

4. Click on "Add TEI analytics".

5. Click on "Save" (**it is important to Save your work**).

6. In your Android app, go to Settings and Sync configuration.

7. Once it is finished, go to an existing TEI in your program ("[User XX] Immunization") and explore the TEI analytics.

#### STOP - End Exercise 3

## Exercise 4 - 

#### STOP - End Exercise 3
