# Trainer’s Guide to the Category Model

## What is this guide?

This guide is a support document for DHIS2 Academy trainers for the session "The correct way to work with the category model." This session follows the standard Academy training approach with 

1. a live demo session where the trainer demonstrate and explain the features, and 
   
2. a hands-­on session with exercises where participants get to practice the same features.

This guide will help the trainer​ prepare​​ for the live demo session. The “Live Demo step by step” section has a detailed walkthrough of all the steps to demonstrate with explanations and screenshots that should be easy to follow. Use that when preparing for the live demo session.

There is also a Quick Guide which lists the steps very briefly and this is meant as a lookup guide or “cheatsheet” WHILE doing the demo, to help the trainer remember all the steps and the flow of the demo.

## Learning objectives for this session

1. Define the DHIS2 category model
2. Use categories to disaggregate data in analysis apps
3. Create category options, categories and category combinations following a standard operating procedure
4. Describe the relationship between categories, data dimensions and anlaytics
5. Apply category combinations to data elements

## Time Requirements

- Live Demo: 30 min
- Hands-on Exercises: 30 min
- Assignment: 30 min

## Background

## Preparations

## Best Practices

## Quick Guide

1. Review the presentation the Category Model

[Link](https://docs.google.com/presentation/d/1243f0aSQATHFFUzZNBNIiH4Hltaor181/edit?usp=share_link&ouid=104677221247573000314&rtpof=true&sd=true)

2. Show how categories can be used to visualize data
   1. Open the chart HIV - HIV cascade by sex - last 12 months from the HIV national dashboard and discuss
   2. Add the Age (HIV) disaggregation to the chart
3. Create a new chart
   1. Data: 
      1. Data Type : Data Elements 
      2. Data Element group: HIV
      3. Data Element names: HIV - HIV tests positive, HIV - PLHIV new on ART, HIV - PLHIV retained on ART last 12 months
   2. Period: last 12 months
   3. Org unit: Lao

STOP - Exercise 1

1. Review the presentation "The correct way to create categories"

[Link](https://docs.google.com/presentation/d/1243f0aSQATHFFUzZNBNIiH4Hltaor181/edit?usp=share_link&ouid=104677221247573000314&rtpof=true&sd=true) 

2. Show how to manage category options in maintenance
   1. Create cat options using your initials for
      1. Sex (male, female) 
      2. Age (0-14, 15+)

STOP - Perform Exercise 2

3. Show how to manage categories in maintenance
   1. Create 2 cateogries
      1. Sex (male, female) 
      2. Age (0-14, 15+)

STOP - Perform Exercise 3

4. Show how to manage category combinations in maintenance 
   1. Age (0-14, 15+) + Sex

STOP - Perform Exercise 4

4. Review the presentation on additional considerations for categories

[Link](https://docs.google.com/presentation/d/1j4zONbJx73HwgiFFu8eGgjVUJOG8mJZf80V6IpS_lLE/edit?usp=sharing)

## Live Demo step by step

### Review the presentation the Category Model

[Link](https://docs.google.com/presentation/d/1243f0aSQATHFFUzZNBNIiH4Hltaor181/edit?usp=share_link&ouid=104677221247573000314&rtpof=true&sd=true) 

### Show how categories can be used to visualize data

Open the chart "HIV - HIV cascade by sex - last 12 months" from the HIV national dashboard.

![HIV-cascade](images/categories/chart1-dashboard.png)

![hiv-cascade-viz](images/categories/chart1-in-viz.png)

This chart has one category with three category options being used to disaggregate several data elements (Sex) located in the series of the chart. In analysis, we can apply as many combination of data dimensions as required to create our intended input and organisation unit groups/group sets can help with this. 

They can also support the disaggregation of our data. 

Add the disaggregation "Age (HIV)" to the to the category of the chart and update the chart. 

![chart1-in-viz-with-age](images/categories/chart1-in-viz-with-age.png)

We can see we can add more then one category to disaggregate our data, as long as the data itself is disaggregated and collected this way.

#### Create a new chart

To create a new chart select File - > New

Here are the inputs for the chart:

**Chart Type**
- Column

**Data**
- Data Type : Data Elements 
- Data Element group: HIV
- Data Element names: HIV - HIV tests positive, HIV - PLHIV new on ART, HIV - PLHIV retained on ART last 12 months

![chart1_data](images/categories/chart1-data.png)

**Period**
- Last 12 months

**Organisation unit**
- Lao

We now want to add in our categories for our data. In this case, we need to know how the data elements we selected are disaggregated. 

If your are not completely familiar with this, one way to perform a quick check is to review the form in data entry or in the reports app if you have access to. 

![hiv-data-entry](images/categories/hiv-data-entry.png)

Here we can see the data elements that we are working with are disaggregated by age and sex; we can therefore also use these to disaggregate our data in visualizer.

Add in the categories for Age (HIV)

![age-cat-selection](images/categories/age-cat-selection.png)

and sex

![sex-cat-selection](images/categories/sex-cat-selection.png)

Modify the layout and update the chart

![chart2-with-categories.png](images/categories/chart2-with-categories.png)

You will see the disaggregations (categories) have now been applied.

#### STOP - Perform Exercise 1

### Review the presentation "The correct way to create categories"

[Link](https://docs.google.com/presentation/d/1xRmqvfrJry6f1fcKCwp6Qd9Ojiw9FQ7LS0oBPGhOyNU/edit?usp=sharing)

### Show how to manage category options in maintenance

In our example, let us create the category options that we had used to disaggregate our HIV data. In this example, we had:

- Sex (male, female)
- Age (0-14, 15+)

Let us just start with these examples. 

Navigate to maintenance -> Category -> Category Option

From this screen, the first thing you want to do is search for the category option you are creating. 

![cat_option_search_maintenance](images/categories/cat_option_search_maintenance.png)

If you type in "Male" as a category option, you will see that this already exists. Under normal circumstances, you would stop here. Never create a duplicate category option when it already exists. 

In this scenario, we want to go through the process of the category model from start to finish; so we will create this category option for demonstration purposes only.

Create a new category option by selecting the plus icon.

Use your initals as a prefix and create the category option Male

![cat-option-male](images/categories/cat-option-male.png)

You can discuss the fields as you fill them in. Save the category option when you are finished.

Repeat this process to create the category options for female, 0-15 and 15+. 

#### STOP - Perform Exercise 2

### Show how to manage categories in maintenance

We want to create two categories:

- Sex (male, female)
- Age (0-14, 15+)

Navigate to maintenance -> Category -> Category

From this screen, the first thing you want to do is search for the category you are creating.

![cat_option_search_sex_maintenance](images/categories/cat_option_search_sex_maintenance.png)

We will see there are a couple of category by name sexes listed already. Under normal circumstances, you would stop here. Never create a duplicate categories when they already exist. 

In this scenario, we want to go through the process of the category model from start to finish; so we will create these categories for demonstration purposes only.

Create a new category by selecting the plus icon.

Use your initals as a prefix and create the category for sex, Make sure you use the category options that you have created (intials_male, initials_female) 

![category-sex](images/categories/category-sex.png)

You can discuss the fields as you fill them in. In particular, make sure to review the data dimension type. Leave it as disaggregation but we will come back to attributes in a later session.

Also, explain that the data dimension tick box allows the category to show up on the left side menu in analysis apps. 

![viz-dimensions](images/categories/viz-dimensions.png)

Repeat this process to create the category for Age (0-14/15+). Ensure you use the category options that you made with your initials to create this new category.

#### STOP - Perform Exercise 3

### Show how to manage category combinations in maintenance

We want to create one category combination

- Age (0-14, 15+) + Sex

Navigate to maintenance -> Category -> Category combination

From this screen, the first thing you want to do is search for the category you are creating.

If we were to investigate a bit, we would see Age and sex (HIV) category combination is actually the same as what we are about to create. This is becase the category Age (HIV) actually contains the same age groups we have made.

![age-hiv-cat](images/categories/age-hiv-cat.png)

It is important to consider that sometimes the duplicate item you are looking for might not be readily apparent based on its name alone. Keep this is mind when searching for duplicates in your own system and only create items when you are absolutely sure they are not located anywhere else.

In this scenario, we want to go through the process of the category model from start to finish; so we will create this category combination for demonstration purposes only.

Create a new category combination by selecting the plus icon.

Use your initals as a prefix and create the category combination for for Age (0-14, 15+) + Sex. Make sure you use the categories that you have created (intials_sex, initials_age (0-14/15+)) 

![catcombo-age-sex](images/categories/catcombo-age-sex.png)

You can discuss the fields as you fill them in. In particular, make sure to review the data dimension type. Leave it as disaggregation but we will come back to attributes in a later session.

#### STOP - Perform Exercise 4

### Review the presentation on additional considerations for categories

[Link](https://docs.google.com/presentation/d/1j4zONbJx73HwgiFFu8eGgjVUJOG8mJZf80V6IpS_lLE/edit?usp=sharing)

