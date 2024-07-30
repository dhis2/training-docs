# Trainer’s guide to Capture

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session “Demonstrating and using Capture App (Web).”

This session follows the standard Academy training approach with: 
 
1. A live demo session where the trainer demonstrates and explains the features, and 

2. A hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheat sheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## Learning objectives for this session

The overall objective of this session is to use the DHIS2 capture app. Detailed objectives include:

* Understand how to select the correct program
* Understand the layout and options of capture app
* Understand how to register a TEI
* Understand how to fill in program stage details
* Demonstrate how to search for a TEI in capture app
* Demonstrate how skip-logic can be used in a program

### Time Requirements

Live Demo: 1.5 hours

Hands-on Exercises: 1.5 hours

## Background

In the Capture app you register events that occurred at a particular time and place. An event can happen at any given point in time.

Events are sometimes called cases or records. In DHIS2, events are linked to a program.

The Capture app lets you select the organisation unit and program and specify a date when an event happened, before entering information for the event. Some events are linked to a tracked entity instance, for example a person, allowing longitudinal follow-up.

As programs are entered on an individual basis, program based data is entered based on the report or enrollment date as defined by the programs requirements. Tracker capture by design is not anonymous in nature, and therefore person details are attached to each event.

In this demo, the **Electronic Immunization Registry** and **Malaria Case Notification, Investigation and Response** demo programs that have been created will be used to demonstrate the features of capture app.
 
## Preparations

Ensure that there are existing records in the demo DB and that you are able to register TEI's and enter event data correctly.

You should consider running through the entire demo prior to presenting it. After this, you should take the quick guide and supplement it with any additional notes you made while running through the demo. If you identify any changes that may be required or additional explanation that would be helpful within the session, please contact the capacity building team in order to allow us to evaluate how to best integrate this feedback into the material.

Also, the learner's guide and session summary are the main material that will be provided to the learner's with both detailed steps for ungraded exercises as well as the key messages from the session. Review these as well to ensure you are able to get these key points across during your demonstration.

## Best Practices

Before starting the demonstration, please keep in mind that the most important thing is that the audience is following, so make sure to ask questions to the audience to verify that they are following. If something is unclear, go back and go through it slowly. If you don’t have time for all the steps, it is better to cut some steps, than to go fast while nobody understands. 

Prior to starting the actual demo, It is a good idea to do a quick overview of the stages and program flow so everyone understands the use-case clearly.

In an online setting, you will be breaking regularly to allow them to perform various ungraded exercises in order to keep them engaged.

If the participants are doing the demo with you at the same time, you can take time to go around the audience and help them if the academy is happening onsite. There should be a team of trainers doing this at all times as well.

## Quick Guide

1. Explain the capture interface and options
   1. Select the EIR (Electronic Immunization Registry) program in capture
   2. Review the initial working list; modify the working list by selecting filters and adding columns
2. Register a new case into the EIR program
3. Review how duplicates are detected during registering. Use these details:
   - Given Name : Diane
   - Family Name : Miller
   - Date of Birth : 2020-06-25
   - Primary contacts first name : Elizabeth
   - Primary contacts last name : Hardy

STOP - Perform Exercise 1

4. Search for an existing person. Use the EPI unique ID EPI_62466
5. Search for an existing person using attributes:
   1. Given name : Jake
   2. Last name : Smith
   3. Sex : Male
6. Review the options that appear when searching for a person using attributes.

STOP - Perform Exercise 2

8. Enter data into the birth details stage
9. Explain why you can't create more events in the birth details stage
10. Create a new event in the immunization stage.
    1.  Fill in data for the event. Explain the program rules associated with the program as you do so.
11. Schedule an event in the immunization stage (6 weeks or more from the 1st stage)
12. Review the event to see how program rules affect which vaccines are available
13. Add a relationship using the contact tracing program
    1.  Create a relationship with an existing person
    2.  Create a relationship by making a new TEI

STOP - Perform Exercise 3

14. Enroll a person from the contact tracing program into the case-based surveillance program
15. Find the record James Dawson in the ***Case Based Surveillance Program*** using the System Case ID : FIB112660
16. Review the person profile widget and associated actions.

STOP - Perform Exercise 4

17. Explain the concept of referrals and transfers. 
    1. Register a new TEI in the surveillance program
    2. Create a single event in a different location then the one you registed them in
    3. Create a one-time referral by scheduling an event in a different location
    4. Transfer the TEI to another org unit

STOP - Perform Exercise 5

## Live Demo step by step

### Part 1 - Explain the capture interface and options 

**Electronic Immunization Registry Overview**

1. Open the Capture from the Apps menu

   ![](resources/images/capture/captureimage.png)

2. Find and select the program ("Electronic Immunication Registry")

   ![](resources/images/capture/captureprogramselection.png)

3. Select the site for (Registering unit) in the org unit hierarchy

   ![](resources/images/capture/selectou.png)


The **Electronic Immunization Registry** is linked to any Organisation Unit at the health facility level. CH Mahosot has some example cases already entered.

> **Note** 
>
> Any person that is already registered will be displayed in a tabular fashion, with each row corresponding to a single record. You can display this list in program maintenance when you configure your program if needed.
 
   ![](resources/images/capture/capturehomepage.png)

**Enrollment status filters:** If a program is selected, the app provides further filtering on the table based on enrollment status. This is displayed in the following order:

You can filter the list based on enrollments: 
* Active,
* Completed,
* Cancelled.

#### Modify an event list layout - Select columns to show:

You can select which columns to hide or show and rearrange them in the event list by selecting the settings/gear icon.

![](resources/images/capture/settings.png)

From here, you can reorganize the order of the program inputs by dragging and dropping them within the list.

![](resources/images/capture/columnstoshow.png)

#### Filter an event list

**New feature for Filte:** the capture app will let you filter the list by **Program Stage**, as well as other additional fields, by selecing "More filters" as shown in the image below

![](resources/images/capture/filterstage.png)

You can select the stage and click on update 

![](resources/images/capture/filterstage2.png)

The filter option will now show only filters for **Birth details** program stage.

![](resources/images/capture/filterstage3.png)

#### Sort an event list

You can sort the list by clicking the arrow down or up in ascending or descending order.

![](resources/images/capture/sort.png)

#### Predefined list views

You can setup your favorite views which can also be shared with others. A view can be saved by filters, column orders and event sort order. 

This can be done by clickning on **Save current view**.

![](resources/images/capture/saveview.png)


#### Explain the unique system identifier (EPI)

System generated ID’s can follow patterns that are defined by the user. This example uses the “"EPI_ + Random Number”

![](resources/images/capture/uniqueidentifier.png)

Go to the registration page and see that the ID will be generated. These ID’s can be a bit dynamic depending on the pattern that is defined to generate them. You can use inputs such as the date (used in this example), org unit codes, etc. The best resource to learn more is here:
[https://docs.dhis2.org/master/en/user/html/working-with-textpattern.html](https://docs.dhis2.org/master/en/user/html/working-with-textpattern.html)

**After you have explained the interface options, proceed to register a TEI into the program.**

### Part 2 - Registration

The capture app now has more support for tracker programs than before. Users will now be able to list and interact with tracked entity instances much in the same way as events, and will have access to searching and registering/enrolling tracked entity instances in the Capture app itself. This will allow data entry user to access tracker and event data in the same place, and have a more integrated workflow.

**Register a TEI into the Electronic Immunization Registry Program** 

There are two ways of registering a TEI under an organization unit.

1. The first way is to register a tracked entity instance without enrolling it to a tracker program.

2. The second options is to register a tracked entity instance with program and enroll it.

In this demo, we will focus on registering a TEI within a program.

1. Open the capture app
2. Select the program "Electronic Immunization Registry"
3. Select an organisation unit
4. Select Create new person

![](resources/images/capture/reg2.png)

> **Note**
>
> The label of this button corresponds to the tracked entity type of the program, which will vary depending on the tracked entity type (ie. in this case we see new person, as person is the TET)

Now you will be able to see the registration page for the Immunization program

   ![](resources/images/capture/regpage2.png)

It will display different information depending on the way the enrollment page is customized for the program.

In this form you have section for enrollment which shows the enrollment date and then you have the profile secction which is used to capture demographic information.

5. Review the TEI registration page

As you navigate the fields notice the exclamation icon next to the field names. If you hover over this, you will see a description of the field.

![](resources/images/capture/field_description.png)

Fields that have a red star next to them indicate they are mandatory and must be filled in.

![](resources/images/capture/mandatory_fields.png)

Fill in the fields and save the person when you are ready

   ![](resources/images/capture/savereg.png)

6. You will then see the tracked entity dashboard.

![](resources/images/capture/savereg2.png)

The dashboard will show relevant information about the newly created tracked entity instance.
Both skip-logic and validation error/warning messages are supported during registration.

In later sessions, you will go over the terminology in more detail so just focus on describing the interface and actions for now. 

#### Duplicates during registration

Navigate back to the TEI front page list in capture by closing the dashboard of the person you just registered.

![](resources/images/capture/close_enrollment.png)

Proceed to register a new TEI using the same process as before (ensure the program and registering unit are selected then select New - New person in Eletronic Immunization Registry)

Try to register a person with the following details

- Given Name : Diane
- Family Name : Miller
- Date of Birth : 2020-06-25
- Primary contacts first name : Elizabeth
- Primary contacts last name : Hardy

When you select Save person, you should see the following dialogue.  

![](resources/images/capture/duplicate.png)

It has identified this as a possible duplicate. You have options to:

1. View the dashboard, which will take you to this persons dashboard for review
2. To cancel so you do not register this person
3. To save this person as a new TEI, which will overrride the warning and save the TEI.

In real life scenarios, it will be important to implemenet as many procedures as possible to reduce duplicates. This feature can help with reducing duplicates at the source. We will also discuss how to search for TEIs later on in this session.

**STOP - Perform Exercise 1** 

### Part 3 - Searching

Let us now find the new tracked entity that we had previously registered. 

From the main list page in capture, select Search - > Search for a person in Electronic Immunization Registry.

![](resources/images/capture/main_search.png)

The search page will then be seperated into a couple of options.

![](resources/images/capture/initial_search.png)

First, you will see the tracked entity attributes that are identified as unique. This is what we see in options 1 and 2 in the image above. 

Next, in 3, we will see the "search by attributes" option. This allows us to search using any of the other tracked entity attributes that have been configured to allow search in this program. 

Where possible, using a unique identifier will yield the best results when searching. For example, I can enter the EPI unique ID (EPI_62466) and I will quickly find the person I previously registered.

![](resources/images/capture/unique_search.png)

If I select "Search by Unique System Identifier (EPI)" and I have the correct ID, it will take me directly to the persons dashboard. 

A more common method may be to use the "Search by attributes" feature. 

![](resources/images/capture/attribute_search.png)

If I enter these details and select "Search by attributes", I will then by shown a list of results in which I can select the correct TEI based on the attributes I have entered

![](resources/images/capture/attribute_results.png)

1. View dashboard: this will take me to the persons tracker dashboard
2. View active enrollment: this will open the dashboard and take me to the active enrollment in the program
3. Search in all programs: if the TEI I searched for is not in the program I have selected, I can also search in every program to make sure I do not duplicate this TEI
4. Create new: if the TEI I searched for does not exist, then I can create a new one based on the search details I entered

In this example, select "view dashboard" to open the persons tracker dashboard.
   
### Part 4 : Describe the Tracker Dashboard

![](resources/images/capture/enrollment_dash1.png)

The dashboard starts with the following items:

1. **Top Bar/Header** - The top of the dashboard defines your context. For example in the image below the context is as follows, the selected program is "Electronic Immunization registry", the organisation unit is "CH Mahosot", the selected person is "Logan Stewart" and the enrollment date is "2024-03-26".
2. **Quick Actions** - The widget will show the frequently used actions for the current enrollment.
3. **Program stage list** - Stages can be collapsed or expanded to reveal the events inside.

   **Collapsed stages:** In the collapsed state, you can view the summary information about stage including: 
   - Icon 
   - Program stage name 
   - Program stage description (on hovering the information icon) 
   - Total number of events - Last updated date Depending on the status of events, there can be additional information regarding: total number of overdue events or total number of scheduled events.

   ![](resources/images/capture/collapsedstage.png)

   **Expanded Stages:** 

   When you expand the list, you will see the table contains the data of events in the stage. 
   This includes mandatory columns:
   - Status, 
   - Report date and 
   - Registering unit, 
   - the following columns depend on the data elements that have been selected as Display in list of event.

   Events are sorted with most recent on top and other columns are also sortable.

   ![](resources/images/capture/expandedstage.png)

4. Widget Descriptions

![](resources/images/capture/widgets.png)

1. **Stages and Events** - This is for doing data entry using either default or custom forms. Depending on the program definition, in particular program stages and events will be displayed. 

2. **Person Relationships** - This helps to relate the selected TEI (the one whose dashboard is shown) to another TEI depending on the relationships that are defined in the system.

3. **Comments about enrollment** - This is to allow you to make any general comments on the enrollment of the TEI.

4. **Indicators** - Any indicator defined for the selected program will have its value calculated and displayed under this widget.

5. **Feedback** - In this widget you can place summary information about the TEI for review. For example if the person has allergies or you want to display information on which vaccines they have received until now you can place this information here based on what has been entered in the program

6. **Person Profile** - This is to edit TEI's profile or attributes. You can also delete the TEI using this widget if the person has the appropirate level of access.

7. **Enrollment** - The enrollment widget shows key details regarding the enrollment. A number of actions can also be completed via this widget related to the enrollment including:

- Change the enrollment status to Active, Canceled or Completed using the buttons in the menu.
- Mark or remove the enrollment for a follow-up.
- Transfer the enrollment to another organisation unit
- Delete the enrollment
- Add coordinates to the enrollment (if the enrollment is configured to capture coordinates)

We will discuss some of the personal profile and enrollment actions later in this session.

**STOP - Perform Exercise 2**

### Part 4 - Data Entry Steps

- To start entering data you need to select a stage and click on **"New Event"** for a stage. Events can also be automatically generated upon enrollment, which is the case in our example program.

- In cases where the event is automatically generated you can select the event in order to start entering data into the program stage.

 ![](resources/images/capture/new_event.png)

- Select the Date and fill out the data. 

 ![](resources/images/capture/complete_event.png)

 1. Select a report date
 2. Fill in the data for the event
 3. Complete the event
 4. Select save

  ![](resources/images/capture/saved_event.png)

After saving the event, you will see a summary of the event you have saved. From here, you can select "Back to all stages and events" in order to proceed.

Note that the option to add a new birth details event is now greyed out. This is because this is a non-repeatable program stage, meaning it can only have one event within the stage.

If an event is not automatically created, then you will have to make a new event. This is the case in the "Immunization" program stage. Select "New Immunization event" to create a new event for this stage.

![](resources/images/capture/create_event.png)

From here, we follow the same steps as before to fill in information for the event. 

![](resources/images/capture/imm_event.png)

Note that you only see the vaccines that are given at birth in this initial event. This is a result of program rules that have implemented a vaccination schedule based on the child's date of birth.

As the immunization stage is repeatable (a person will attend multiple vaccination events over time) We can schedule the next vaccination visit by selecting "schedule an event" from the tracker dashboard.

![](resources/images/capture/schedule_event.png)

It will give you a suggested date based on the program configuration; however you can change this if needed. As the next routine dose is typically 6 weeks after birth, select a date 6 weeks or beyond the date of birth. Select "Schedule" to schedule the event. This will take you back to the tracker dashboard, where you will see the event listed along with the expected visit date.

![](resources/images/capture/next_event.png)

If you quickly open this event up and select a date 6 weeks from the date of birth, you will now see the next routine doses in the schedule.

![](resources/images/capture/imm_rules.png)

In summary, the data entry process is as follows.

1. Register a new TEI if it doesnt exist
2. Find an existing TEI if it does exist
3. Review the stages and events section of the tracker dashboard
4. Update automatically generated events or add new events as needed
5. For repeatable stages, events can be scheduled as well as being created as needed

### Part 5 - Add a Relationship

To perform this step we will refer to **Contact tracing program**

1. While you are in an event,Click Add Relationship
2. Selct the relationship you want to create.

    ![](resources/images/capture/relationship.png)

3. Select a New TEI Relationship

   ![](resources/images/capture/relationship1.png)

4. You now will get two options:
  * Link to an existing tracked entity instance
  * Create new tracked entity instance

    ![](resources/images/capture/relationship2.png)


#### Adding a relationship by Linking to an existing person.

1. Click on **Link to an existing person**. You will see a Program search option where you can select a program where you want to search your TEI.

2. Once you select a program , attributes will be seen to filter down the search for the existing tracked entity. You can search for attributes or by system generated ID

    ![](resources/images/capture/relationship3.png)

3. You can also narrow down the search by clicking on the "Organisation Unit Scope"

    ![](resources/images/capture/relationship4.png)

4. After a Search you will be presented with a list of Tracked Entity Instances matching the search criteria. To create a relationship click the **Link** button on the Tracked Entity Instance you would like to create a relationship to.

    ![](resources/images/capture/relationship5.png)

5. You will see the new relationship has been added under relationship widget in the personal dashboard 

    ![](resources/images/capture/relationship7.png)

#### Adding a relationship by Creating a new Tracked Entity.

1. Click on **Create new Tracked Entity Instance**.
2. You will be presented with a form for registring a new person.You can choose to register this person with or without enrollement to the program
3. You can change the Organisation unit by removing the one that is automatically set and selecting a new one.

    ![](resources/images/capture/relationship2.png)

    ![](resources/images/capture/relationship8.png)

#### STOP - Perform Exercise 3

### Part 6 - Enrolling a person in multiple programs

Any TEI in the system can be enrolled in multiple programs. This is a function that can be quite useful if you want to track all of the services a single entity has received. In health, as an example, you may want to track all of the health services a single patient has been provided. 

To perform this demo, you can use the contact tracing and case-based surveillance programs, simulating what could happen when a contact becomes a case. 

Start by registering a person in the contact tracing program in any org unit. 

Go into the follow-up visits stage and enter some symptoms for the person, just to indicate they are now a case to be enrolled into the case-based surveillance program. When you are done save the event.

![](resources/images/capture/follow_up.png)

Now let us take this person and enroll them into the case-based surveillance program.

From the persons tracker dashboard, select the program dropdown then the case-based surveillance program.

![](resources/images/capture/select_program.png)

You will receive a message that they are not enrolled in this program. Select the option to enroll them in the program.

![](resources/images/capture/not_enrolled.png)

After selecting this button, it will take you to the registration page of the program that you have selected. Any of the tracked entity attributes that you have previously entered and are shared between programs will be automtically populated (ie. you wont need to enter these details again). 

![](resources/images/capture/re_enroll.png)

Fill in any of the missing details and select "Save person" at the bottom of the screen. 

This will take you to the person's tracker dashboard in the new program. The person has now been enrolled into the new program succesfully.

### Part 7 - Widget Actions

To review this session, find James Dawson in the ***Case Based Surveillance Program*** using the System Case ID : FIB112660

When we open this record, we will be able to see responses for within the widgets of the TEI dashboard. We will see the feedback populated with the initial diagnosis as well as an indicator showing the number of lab results. This person also has a relationship.

Let us focus on two parts of the widget area to explain them further.

1. The person profile.
2. Enrollment actions.

#### The person profile

In the person profile, you are able to edit the person's attributes. You can do this by selecting "Edit" in this widget. This will bring up their profile where you can edit their attributes.

![](resources/images/capture/edit_person.png)

You can also delete a TEI from this menu by selecting the three dots followed by "Delete"

![](resources/images/capture/delete_tei.png)

You need to be very mindful of this authority as this will delete the TEI, along with all of its enrollments and related events. A warning box will come up if you select this option to confirm you really want to delete it.

![](resources/images/capture/delete_tei_warning.png)

> **Important**
>
> You are able to disable permission of users to delete TEIs. You do this through managing user roles. There is an authority specifically meant to control this.
>
> ![](resources/images/capture/tracker_authorities.png)
>
> If a user does not have this authority, the option to delete a person will be greyed out.
>
> ![](resources/images/capture/no_delete.png)

#### STOP - Perform Exercise 4

### Part 8 - Referrals and Transfers

You can perform referrals/have a single event in a different location as well as perform a permanent transfer in the capture app. How this is done is a bit different when compared to tracker capture. 

Lets start with reviewing a single event in a different location. We can do two operations essentially.

1. We can create an event in a different org unit at the time of data entry
2. We can schedule an event in a different org unit, similar to the previous referral functionality

#### Single event in a different location

Let us start by crating an event in a different org unit at the time of data entry.

***To do this, start by registering a new person in any org unit in the Case based surveillance program.***

After registering the person, scroll down and review the enrollment widget.

![](resources/images/capture/enrollment_widget.png)

You will see two fields here:

- Started at
- Owned by

This fields are where the person was initially registered, and where the enrollment is currently owned by. We will come back to this widget later on in this part of the demo.

This program consists of 5 stages

![](resources/images/capture/program_overview.png)

Upon registration, one event is automatically generated in the diagnostic and clinical information stage, ***at the same org unit in which you initiated the registration.***

Other subsequent events can happen in the same org unit or in other org units depending on where services are provided. 

As an example of this, the lab result and/or final classification could occur at a different facility (it seems less likely the lab request and tracking would occur from a different facility in this scenario).

For the sake of demonstration, even though none of the events are filled in or have data, we could enter information on the lab result simulating that this is occuring at another facility.

To start this process, from the persons dashboard, first select the "registering unit" dropdown then select a different facility the the one you enrolled the person in.

![](resources/images/capture/referral1.png)

Next, lets create a new event in the lab results stage. Enter in some details and save the event. You will then be taken back to the persons dashboard.

Review the event. If you compare it with your enrollment widget, you will see the event is located in a diffferent org unit.

![](resources/images/capture/referral2.png)

#### One-time referral

Setting up a single event in a different location at the time of data entry can be useful if this is unexpected (ie. they just show up at a facility to receive service) or a person is not sure where the next event is occurring, but you can also schedule a referral if you know where the next event is going to take place.

Make sure your registering unit is still different then your started/owned by org unit as seen in the enrollment widget.

Then, select "Schedule an event" from the quick actions toolbar in the person's dashboard.

![](resources/images/capture/schedule_referral.png)

From here, you will be able to select the program stage you are scheduling an event for.

![](resources/images/capture/schedule_referral2.png)

Select the final classification stage.

From here, you will be able to schedule the anticipated date of this event. In this example, we are scheduling when the final classification should take place by.

![](resources/images/capture/schedule_referral3.png)

Select the scheduled date, followed by "Schedule" to schedule the event in the facility you have selected.

This will take you back to the person's dashboard. You will now see an event scheduled in the facility you have selected, which is different from the facility they were enrolled into.

![](resources/images/capture/schedule_referral4.png)

#### Transfers

In addition to having a single event in a different location, either by doing this at the time of data entry or scheduling the event, you are able to perform a permanent transfer of a person to an other organisation unit. 

This could be useful if they are no longer receiving any services in the initial organisation unit they were enrolled in for example. 

To perform a permanent transfer, you can take the person you registered into the case based surveillance program.

Navigate down to the enrollment widget and

1. Select enrollment actions
2. Select transfer

![](resources/images/capture/transfer1.png)

From here, the organisation unit selection panel will appear. You can then select which org unit you want to transfer this person to.

![](resources/images/capture/transfer2.png)

Select transfer when you are ready to transfer the person.

Review the enrollment widget of this person, it should be updated. The "started by" and "owned by" organisation units will now be different.

![](resources/images/capture/transfer3.png)

This indicates the ownership of this person has been transferred to the new org unit.

> **Note**
>
> This has some implications on analytics, relating to the ownership organisation unit. Enrollment type analytics will be counting enrollments based on the "owned by" org unit, and enrollments in line lists will be displayed based on the "owned by" org unit as well.
>
> This also has some affect on data entry/user access. A user that has capture access to the organisation unit that is the current owner of the TEI/Program will have write access to all enrollments for that TEI/Program combination. A user that has search access to the organisation unit that is the current owner will have access to search and find the TEI/Program combination.

#### STOP - Perform Exercise 5

### Review the recap slide

## Assignment

After you have completed all demos, they have finished the exercises and you have reviewed the recap slip, have them complete the graded assignment for this session. If you find you are running out of time, assign the graded assignment to them and ask them to complete it outside of the live scheduled session.