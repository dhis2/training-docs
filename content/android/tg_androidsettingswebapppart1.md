# Trainer’s Guide on Android Settings Web App Part-1

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
Hands-on exercises: 15 min

## Background

The Android Settings Web App

1. Allows admins to configure synchronization parameters for the DHIS2 Android App, 
2. Can encrypt the local database of an Android device
3. Can customize the appearance of Programs, Data sets, the Home screen, and add TEI Analytics items. 

The configuration parameters defined within this web app will overwrite the settings of all Android devices using the DHIS2 Android Capture App.

**_NOTE: In the version of the Web App (2.3), if the DHIS2 version is greater then or equal to (>=) 2.40, only users with the "M_androidsettingsapp" or "ALL" authority can define these parameters in the configuration. Other users accessing the web app can see the value of the parameters but cannot edit them._**

## Part 1: Installation of the Android Setting Web App

To use the Android Settings Web App you need to first install the app by going to DHIS2 web interface

* Go to Search Bar and Search for the App Management app
* Go to the app hub
* Click on Android Settings
* Install the Android Settings App

![](images/androidsettingswebapp/image14.png)

### Users roles to use the App

Trainers can briefly discuss the user roles. For more information about user roles. ([Click Here](https://docs.dhis2.org/en/use/user-guides/dhis-core-version-240/configuring-the-system/users-roles-and-groups.html?h=user+2.40#mgt_userrole))

Please note that in this version of the web app, only users with the 'ALL' authority or the one with Android Settings app are able to define those parameters in the configuration.With All authority you can also edit, create or delete the all settings (general, synchronization, appearance and analytics).

So to make sure your users have this role, you can go to Users > User group and in this you can select the app authorities as android settings app.

Other users having access to the web app can see the value of the parameters, but cannot edit them.

![](images/androidsettingswebapp/image1.png)

### STOP : Perform Exercise 1 - Install the Android Settings Web App

## Part 2: Android Settings App Overview

_Note: In this session trainers will give an overview of each section and will do a detailed session on Appearance._

* Open DHIS2 web interface
* In the Search Bar , search for Android Settings.
* Select the App and you will see the Home Screen for Android Settings Web App as shown below:

![](images/androidsettingswebapp/image3.png)

### General Settings:

* General: Defines generic parameters like SMS gateway number and TEI reserved values

### Synchronization:

* Global: It offers additional parameters to control metadata/data synchronization.
* Programs:This section controls the program data synchronization parameters. It has a section to define global or default parameters to be used in the synchronization of all programs.
* Datasets: Define synchronization parameters for data sets
* User sync test: Check how much data a user downloads when syncing

### Analytics:

* TEI: Manage TEI analytics for tracker programs
* Home: Manage visualizations to be shown in home screen
* Program: Manage visualizations for programs
* Data set: Manage visualizations for data sets

### Appearance:

These settings give control over the appearance of the data entry and list forms.

* Homescreen
* Programs
* Data sets


## Part 3: Home Screen Settings in Appearance Section

It allows the admin user to enable or disable the option to show the filters related to Date, Organisation Unit, Sync Status, and Assigned to me on the Home screen.

In the current setup you can see all options enabled.

![](images/androidsettingswebapp/image6.png)

For this session you can ,

* Disable the filter Assigned to me and Save.

  ![](images/androidsettingswebapp/image14.png)
  

* Now Go to the Android App (make sure you go to Settings &lt; Sync Configuration now, to sync the changes that were done in Android settings web app)
* Now go to Home Screen,You will see the below screen with only Date,Org Unit and Sync option in the filter.

  ![](images/androidsettingswebapp/image5.png)


### STOP : Perform Exercise 2 

## PART 4: Program Settings in Appearance Section

Program appearance allows to hide/show features within the program according to the configuration needs. These changes can happen globally, applying to ALL the programs, or specifically to a single one.

### Global Settings

Percentage (%) complete in Program: Enable or disable the option to show the completion percentage of the data entry form.

TEI referrals (**New 2.3.1**): It allows you to switch off/on the TEI referral option.

Collapse sections in form (**New 2.3.1**): Current behavior lets the sections collapse and expand in an accordion style. This option overrides the behavior by keeping all the sections of the form (registration and events) open and removing the "next" button in each section.

For this session Trainers can

* Disable “Show percentage (%) complete in Program toolbar”
* Go to Android Device to check the changes. 
* Make sure you perform Synchronization by going to Settings &lt; Sync Configuration
* Show the enrollment Screen to see the changes.

    ![](images/androidsettingswebapp/image7.png)

### For Program specific settings

Trainers can explain that this section allows the admin user to customize features such as filter, completion percentage, mandatory search, referrals, TEI headers and referral options. Each explained in the section below.

To add a specific setting:

* Click on _Add a Program Settings_, and a dialog will appear.

![](images/androidsettingswebapp/image11.png)
 
* Click on the dropdown that will show a list of programs.
* Clicking on a program will show the different filters to configure. The category combo filter depends on the category combo name.

![](images/androidsettingswebapp/image10.png)

TEI without searching: Offer online and offline search, as well as allow the user to create a TEI without a prior search.

TEI Header (**New 2.3.1**): Assign a specific attribute or expression that will be displayed as a header in TEI cards.

To add a TEI Header:

* Select a Program Indicator
* An expression related to the program indicator will be displayed

    **_Note:A notice box will be displayed if the selected program lacks expressions related to program indicators that are valid for Android._**


If any specific settings have been saved, a table will summarize the particular configuration per program, and the options to edit or delete these settings.

![](images/androidsettingswebapp/image2.png)

For this exercise the trainers can,

* Go to Immunization Program
* Enable “Allow the user to create a TEI without searching”

    ![](images/androidsettingswebapp/image4.png)

* Save the program

To test this you need to log back in your android device perform Sync configuration

* Go to Immunization program you should be able to to create a TEI without searching

### STOP : Perform Exercise 3

## PART 4: Data Set Settings in Appearance Section

Customize filter and sorting options available for data sets. 
* Settings can apply to all data sets a mobile user has access to. 
* Settings specific to individual data sets can also be applied.

### Global settings

The first part is for global settings that apply to all data sets an android user has access to.

![](images/androidsettingswebapp/image13.png)

In this section you can disable Sync Status from Global Settings and Perform the same steps as above to see the changes in the Android device.

### Specific settings

To add a specific setting:

* Click on _Add a Data set Settings_. A dialog box will pop up with a dropdown with a list of data sets.
* Click on a data set, and a list of options to enable or disable filters will be displayed.

![](images/androidsettingswebapp/image12.png)

![](images/androidsettingswebapp/image8.png)

### STOP : Perform Exercise 4