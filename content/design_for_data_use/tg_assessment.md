# Trainer’s Guide to Assessments - Part 1

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session "Asessments" This session follows the standard Academy training approach with 

1. a live demo session where the trainer demonstrate and explain the features, and 
   
2. a hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## Learning objectives for this session

1. Describe the concept of metadata assessment
2. Demonstrate the use of the metadata assessment tool 
3. Explain the outputs of the metadata assessment tool
4. Describe manual checks that can supplement the tools findings

## Time Requirements

- Live Demo: 
- Hands-on Exercises: 
- Assignment: 

## Background



## Preparations



## Best Practices



## Quick Guide

1. Support all participants to ensure all the necessary tools are installed on their computer
2. Quickly show and discuss the outputs of the report
3. Review how to run the report'
   1. Discuss the inputs of the .Rprofile file
   2. Knit the report and show the output

4. Review the output of the report along with the participants
5. If time allows, select participants to share the outcomes of their report with the group

#### STOP - Perform Exercise 1

4. Review the recap slide

## Live Demo step by step

### Support all participants to ensure all the necessary tools are installed on their computer

### Quickly discuss the outputs of the report

### Review how to run the report

#### Discuss the inputs of the .Rprofile file

include_slow hits the data value table (for example, abandoned data elements = DEs with no data attached to them). This can be a very lengthy operation depending on the amount of data in the system. Will also depend on the power of the server. Underpowered server + lots of data means it will be very slow. May want to exclude, can take 5-10 mins PER check, increasingly the time significantly

#### Knit the report and show the output



#### STOP - Perform Exercise 1

### Review the output of the report along with the participants

If errors, copy the ID of the unexecuted view, go into the instance, can either use API or go into the SQL view section of maintenance. paste in the UID of report that failed at the end of this URL. This will take you to the SQL view that did not run and may help you explain why it didn't run. 

### If time allows, select participants to share the outcomes of their report with the group