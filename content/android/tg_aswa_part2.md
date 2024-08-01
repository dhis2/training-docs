# Trainer’s Guide on Android Settings Web App Part-2

## What is this guide?

This guide is a support document for DHIS2 Android Academy trainers for the session "Android Settings Web App". The session follows the standard Academy training approach with

* A live demo session where the trainer demonstrates and explains the features of the topic
* A hands-on session with exercises where participants get to practice the explained features.

## Learning objectives for this session

* How to Install the Android Settings Web App
* How to navigate through the Android Settings Web App
* Understand different features for the web App

## Time needed for this session

Live demo: 45 min

## Background

The Android Settings Web App

1. Allows admins to configure synchronization parameters for the DHIS2 Android App, 
2. Can encrypt the local database of an Android device
3. Can customize the appearance of Programs, Data sets, the Home screen, and add TEI Analytics items. 

The configuration parameters defined within this web app will overwrite the settings of all Android devices using the DHIS2 Android Capture App.

## Part 1: TEI Analytics configuration

TEI Analytics manage Tracked Entity Instance (TEI) analytics for tracker program.

To add analytics (Bar chart, line chart, pivot tableor single value type) for TEI 

* Click on Add TEI Analytics

  ![](images/androidsettingswebapp/teianalytics.png)

A window will pop-up,now you need to select,

* Select Program , in this case we will select Immunization program.

* Select program stage - Immunization

* Give name and short name to the analytics chart title: Weight

* Select Visualization type : Line chart

* Select period type : Quarterly

* Select visualization element type : Data Element

* Select Data Element : Weight in (kg)

* Click on Add Analytics

  ![](images/androidsettingswebapp/addteianalytics.png)

This will be listed under TEI Analytics section

![](images/androidsettingswebapp/addteianalytics1.png)

* Now Go to the Android App and sync your changes (make sure you go to Settings -> Sync Configuration now, to sync the changes that were done in the Android settings web app)

* Now go to the Immunization program.

* Select any child,click on the Analytics tab,you will see the below screen with all the analysis you have added for TEI.

  ![](images/androidsettingswebapp/androidtei.png)

### STOP : Perform Exercise 1

## PART 2: Home Analytics configuration

Manage visualization for Home Screen in Android App.

* Select Home under Analytics tab

* Click on "Add Home Visualization"

* Select the visualization type from the list

_Note: From 2.40 version you can now select two different types of visualization_

  1. Event visualization
  2. Data visualization

   ![](images/androidsettingswebapp/homeanalytics.png)

* Select Visualization type : Data visualization

* Select Visualization item : NUT - Growth Monitoring

  ![](images/androidsettingswebapp/homeviz.png)

* Add an alternative title, otherwise, the app will display the name of the visualization.By default, the app will enable the group visualization setting.

* Create a new group: A free text box will pop-up to type the name or

* Select a created group visualization: Choose an option from the list to add the visualization or
Disable the group visualization by clicking on the checkbox.

* Click on the "Add Home Visualization" button.

* Click on "Save"

  ![](images/androidsettingswebapp/homesave.png)

* Now Go to the Android App and sync your changes (make sure you go to Settings -> Sync Configuration now, to sync the changes that were done in the Android settings web app)

* In the Home Screen, select the analytics tab

  ![](images/androidsettingswebapp/homeanalytics1.png)

* You will see the below screen with all the analysis you have added for Home.

  ![](images/androidsettingswebapp/homeanalytics2.png)



    NOTE: For each visualization object, the user will be able to filter in the app by:

    1. Period: Daily, Weekly, Monthly, Yearly, This Quarter, Last Quarter, Last 4 Quarters and Quarter this year.

    2. OrgUnit: Select "All" to display all the org units available to the user or "Selection" to specify one or multiple org units.

    Check the sharing settings of the visualization. The android users must have read access in order to download it. Use the “Visualization user test” functionality to test it.

### STOP : Perform Exercise 2

You can also perform the similar steps to add visulaization in Program and Datasets in Android settings web app.
## PART 3: 



