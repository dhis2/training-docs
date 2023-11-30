# Trainer’s Guide on APK Distribution Web App

## What is this guide?

This guide is a support document for the trainers to go over the topic "APK Distribution Web App".The session follows the standard Academy training approach with

* A live demo session where the trainer demonstrates and explains the features of the topic
* A hands-on session with exercises where participants get to practice the explained features.

## Learning objectives for this session

* Demonstrate how to Install the APK Distribution Web App
* Understand the implementation usage of the APK App.

## Time needed for this session

Live demo:
Hands-on exercises:

## Background

The APK Distribution app enables implementation administrators to manage and control the version of the Android app, making it easier to manage app updates and ensure compatibility with the DHIS2 system.

Admins will be able to upload the desired version and users will get a prompt message to update when they are not in the last updated version.

Please note that in this version of the Web App, only users with "ALL" authority are able to define the Android app versions. Other users having access to the web app can see the version history list and download the latest version, but cannot edit them.

## Part 1: Installation of the APK Distribution Web App

To use the APK Distribution Web App you need to first install the app by going to DHIS2 web interface

* Go to Search Bar and Search for the App Management app
* Go to the App hub
* Click on APK Distribution App
* Install the App.

_NOTE: The APK Distribution Web App is compatible with DHIS2 version 2.36 and above._

![](images/apk/apkinstall.png)

## Part 2: Upgarde the DHIS2 Android App to the new version

### Upload version

Follow the steps below to upload an Android app version:

* Click on Upload new version button.
* Assign a version number.
* Choose the minimum and/or recommend Android OS version.
* Add a URL that contains the APK of the Android app.
* Click on the "Create app version" button.

![](images/apk/uploadversion2.png)
![](images/apk/uploadversion.png)

So in this case we want to upgrade a new version 
2.9.0

So, for this we will follow the below steps:

* So in **Version** we will add latest vesrion i.e. 2.9.0
* You need to add a **Minimum Android version** that the app should support which is 5.0.2
* In the **Recommended Android vesrion** we will add 8.0
* In **Download URL** - you can go to the 
Github Link (https://github.com/dhis2/dhis2-android-capture-app/releases)
 
  * Select the apk file and copy the link 

* Go back to the DHIS2 web interface and paste the link.

![](images/apk/createversion.png)

_NOTE: When uploading a new apk, make sure that the app version is higher than the current/latest version_

* Create app version

### Delete version

To remove an Android App version:

* Search for the Android app version to delete.
* Click on "Delete".
* Click on the "Delete" button.

![](images/apk/deleteversion.png)

### Using Mobile device

This Web App can also be manipulated from a mobile device. To use it, open DHIS2 in the browser from a mobile or tablet device.

The mobile version allows the administrator user to upload and download app versions.




