# Trainer’s Guide to Tracker Maps - Event and TEI Layer

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session “Event Visualizer.” This session follows the standard Academy training approach with 

1. a live demo session where the trainer demonstrate and explain the features, and 
   
2. a hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## Learning objectives for this session

1. Describe the maps app as it relates to tracker data
2. Describe the limitations of maps when working with tracker data
3. Create maps using tracker data within:
   1. The event layer
   2. The tracked entity layer


## Time Requirements

- Live Demo: 2 demos, 15 minutes each
- Hands-on Exercises: 2 exercises, 15 minutes each
- Assignment: 

## Background

This session is a mix of a review of what the participants would have learned through the event fundamentals academy and also introduces the tracked entity instance layer. This is because working with the event layer when using tracker data is no different then when you are using event data, which would have been covered in great detail within event fundamentals. The tracked entity layer is a new concept however currently has several limitations. This limitations will be discussed within the demonstration.

Note that the thematic layer is discussed during the program indicators session, not during this session.

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

1. Review how tracker co-ordinates are captured during both registration and within an event
2. Create a map using the event layer
   1. Create the map with the following inputs
      - Layer Type : Event
      - Data:
        - Program : COVID-19 Case-base Surveillance
        - Stage : Stage 3 - Lab Results
        - Coordinate field : Event Location
        - Event status : all
      - Period : This Year
      - Org Units : User org units 2x below
      - Filter :
        - Data item : Lab Test Result = Positive
      - Style :
        - Group events
        - Style by data element : Sex
   2. Note that dealing with event or tracker data when using the event layer is exactly the same
3. Create a map using the TEI layer with relationships
   1. Create the map with the following inputs
      - Layer 1 Type : Boundary Layer - Vientiane Capital
      - Layer 2 Type : Tracked Entity
      - Data:
        - Tracked Entity Type : Person
        - Program : COVID-19 Case-base Surveillance
        - Program status : all
      - Relationships : 
        - Display tracked entity relationships = yes
        - Relationship type : Has Been in Contact with
      - Period :
        - Program/Enrollment date
        - Start/ End Date : Oct 16, 2020 - Oct 16, 2021
      - Org Units : CHW Mitthaphap
      - Style : leave as default
   2. Discuss the limitations of this layer in its current state (no relationships across other programs, can't just collect the co-ordinate during registration and combine this with data within one of the events)
4. Review the recap slide
5. Have them perform the assignment

## Live Demo step by step

### Review how tracker co-ordinates are captured during both registration and within an event

To start this demonstration, let us discuss where we get the co-ordinates that are used on the TEI and event layer in regards to tracker data.

Go to capture and select any Level 4 OU (facility) along with the COVID-19 Case-based surveillance program. You will see a list of TEIs after making this selection

![tei_list](resources/images/maps/capture_tei_list.png)

Proceed to register a new person into this program

![new_registration](resources/images/maps/new_registration.png)

In this page, you will notice the co-ordinate field present. This co-ordinate field is for the tracked entity and can be used by the tracked entity layer within the maps app.

![registration_coordinate](resources/images/maps/registration_coordinate.png)

On android, you are able to capture the co-ordinate using your location; while on the web you must enter or select it from the map.

Cancel the registration and open up one of the existing records within your org unit; this will take you to their TE dashboard in tracker capture.

Review Stage 1, 3 and 4. Each of these stages will have a field called "Event point"

![event_coordinate](resources/images/maps/event_coordinate.png)

This is the co-ordinate field that is used to display data within the event layer and is captured in the same way as the registration co-ordinate (on android, you are able to capture the co-ordinate using your location; while on the web you must enter it or select it from the map).

### Create a map using the event layer

As a review, you can create a map using the event layer. The process is exactly the same as when working with an event. 

We can create a map using data from the COVID-19 Case-Based Surveillance Program for lab confirmed cases. 

Open the map "COVID_CBS - Lab confirmed cases, this year, by home location." This the map that you will create. You can explain the layout to the participants before continuing.

Clear your inputs by going to File -> New.

Create the map using the event layer with the following inputs:

- Layer Type : Boundary
  - Level 3
- Layer Type : Event 
- Data:
  - Program : COVID-19 Case-base Surveillance
  - Stage : Stage 3 - Lab Results
  - Coordinate field : Event Location
  - Event status : all
- Period : This Year
- Org Units : User org units 2x below
- Filter :
  - Data item : Lab Test Result = Positive
- Style :
  - Group events
  - Style by data element : Sex

The map should look like this

![map1](resources/images/maps/map1.png)

**Data Tab**

![map1_data](resources/images/maps/map1_data.png)

**Period Tab**

![map1_period](resources/images/maps/map1_period.png)

**Org Units Tab**

![map1_OUs](resources/images/maps/map1_OUs.png)

**Filter Tab**

![map1_filter](resources/images/maps/map1_filter.png)

**Style Tab**

![map1_style](resources/images/maps/map1_style.png)

As the events are grouped together, and you have chosen to style them by sex, we see the doughnut charts when we are zoomed out. As you zoom in however you will start to see the individual locations of each of these events. Select an event to see the details. 

![map1_zoomed](resources/images/maps/map1_zoomed.png)

As we can see, using this layer is the same whether we are using event or tracker data. As with our other analyses, we do have to keep in mind that the event layer will be displaying all the events within a program on this map; so in the case of repeated event data you can have multiple events on the map representing each of these events.

#### Review how to save a map

Go to the file menu and select the "Save" option

![map1_save](resources/images/maps/map1_save.png)

Give the map a name and a description and select "Save"

![map1_save_dialog](resources/images/maps/map1_save_dialog.png)

#### Review how to download a map

Select the download option from within the app. This will open up a new dialog. Position your legend where you want it and select "Download" to download the map. This will download a PNG file of the map to your downloads folder.

![map1_download](resources/images/maps/map1_download.png)

#### STOP! Have them perform *Exercise 1* in the learner's guide.

### Create a map using the TEI layer with relationships

We will now create a map using data from the COVID-19 Case-Based Surveillance Program where we will display relationships on the map.

Open the map "COVID_CBS - Cases and Contacts." This is the map that you will create. It is showing a person along with their relationships. In the context of this program, it means it is displaying index cases along with their contacts. The red circle in the map is the index case (or where the relationship was initiated from) and the black circles are the contacts.

Clear your inputs by going to File -> New.

Create the map using the tracked entity layer with the following inputs:

- Layer 1 Type : Boundary Layer - Vientiane Capital
- Layer 2 Type : Tracked Entity
- Data:
  - Tracked Entity Type : Person
  - Program : COVID-19 Case-base Surveillance
  - Program status : all
- Relationships : 
  - Display tracked entity relationships = yes
  - Relationship type : Has Been in Contact with
- Period :
  - Program/Enrollment date
  - Start/ End Date : January 1, 2022 - September 30, 2022
- Org Units : CHW Mitthaphap
- Style : leave as default


The map should look like this

![map2](resources/images/maps/map2.png)

**Boundary Layer**


![map2_boundary](resources/images/maps/map2_boundary.png)

---

***Tracked Entity Layer***

**Data Tab**

![map2_data](resources/images/maps/map2_data.png)

**Relationships Tab**

![map2_relationships](resources/images/maps/map2_relationships.png)

Explain the relationships tab in a bit more detail as you are configuring this part of the map. This allows you to show relationships between tracked entities, but has a large warning message as it is still in development.

One of the main drawbacks when using the relationship layer is that it only allows you to display relationships within the same program. In our example, we actually have a separate program for registering contacts, but we are not able to display the relationships between the surveillance program and the contacts program; we can only display relationships within the surveillance program (ie. both the cases and contacts must be in this program). Applied more generally, this means that you are only able to display relationships within the same program on the map currently using the tracked entity layer.

**Period Tab**

![map2_period](resources/images/maps/map2_period.png)

**Org Units Tab**

![map2_OUs](resources/images/maps/map2_OUs.png)

**Style Tab**

![map2_style](resources/images/maps/map2_style.png)

Explain the style tab in a bit more detail as you are reviewing it. You can see here you can select the colour of tracked entity, its related entities and the line used to represent the relationship. This allows you to customize the output of these relationship outputs slightly when creating the map layer.

#### Discuss the map output along with limitations of this layer

As we can see, we are able to display tracked entities along with their relationships using this layer. We have already discussed that we are only able to display relationships within the same program currently, but in addition you are not able to apply any event data to filter out the tracked entities that you are showing. Therefore, ***the tracked entity layer can not be combined with any information from the events within a program stage.***

This is unfortunate, as it requires us to collect co-ordinates for every event within a tracker program, rather then just being able to collect the coordinate once and using it in conjunction with our event data.

This is something that is being worked on however and is expected in future releases.

#### STOP! Have them perform *Exercise 2* in the learner's guide.

## Recap

Review the recap slide with them at the end of the session before they perform the assignment

## Assignment

After you have completed all demos and they have finished the exercises, have them complete the graded assignment for this session. If you find you are running out of time, assign the graded assignment to them and ask them to complete it outside of the live scheduled session.