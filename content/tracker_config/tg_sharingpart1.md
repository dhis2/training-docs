# **Trainer’s guide to Sharing**

## **What is this guide?**

This guide is a support document for DHIS2 Academy trainers for the session “User roles and sharing.” This session follows the standard Academy training approach with
1. a live demo session where the trainer demonstrate and explain the sharing concept and
2. a hands-­on session with exercises where participants get to modify sharing settings.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## **Background**

Sharing can be used in order to provide granular access to meta-data and data as of 2.38. This is a new concept and is an important consideration to define for any tracker implementation. This session should accompany the sharing and user roles presentation that is available here. 

## **Preparation**

Everything in Trainingland has been configured already for you to use in this demo. Just follow the guide using the accounts listed and everything should work as intended. Use the **MAIN** trainingland instance with data, **DO NOT** use the customization instance as this is not configured there.

## **Learning objectives for this session**

* Describe the sharing concept
* Explain the link between sharing and user groups
* Describe the difference between metadata and data sharing
* Identify the objects within a tracker program that can be shared
* Describe the concepts of program and program stage sharing
* Apply program and program stage sharing to your own program

## **Time Requirements**

Live Demo: 1 hr 30 min

## **Quick Guide**

1. Login as the case registration user : casereg/District1#
2. Login as the ANC staff member : ancstaff/District1#
3. Login as the ANC manager : ancmanager/District1#
4. Login as the TB data entry user : tb_entry/District1#
5. Login as the TB analysis user : tb_analysis/District1#
6. Login as the TB admin user : tb_admin/District1#

For each of these users explain the different level of sharing authorities they have and what this allows them to do in relation to the ANC program.

## **Live Demo step by step**

In this demo you will be logging in as 3 different users in order to show that you can configure users to have different levels of access to tracker programs and program stages. 

### Step 1 - Log in as the case registration user

Log in as the first user

Username: casereg

Password: District1#

This user can only register cases and enter data into the first stage of the program. This may be the person at the front desk who is responsible for registering all clients regardless of what service they received.

Note that this user does not have access to any data analysis apps, only tracker capture. This is a result of their user role which will be discussed further later on. The apps they do see are all controlled by their user role.

![](Images/sharing1/image3.png)

Go to tracker capture and select an org unit at the facility level. You will see in this case this user has access to multiple programs as they are responsible for registering patients in all health programs. 

![](Images/sharing1/image17.png)

As this user’s primary role is to register clients, note that the “Register” button exists for this user. Select this button and register a new patient into the Antenatal care program.

![](Images/sharing1/image2.png)

Select save and continue.

This user is unable to create any new events. This will result in an error if this user tries to do so.

![](Images/sharing1/image10.png)

This is controlled via sharing. They have access to view data that is already within a record, so they can look up a person’s record and the information if that is already completed for example in order to reduce duplicate entry, but they can not add any events to the program stages.

### Step 2 - Log in as ANC staff 

Login as the ANC staff member. This user has access to view and edit all the data within all program stages. They are not able to register however, as that is handled by another user type.

Username: ancstaff

Password: District1#

You can see they have access to more apps when compared to the previous user. This is defined through the user role(s) assigned to them.

![](Images/sharing1/image5.png)

When you go to tracker capture with this user and select a facility (select the same facility you registered a mother in using the caereg user), note that they will not see the “register” button at all when within an organisation unit. This is because these users do not have the ability to register new patients. This is reserved for the users in the “Case Registration” user group.

![](Images/sharing1/image11.png)

You will, however, see the new case that the other user has registered. You can select (or search and select) the case you previously registered which will take you to the tracker dashboard. This user will be able to add new events to the program stages

![](Images/sharing1/image15.png)

They can also interact with the data elements as they have the ability to edit the data.

![](Images/sharing1/image6.png)

### Step 3 - Login as the ANC Manager

Login as an ANC manager. This user has access to view and all the data within all program stages. They can not edit any of the stages or register new expectant women however.

Username: ancmanager

Password: District1#

This user has access to the same apps as the ANC staff member. They will likely have the same user roles assigned to them, but this can be confirmed later on. Go to tracker capture and find the same person you have been working on in the other examples. This person can not register cases, similar to the ANC staff member. When you go to the dashboard for the patient you were working with, you will see the ANC manager can see the data for the program stages, but can not edit any of the data.

![](Images/sharing1/image14.png)

Similarly, if they try to add an event, they will see an error.

![](Images/sharing1/image9.png)

The ability to see the data within these program stages but not edit the program stages is controlled via sharing. The ability to see data is not restricted to only tracker capture; they can also view data in the analysis apps. This must be combined with the authority “View event analytics” to view data within the analysis apps. 

```
Both the ANC manager, ANC staff and case registration user have the same permissions to view this data, though this could be changed via sharing if you did not want this to be the case. The case registration user is limited where they can see this data however, as they do not have access to any analysis apps. They could therefore only see the data in the dashboard or through a person's tracked entity dashboard. This could be changed by assigning them the correct user authorities via a user role.
```

#### STOP - Perform Exercise 1 in the learner’s guide


### Step 4 - Login as the TB Data Entry User

Login as the TB data entry user. This user has access to register data and enter data for all of the program stages. 

Username: tb_entry

Password: District1#

As an entry user, they only have access to certain apps

![](Images/sharing1/image3.png)

If we go to tracker capture we can register a new person

![](Images/sharing1/image13.png)

And we can see they can enter data for all of the stages

![](Images/sharing1/image7.png)

### Step 5 - Login as the TB Data Analysis User

Login as the TB analysis user. This user has access to view data for all of the program stages. They also have additional access to analysis apps.

Username: tb_analysis

Password: District1#

This user has access to tracker capture to view records, 

If we navigate to tracker capture we will see they can’t register any records

![](Images/sharing1/image12.png)

If you open a record, they can not edit it either

![](Images/sharing1/image16.png)

They can however run reports

![](Images/sharing1/image4.png)


### Step 6 - Login as the TB Admin User

Login as the TB admin user. 

Username: tb_admin

Password: District1#

This user has access to tracker capture and analysis apps to view records as well as maintenance to edit metadata. It is the only user out of the three that has access to maintenance.

![](Images/sharing1/image1.png)

#### STOP - Perform Exercise 2 in the learner’s guide
