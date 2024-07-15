# Learner's Guide to Capture App (Web-Based)

## What is this guide?

This guide contains all exercises and detailed steps to perform them related to capture app (web-based) session for the academy. Please perform each of the exercises when prompted to by your instructors.

## Learning objectives for this session

The overall objective of this session is to use the DHIS2 capture app. Detailed objectives include:

* Understand how to select the correct program
* Understand the layout and options of capture app
* Understand how to register a TEI
* Understand how to fill in program stage details
* Demonstrate how to search for a TEI in capture app
* Demonstrate how skip-logic can be used in a program

## Exercise 1

### Review the capture interface and options 

In this section we will review program **Electronic Immunization Registry Overview**

1. Open the Capture from the Apps menu

   ![](resources/images/capture/captureimage.png)

2. Find and select the program ("Electronic Immunication Registry")

   ![](resources/images/capture/captureprogramselection.png)

3. Select the site for (Registering unit) in the org unit hierarchy

   ![](resources/images/capture/selectou.png)


The **Electronic Immunization Registry** is linked to any Organization Unit at the health facility level. CH Mahosot has some example cases already entered.

**Note** : Any person that is already registered will be displayed in a tabular fashion, with each row corresponding to a single record.

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

**New feature for Filter:** the capture app will let you filter the list by **Program Stage**, as well as other additional fields, by selecing "More filters" as shown in the image below

![](resources/images/capture/filterstage.png)

You can select the stage and click on update 

![](resources/images/capture/filterstage2.png)

The filter option will now show only filters for **Birth details** program stage.

![](resources/images/capture/filterstage3.png)

#### **Sort an event list**

You can sort the list by clicking the arrow down or up in ascending or descending order.

![](resources/images/capture/sort.png)

#### Predefined list views

You can setup your favorite views which can also be shared with others. A view can be saved by filters, column orders and event sort order. 

This can be done by clickning on **Save current view**.

![](resources/images/capture/saveview.png)


#### **Explain the unique system identifier (EPI)**

System generated ID’s can follow patterns that are defined by the user. This example uses the “"EPI_ + Random Number”

![](resources/images/capture/uniqueidentifier.png)

Go to the registration page and see that the ID will be generated. These ID’s can be a bit dynamic depending on the pattern that is defined to generate them. You can use inputs such as the date (used in this example), org unit codes, etc. The best resource to learn more is here:
[https://docs.dhis2.org/master/en/user/html/working-with-textpattern.html](https://docs.dhis2.org/master/en/user/html/working-with-textpattern.html)

### Register a TEI into the Electronic Immunization Registry Program

There are two ways of registering a TEI under an organization unit.

1. The first way is to register a tracked entity instance without enrolling it to a tracker program.

2. The second options is to register a tracked entity instance with program and enroll it.

In this exercise, we will focus on registering a TEI within a program.

1. Open the capture app
2. Select the program "Electronic Immunization Registry"
3. Select an organisation unit
4. Select New -> New person in Electronic Immunization Registry

![](resources/images/capture/reg2.png)

> Note: The label of this button corresponds to the tracked entity type of the program, which will vary depending on the tracked entity type (ie. in this case we see new person, as person is the TET)

Now you will be able to see the registration page for the Immunization program

   ![](resources/images/capture/regpage2.png)

   It will display different information the way the enrollment page is customized for the program.

   In this form you have section for enrollment which shows enrollemnt date and then you have profile secction which is to capture demographic information.

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

#### Duplicates during registration

Navigate back to the TEI front page list in capture by closing the person you just registered.

![](resources/images/capture/close_enrollment.png)

Proceed to register a new TEI using the same process as before (ensure the program and registering unit are selected then select New - New person in Eletronic Immunization Registry)

Try to register a person with the following details

- Given Name : Diane
- Last Name : Miller
- Primary contacts first name : Elizabeth
- Primary contacts last name : Hardy

When you select Save person, you should see the following dialogue.  

![](resources/images/capture/duplicate.png)

It has identified this as a possible duplicate. You have options to view the dashboard, which will take you to this persons dashboard for review, to cancel so you do not register this person, or to save as new, which will overrride the warning and save the TEI.

In real life scenarios, it will be important to implemenet as many procedures as possible to reduce duplicates. This feature can help with reducing duplicates at the sources. We will also discuss how to search for TEIs later on in this session.

## Exercise 2

### Searching

Find the new tracked entity that we had previously registered. 

From the main list page in capture, select Search - > Search for a person in Electronic Immunization Registry.

![](resources/images/capture/main_search.png)

The search page will then be seperated into a couple of options.

![](resources/images/capture/initial_search.png)

First, you will see the tracked entity attributes that are identified as unique. This is what we see in options 1 and 2 in the image above. 

Next, in 3, we will see the "search by attributes" option. This allows us to search using any of the other tracked entity attributes that have been configured to allow search in this program. 

Where possible, using a unique identifier will yield the best results when searching. For example, I can enter the EPI unique ID and I will quickly find the person I previously registered.

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
   
### Description of Tracker Dashboard

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

6. **Person Profile** - This is to edit TEI's profile or attributes. 

7. **Enrollment** - The enrollment widget shows key details regarding the enrollment. A number of actions can also be completed via this widget related to the enrollment including:

- Change the enrollment status to Active, Canceled or Completed using the buttons in the menu.
- Mark or remove the enrollment for a follow-up.
- Transfer the enrollment to another organisation unit
- Delete the enrollment
- Add coordinates to the enrollment

## Exercise 3

### Data Entry

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

#### Add a Relationship

To perform this step we will refer to **Contact tracing program**

In the capture app ,Relationships is only supporting Event to Tracked entity relationships.

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

##### Adding a relationship by Creating a new Tracked Entity.

1. Click on **Create new Tracked Entity Instance**.
2. You will be presented with a form for registring a new person.You can choose to register this person with or without enrollement to the program
3. You can change the Organisation unit by removing the one that is automatically set and selecting a new one.

    ![](resources/images/capture/relationship2.png)

    ![](resources/images/capture/relationship8.png)




