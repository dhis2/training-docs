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

## Part 1: Installation of the Android Setting Web App

To use the Android Settings Web App you need to first install the app by going to DHIS2 web interface

* Go to Search Bar and Search for the App Management app
* Go to the app hub
* Click on Android Settings
* Install the Android Settings App

![](images/androidsettingswebapp/image14.png)

### Users roles to use the App

Trainers can briefly discuss the user roles. For more information about user roles. ([Click Here](https://docs.dhis2.org/en/use/user-guides/dhis-core-version-240/configuring-the-system/users-roles-and-groups.html?h=user+2.40#mgt_userrole))

Please note that in this version of the web app, only users with the authority to manage the android settings web app, found under "Other authorities" can edit and access the app.

So to make sure your users have this role, you can go to Users > User role and in this you can select the app authorities as android settings app.

![](images/androidsettingswebapp/image1.png)

### STOP : Perform Exercise 1 - Install the Android Settings Web App

## Part 2: Android Settings App Overview

_Note: In this session trainers will give an overview of each section and will do a detailed session on Appearance._

* Open the DHIS2 web interface
* In the apps menu , find the android settings app
* Select the App and you will see the Home Screen for Android Settings Web App as shown below:

![](images/androidsettingswebapp/image3.png)

### General Settings:

* General: Defines generic parameters like SMS gateway number and TEI reserved values. 
* An important paramater here is whether or not you allow the user to take screenshots. This may significantly help with troubleshooting in the field. 
* Another important option is the "reserved values." This is used for generating your unique IDs. This option allows you to download pre-generated IDs for the device to use offline. When you come back online, it will refresh your IDs when you sync. Based on the connectivity etc. you should be careful in defining this so people do not run out of IDs when they are working offline. 

### Synchronization:

* Global: It offers additional parameters to control metadata/data synchronization.
  * Sync options that are included here include both the defaults for metadata and data. 
  * You may also want to include a maximum size of a file download if you are on a capped data plan. 
* Programs: This section controls the program data synchronization parameters. It has a section to define global or default parameters to be used in the synchronization of all programs.
  * Note that you can define how many TEIs are downloaded to the device upon syncing.
  * You also have options for defining how many events are downloaded in total
  * It priortizes these downloads based on the date the TEI or event was created
  * These downloads are spread depending on the settings level
* Datasets: Define synchronization parameters for data sets
  * This number determines how many past data sets PER org unit that you are assigned gets downloaded. So a value of 10 could download many more data sets depending on how many org units a person is assigned.
* User sync test: Check how much data a user downloads when syncing and determine if the user can sync everything correctly based on your defined settings

