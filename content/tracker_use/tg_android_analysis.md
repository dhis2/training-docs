# Trainer’s Guide to Android Analysis

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session “Android Analysis.” This session follows the standard Academy training approach with

1. a live demo session where the trainer demonstrate and explain the features, and 
   
2. a hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by
step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## Learning objectives for this session

1. Demonstrate how maps are displayed in the tracker program and the use of the following elements:

   1. Carousel
   2. Navigation to location
   3. Map layers
   4. User current location

2. Understand how TEI Analytics work

   1. Data element evolution
   2. Program indicators


## Time Requirements

## Background

In this session, we will give the participants an opportunity to review the various features implemented within the android app to facilitate local analysis of data. These features can function when they are offline using data stored on the android device itself, and has the potential to add value within an implementation when used correctly.

## Preparations

Go through the Live demo step by step guide a few times before doing the actual demo for participants.
Make sure your user account is same or similar to the participants’ training accounts so that you don’t show more features, dimension options or forms than what they can see when doing the exercises.
Make sure the resolution on projector is OK for zooming

Create an account with the same level of access as the users you are demonstrating to (ie. if they can only search and enter within one facility, have your user have the same authority). If it is the procedure to enter this data from a paper form, it will be useful to have a copy of the form they would normally use as reference filled in. This can just be a form that you have filled in yourself for example. If they are entering data in real-time, then this is not required but you should prepare the details of an example case that you can follow in your examples.

For the exercises and small activities during the demo, fill out a couple extra forms that the participants can use to register their own cases. Your training DB should have some existing cases filled in to help support the working list filter, relationships and searching functionality. If demonstrating the working lists functionality, you will need to have a subset of the events you have created and assigned to a user where you can show this functionality.

### APK File

Make sure that you have the app made for training purposes otherwise you will not be able to cast your screen:

https://github.com/dhis2/dhis2-android-capture-app/releases

This will be denoted by “training” at the end of the APK file.

![](resources/images/tracker_capture_android/image1new.png)

### Projecting your Android Device

The instructor will have to decide on which method they would like to use to mirror the android app on their computer screen. They will also have to set up a user account (if it doesn’t exist already) that is assigned to the same org unit as the program they are demonstrating.

Please review this CoP post for details on options you may use to mirror your android device:

https://community.dhis2.org/t/how-to-clone-your-android-screen-useful-for-presentations-debugging-etc/38077

### User Account

Ensure that there is a user account assigned to a lower level set of org units at the facility level within Trainingland that you can use prior to performing this session. If the participants are following along, ensure that there are user accounts for them to use as well assigned to lower level organization units. The demo user account is:

Username: android1

Password: District1#

### Participants

Send the instructions to the participants on how to install the Android app prior to the session. The instructions can be found 
[here](https://docs.google.com/document/d/1SUUUdmPSDycFtdB9yUMq8ZWiWf8gNOu5xvtNj4_V63U/edit?usp=sharing).

Some participant's may not have been able to install the app by themselves. In that scenario, you may need to walk them through how to do this via google play.

## Quick Guide

1. Review the maps display within the Case Based Surveillance Program
   - Select the program and open the maps tab
   - Cycle through the carousel
   - Select a TEI and navigate to their dashboard
   - Navigate to the TEIs location (than switch back to the original maps display)
   - Change the map layers to show the heatmap and use the satellite view
   - Navigate to your location
2. Review data element evolution charts within the Malaria case notification , investigation and response
   - Search for the TEI Alakazam Malakazama
   - Navigate to the analytics tab
   - Review and explain the chart that is shown
   - Move between visualization types
   - Explain the filters
3. Review program indicators within the Case-based surveillance program
   - Search for the TEI Theo Fleury
   - Review the events in Laboratory Result
   - Navigate to the analytics tab
   - Review and explain the program indicator “Total Lab Results”
4. Review program feedback within the Electronic Immunization Registry Program
   - Search for the TEI Maria Smith
   - Navigate to the analytics tab
   - Review and explain the various information that is displayed

## Live Demo step by step

Before starting, login to the android app using your training instance.

Username: android

Password: District1#

### Review the maps display within the case based surveillance program

The android app will display the map screen in event or tracker programs that contain one or more of the following elements:

- Event coordinates/Polygon
- TEI coordinates/Polygon
- Enrollment coordinates/Polygon
- Tracked entity attributes type coordinate
- Data elements type coordinate

#### Open the map

To access the demo map open the Case based Surveillance program and wait for it to load the list. At the bottom you’ll see the navigation bar. Select the map icon to access the map (note, in order to use this feature, your program needs to be collecting the coordinate during registration).

![](resources/images/android_analysis/cbsmap.png)

#### Cycle through the carousel

After opening the map icon, you will see TEI details at the bottom of the screen. This is referred to as the map carousel. You can scroll through all of the individuals registered in this program by scrolling the carousel horizontally.  The map will zoom into the selected coordinates. If there are no coordinates then a message will be shown. Each card in the carousel displays the tracked entity attributes marked as ‘Display in list’ when you configure your program. Click on the arrow to expand the card information. 

![](resources/images/android_analysis/mapopen.png)

If the TEI contains an image as an attribute you will also see the picture instead of the Person icon. 

Click on the card to open the TEI dashboard

![](resources/images/android_analysis/mapopentei.png) 

![](resources/images/android_analysis/mapteidash.png)

#### Navigate to the TEIs location (than switch back to the original maps display)

From the TEI dashboard, select back. This will take you back to the map. If the TEI or event has coordinates then a navigation icon will be displayed at the top right corner of the card. When you click it, your device will ask to select an app to open the location (if you have multiple maps apps, if not it will use the default one). This will take you to the location in the maps app you have selected.

![](resources/images/android_analysis/cbsmap2.png) 

![](resources/images/android_analysis/cbsmap3.png)

#### Change the map layers to show the heatmap and use the satellite **view**

Go back to the maps information in DHIS2 by navigating back to the capture app. By selecting the second button at the top right corner of the app, a menu will appear displaying all the possible layers.

Map layers you can see here include (depending on the configuration of the program): TEI coordinates, enrollment coordinates, Individual stage coordinates,  relationships, heatmap, tracked entity attributes of coordinate type, and data elements of coordinate type.

In the Case based surveillance program the app offers the TEI and Enrollment coordinate. Change the background layer and the add the heatmap to show how the map changes, click on the “Apply” button to the changes.

![](resources/images/android_analysis/mapopen3.png) 

![](resources/images/android_analysis/mapopenheatlayer.png) 

#### Navigate to your location

Navigate to your location by selecting the location icon on the map

If the user grants location permissions to the App, the map will show the current location represented as a blue color dot. The maps in the DHIS2 Android Capture App now include the possibility to center the map on the users location.

![](resources/images/android_analysis/cbsmap4.png)

#### STOP! Have them perform Exercise 1 

### Review data element evolution charts within the Malaria case notification , investigation and response program

Exit the maps tab and go back to the list within a program. 

It is possible to display the evolution of data elements over time as charts, values or tables. It is important to explain that this analysis will be available only for numeric value types within a repeatable stage.

Select the Malaria case notification , investigation and response Program and search for the TEI “Alakazam Malakazama”

Open the Analytics menu in the TEI dashboard by selecting the graph icon in the navigation panel to show the chart.

The chart here shows the temperature of the person as taken from different repeated events within a program stage. In this example, you are seeing a person’s temperature in degree celsius. 

![](resources/images/android_analysis/dedaily.png)

Explain it is possible to change the visualization to bars, line, table or single value

![](resources/images/android_analysis/diffcharts.png)

Filters are also available. Display the menu to see periods and organisation units available as filters.

![](resources/images/android_analysis/diffperiod.png)

#### STOP! Have them perform *Exercise 2* in the learner’s guide.

### Review program indicators (within the Case-based surveillance program)

You can display any program indicator by enabling the “Display in form” feature when configuring your indicator. All program indicators are listed at the top of the screen. These also would have appeared within tracker capture on the web.

Open the Case-based surveillance program and search for 

Given Name : Fleury 

Family Name : Theo 

Selecth the Analytics menu in the TEIs navigation bar from their dashboard and explain that "Total Lab results" indicator counts the total number of lab results recorded for this single case. 

![](resources/images/android_analysis/indicators.png)

Note that you can also set up program indicators to work within an event. You would just select the analytics section from within the event, rather then from the TEI dashboard.

> **NOTE** 
>
> The Android App does not support customized boundaries for program indicators.

### Review program feedback within the Electronic Immunization Registry Program

Switch over to the Electronic Immunization Registry Program and search for the TEI “Maria Smith” Select the analytics tab after opening this record. You can also show other information in the analytics tab. This will include feedback or other information that has been configured to show on the tracker dashboard. 

![](resources/images/android_analysis/feedback.png) 

#### STOP! Have them perform *Exercise 3* in the learner’s guide.

### Review program based dashboards

On an android device, you are able to review program dashboards, either on the home screen of android device or within each of the screens of the programs themselves.

You can get started by viewing a dashboard on the home screen. Do this by navigating to the home screen where all of your programs/datasets are listed. From here, select the analytics tab.

![](resources/images/android_analysis/home_dashboard.jpg)

This will take you to the dashboard page. 

These dashboards use locally stored data and already made visualizations (in line listing and data visualizer) in order to populate visualizations on the android device. Since they only use the locally stored data, this means this dashboards are available completely offline.

> **Note:**
> 
> Already existing visualizations get added to these dashboards by someone who has the "ALL" authority using the android settings web apps. There are many limitations to the android dashboard that will be covered in an accompanying slide. If you want to see how these dashboards are configured, navigate to the android settings web app and under the analytics section view either the home or program tabs.

In the dashboard page, you will see the avaiable dashboards at the top of the screen. You can switch between them by selecting one at any time.

![](resources/images/android_analysis/select_dashboard.jpg)

These dashboards only support a couple of chart types currently, this includes:
- Pivot tables
- Column Charts
- Line Charts
- Pie Charts
- Single Value Charts
- Line Lists

Let us start by reviewing the malaria case surveillance dashboard. It has both a pivot table as well as column chart on it. Both of these visualizations are reviewing cases by age distribution. The cases being shown are only those cases that are synced to the android device, based on the sync settings and the users assignment of org units.

These charts are interactive. By clicking on the menu icon of each visualization, you are able to modify the type of visualization and add period and org unit filters. 

![](resources/images/android_analysis/chart_menu.jpg)

To switch dashboards, just select the dashboard you want from the top of the menu bar.

Navigate back to the home screen and select the case based surveillance program.

There is also an analytics menu available at the program level, as we can see is the case for this program.

![](resources/images/android_analysis/program_dashboard.jpg)

If we select it, we will be able to view dashboards associated with the program. In this case, the dashboard shown here is the same as what is available on the home screen, but you are able to configure different outputs to use at the program and home level if needed.

At this point, navigate back to slide 3 of the Android analysis presentation to review the limitations of android analysis items. 

When you have completed a review of these points, have them complete the exercise.

#### STOP! Have them perform *Exercise 4* in the learner’s guide.
