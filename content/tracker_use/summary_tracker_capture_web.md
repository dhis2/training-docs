# Capture - Session Summary

Capture is the primary web application used in DHIS2 for registration and enrollment of tracked entities and capture event data related to them. In addition, the tracked entity dashboard of tracker capture contains multiple widgets that supports adding relationships, providing feedback and displaying program indicators.

Steps to be followed to Open the Capture app

1. Open the URL in your browser
2. Enter the username and password
3. Click on the appes menu in the upper right corner of the screen
4. Search or Click on the capture icon

## Registration and Enrollment

1. Select the program
2. Select an Organisation unit
3. You can now see capture interface with 
* Listing of the registered cases
* Filters, sorting, adding columns, downloading the TEI list
* System generated UIDs (if the program has this configured)

- Register a TEI. 
  - Select the “Create new" button. The label will be slighltly different depending on the tracked entity type. Enter all of the demographic details of the person and click on “Save and Continue” to go to the tracker dashboard.
- The tracker dashboards include:
  * Persistent top bar
  * The buttons at the top of the page
  * Widgets and their descriptions

## Data Entry

- In order to enter data, either select an automatically generated event or create a new event. For each event, start by selecting the event date.
  * You can interact with the data elements for each event. Data elements could be a mix of items, including numerical values, option sets, etc. 
  * Enter all the relevant fields 
  * Complete the event if all of the information has been entered
  * Select “Save” when you are finished

## Adding a Relationship

* Add a “Relationship”
  * Click on Add Relationship.
  * Select the Relationship type and 
  * Select TEI and Save button.

## Enrollment in another program

- In order to enroll the entity in another program
    - From a person's tracker dashboard, select another program
    - If they are not enrolled, you will see a dialogue asking to enroll them in program. Confirm this selection
    - Shared attributes will be carried over between programs. Add in any supplemental information and select "Save."
    - You will be taken to the tracker dashboard in the new program and the person is now enrolled.

## Referrals and Transfer

- You can create one-off events at another facility, refer a person to another facility one-time, or transfer a person permanently
  - One-off events at another location : Select a different organisation unit from the "Registering unit" drop down. Create your new event. It will be in the location you have selected.
  - One-time referrals : Select a different organisation unit from the "Registering unit" drop down. Select "Schedule event" from the quick actions widget. Select the event you want to schedule in the other facility. Select the scheduled date. This will take you back the the tracker dashboard and you will be able to see the scheduled referral.
  - Permanent transfer: From a TEI's tracker dashboard, navigate to the Enrollment widget. Select enrollment actions -> transfer. Select the org unit you want to transfer to. Select "Transfer." You will see the "Owned by" org unit get updated to the new org unit you have selected. The transfer is now complete.



