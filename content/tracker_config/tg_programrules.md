# **Trainer’s guide to Program Rules**

**_CREATE THE RULES for TB in CONFIG._**

## **What is this guide?**

This guide is a support document for DHIS2 Academy trainers for the session “Program Rules.” This session follows the standard Academy training approach with 

   1. a live demo session where the trainer demonstrate and explain how to create program rules, and
   2.  a hands-­on session with exercises where participants get to create program rules.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## **Learning objectives for this session**

The overall objective of this session is to demonstrate how to create program rules in DHIS2 for both event and tracker programs. Detailed objectives include:

* Define the program rules concept
* Create program rules using variables, expressions and actions in DHIS2

## **Time Requirements**

Live Demo: 1.5 hours

Assignment: 1 hour

## **Background**

Program rules allow you to create and control dynamic behavior of the user interface in the Tracker Capture and Event Capture apps. Program rules gives functionality to configure dynamic behavior in the programs in DHIS2 that are implemented on the paper forms through skip logic, warnings and patterns as well as auto filling some fields.

## Preparations

Decide how you would like to run the session. The guide has you alternating between introducing the rule concept followed by creating a rule together with the participants. It is important to gauge your participants to see how much additional guidance they need as this topic is always problematic due to the number of new concepts introduced combined with the participants desire to learn complex rules immediately. YOU CAN PERFORM THIS IN THE DEMO SYSTEM, as this as both programs configured for you. 

## **Quick Guide**

1. Create a program rule using the TB Treatment Card Program
    1. Hide the EPTB Field when the disease site is Pulmonary
    2. Test the rule

STOP - Have the participant’s perform Exercise 1 in the learner’s guide

2. Create a program rule using the TB Treatment Program
   
    1. If sex is Male then hide Pregnant
    2. Test the rule

STOP - Have the participant’s perform Exercise 2 in the learner’s guide

3. Create a program rule using the TB program
   
    1. If the weight is &lt;=5 or >= 140 display a warning message
    2. Test the rule

STOP - Have the participant’s perform Exercise 3 in the learner’s guide

4. Create a program rule using the TB Treatment Card Program
   
    1. Show the disease site in the feedback
    2. Test the rule

STOP - Have the participant’s perform Exercise 4 in the learner’s guide

5. Create a program rule using the TB Treatment Card Program
   
    1. Calculate the patient’s age based on the Date of Birth
    2.  Test the rule

STOP - Have the participant’s perform Exercise 4 in the learner’s guide

## Program Rules Reference

In reality, it is difficult to remember all of the rule operators and actions that are possible to use. It is likely you will need to reference the [documentation](https://docs.dhis2.org/en/use/user-guides/dhis-core-version-master/configuring-the-system/programs.html#configure_program_rule) from time to time as it is a useful resource regarding what types of expressions, operators and actions you can use. 

## Live Demo step by step

In order to create a program rule, we can follow these general guidelines:

1. Conceptualise the logic of the rule you want to create
2. Create a program rule variable that points to the data element/attribute which will trigger your logic
3. Create a new program rule
    1. Fill in the program rule details
        1. Select the program
        2. Provide a name and description
        3. Assign a priority if applicable
4. Enter the program rule expression
    2. Refer the the [documentation](https://docs.dhis2.org/en/use/user-guides/dhis-core-version-master/configuring-the-system/programs.html#configure_program_rule) to see many examples of the items that can be used within the expression, as well as examples of expressions
5. Define the program rules actions
    3. Refer to the [documentation](https://docs.dhis2.org/en/use/user-guides/dhis-core-version-master/configuring-the-system/programs.html#configure_program_rule) for more detail on each individual action
6. Clear your cache and test the 


## **Rule 1 -** In the first example, we will create a program rule for the TB program which hides the “EPTB Site” data element if the TB is not classified as extra-pulmonary.

**You should start this session by presenting ONLY Slides 1-4 here:**

(https://docs.google.com/presentation/d/1igu8J5ybDOPHJnxMX6n5Ah2gHhL1Ri54v9lX4ZvZGSA/edit#slide=id.g3bdf14aaf4_0_0)

### Step 1 - Access the Program and attribute app

**Log into the blank instance and go to Maintenance App**

![](Images/pr/image18.png)

**and click on Program**

![](Images/pr/image2.png)

NOTE: To create a new program rule, you may need to first create Program rule variables

### Step 2 - Create the program rule variable

You can explain the concept of a variable using slides 6-7

(https://docs.google.com/presentation/d/1igu8J5ybDOPHJnxMX6n5Ah2gHhL1Ri54v9lX4ZvZGSA/edit#slide=id.g3bdf14aaf4_0_0) 

**To create a new program rule variable, you need to first create Program rule variables**

**Click on Program rule variable and Add**

![](Images/pr/image25.png)

* **Use code for option set**: When your variable is using an option set, this allows you to select whether or not you will use the option set code rather than the value when creating your program rule expressions. It is often useful to use the code as this is less subject to change than the value. You may not want to use the code however if you are displaying feedback of some kind for example.
* **Source type:** The source type is determining how the source field is populated with a value. Please refer to the [documentation](https://docs.dhis2.org/en/use/user-guides/dhis-core-version-master/configuring-the-system/programs.html#configure_program_rule) for the latest info.

The majority of the time you will be using “data element in current event” or “Tracked entity attribute” however there are uses for the other fields. We can explain them further in additional examples. 

### Step 3 - Create the program rule

**To create a new program rule, Click on Program rule and Add (the “+” **symbol)**

**Enter Program rule details**

![](Images/pr/image8.png)

Do not worry about the priority for now. This will be covered in other trainings/academies.

**Enter the Program rule expression**

You can refer to Slide 8 and 9 on expressions and operators:
(https://docs.google.com/presentation/d/1igu8J5ybDOPHJnxMX6n5Ah2gHhL1Ri54v9lX4ZvZGSA/edit#slide=id.g3bdf14aaf4_0_0) 

**Create an expression #{TBDiseaseSite_current} == ''  || #{TBDiseaseSite_current} == 'Pulmonary'**

Recall the operators from the documentation that are now present along the bottom row and go through a quick refresher on what these mean.  You will be using an expression that includes the **equals to** and **OR** logical operators.

![](Images/pr/image38.png)

**Create the action (“Hide Field” on EBTB Site Data Element).**

**At this stage explain the various actions that are available once again.**

The full list of actions can be viewed in the [documentation](https://docs.dhis2.org/en/use/user-guides/dhis-core-version-master/configuring-the-system/programs.html#configure_program_rule). 

![](Images/pr/image16.png)

**and click on COMMIT to save. SAVE the program rule before continuing.**


### Step 3 -Test the Program Rule

You may need to clear your cache or reload in incognito mode so the rule works correctly.

**Go to tracker capture to show the rule in action**

![](Images/pr/image36.png)

**Register a new person**

![](Images/pr/image27.png)

**We can see immediately that the rule is working, as there is no value for disease site and the EPTB site data element is hidden.**

Selecting Pulmonary yields the same result

![](Images/pr/image11.png)

Only when we select Extra Pulmonary does the EPTB site data element appear. This is the intended action of the rule.

![](Images/pr/image32.png)

Note that if you select an EPTB site

![](Images/pr/image4.png)

However go back and change the TB Disease site to Pulmonary

![](Images/pr/image19.png)

You will get an error message saying that the EPTB Site value was deleted. The logic here is that unless the disease site is extra-pulmonary, the EPTB site value is hidden and therefore can not have a related value entered within it.

![](Images/pr/image12.png)

### STOP - Have the participant’s perform Exercise 1 in the learner’s guide

## **Rule 2 -** Create a program rule to hide pregnant if Gender is Male using the TB Program

**Access the Programs rules from Maintenance App ⇒ Program**

**Log into the blank instance and go to Maintenance App**

![](Images/pr/image18.png)

**and click on Program**

![](Images/pr/image2.png)

**Add in a new program rule variable**

![](Images/pr/image37.png)

**Create a Program Rule**

Hide pregnant if sex is Male

Enter the program rule details.

In the expression, we are using option from Gender that we have created 

![](Images/pr/image39.png)

**Test the rule with the participants**

Clear the cache if needed, than go to tracker capture to test the rule

Pregnant should be hidden if sex is Male

![](Images/pr/image34.png)

It should show 

![](Images/pr/image7.png)

### STOP - Have the participant’s perform Exercise 2 in the learner’s guide

## Rule 3 - Create another program rule for the TB Treatment Card which displays a warning message when Weight is out of range

**Access the Programs rules from Maintenance App ⇒ Program**

**Log into the blank instance and go to Maintenance App**

![](Images/pr/image18.png)

**and click on Program**

![](Images/pr/image2.png)

**Add in a new program rule variable**

Weight, data element in current event, Weight (in kg)

![](Images/pr/image14.png)

## Create the program rule

**Provide the Program rule details**

![](Images/pr/image24.png)

In the expression, we combine several principles to create our output by using the a custom function, the “AND” and “OR” logical operators as well as brackets to define the extreme ranges of the weight value. As weight is a numerical value, we can apply logic similar to a validation rule in order to determine which values we consider out of range. Make sure to explain everything that you are doing to the participants (why brackets are important for grouping together elements of a rule, why we use certain logical operators here). 

![](Images/pr/image21.png)

**Provide the program rule action**

![](Images/pr/image31.png)

**Test the program rule as before**

**Clear your browser cache by using the browser cache cleaner app**

![](Images/pr/image13.png)

“Select all” -> Clear

![](Images/pr/image33.png)

When the weight value is out of the range you have defined it should display a warning message.

![](Images/pr/image17.png)

![](Images/pr/image40.png)

When the weight is within the range you have defined, or the weight data element has no value, no warning message should appear.

![](Images/pr/image30.png)
![](Images/pr/image6.png)

### STOP - Have the participant’s perform Exercise 3 in the learner’s guide

## Rule 4 - Create a program rule using the TB Treatment Card. 

Show the disease site in the feedback widget

**Access the Programs rules from Maintenance App ⇒ Program**

**Log into the blank instance and go to Maintenance App**

![](Images/pr/image18.png)

**and click on Program**

![](Images/pr/image2.png)

**Add in a new program rule variable**

![](Images/pr/image35.png)

We want to see the disease site regardless of what stage we are viewing in tracker capture. The disease site is only captured in the initial stage, so we want to refer to it to display the necessary information in the widget. This is an example of when we can use a different source field than we have so far.

**Create the new rule**

![](Images/pr/image1.png)

**Create and explain the expression. We will use a function called d2:hasValue to check if there is any value for the data element**

![](Images/pr/image28.png)

**Define the action**

![](Images/pr/image22.png)

For the action, we will display the value that was collected in the feedback widget.

**Test the rule. Clear cache if necessary**

![](Images/pr/image5.png)

### STOP - Have the participant’s perform Exercise 4 in the learner’s guide

## Rule 5 - Create another program rule for the TB Treatment Card to Assign Age based on the date of birth

**Access the Programs rules from Maintenance App ⇒ Program**

**Log into the blank instance and go to Maintenance App**

![](Images/pr/image18.png)

**and click on Program**

![](Images/pr/image2.png)

**Add in a new program rule variable**

**Program rule variable “dateofbirth” with “Tracked entity attribute” source type**

![](Images/pr/image26.png)

**Create the program rule**

**Provide the Program rule details**

![](Images/pr/image29.png)

In the expression, we will use a numerical function. You can point the participants to the documentation for a full listing of custom functions available to the user, as the other will not be covered in detail here. This is rather to give them an idea of what is possible with these functions.

![](Images/pr/image10.png)

**Provide the program rule action**

![](Images/pr/image15.png)

**Test the program rule as before**

**Clear your browser cache by using the browser cache cleaner app**

![](Images/pr/image13.png)

“Select all” -> Clear

![](Images/pr/image33.png)

**Register a new entity and enter the date of Birth**

![](Images/pr/image9.png)

After entering the Date of Birth, Age will be calculated

![](Images/pr/image20.png)

### STOP - Have the participant’s perform Exercise 5 in the learner’s guide
