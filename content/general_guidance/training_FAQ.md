- [Introduction](#introduction)
  - [Working with a Training Database](#working-with-a-training-database)
    - [Local Training](#local-training)
    - [Academies](#academies)
    - [Training Database Hosting](#training-database-hosting)

# Introduction

This guide describes some of the practical considerations specific to conducting DHIS2 trainings/academies. This guide targets anyone who is either considering or has conducted a DHIS2 related training. This guidance is based on feedback that has been received throughout conducting academies and trainings over the course of several years and should hopefully support you in providing practical steps for conducting your training.

## Working with a Training Database

Databases are a critical practical consideration when conducting a DHIS2 academy or training. They are the basis in which all materials will be derived from, and if supporting components are not available to meet outlined learning objectives then training outcomes will likely not be as intended. When performing a local training, it is always recommended to use a copy of the local database. When conducting a global or regional academy, several databases are maintained for use in conjunction with the course material in order to meet pre-defined learning objectives.

### Local Training

For a local training, you should use a copy ***of the same database they will be expected to use during the actual implementation***. If you are introducing a new process or procedure, then there may be some significant work that need's to be performed to the database in order to prepare it for the training. Let's take an example of performing a data quality (DQ) training. If you are introducing this as a new process you may want to configure some of the following:

1. DQ Dashboards along with the predictors and indicators that contribute to the dashboards
2. The WHO DQ App as well as indicator and data element groups that will be used to explore the metadata within the DQ app
3. Validation Rules, Groups and Notifications

These are just examples of what you might want to prepare as part of your configuration in relation to this topic. While there are generic databases available to show these concepts, they will be more recognizable for the learner when designing these to work on your own system and can be used as the basis for any training material you create or modify.

### Academies

DHIS2 Level 0 and Level 1 Academies have permanently maintained databases that are associated with each course and can be accessed if needed to conduct an academy. As all of the course material is linked to the various configuration within these databases, minimal configuration or alteration will be required when using one of these databases and pairing them with the standard curriculum for the academy being conducted. This includes the following courses and databases:

| Course              	| Database      	| Description                                                                                                                                               	| Online  Link                                   	| Database Download Link 	|
|---------------------	|---------------	|-----------------------------------------------------------------------------------------------------------------------------------------------------------	|------------------------------------------------	|------------------------	|
| Event Fundamentals  	| Capture       	| Participants perform web and android data entry exercises on this instance.                                                                               	| https://academy.events.dhis2.org/capture       	|                        	|
| Event Fundamentals  	| Analysis      	| Participants perform analysis exercises using event reports, visualizer, maps and joint analysis using aggregate and program indicators on this instance. 	| https://academy.events.dhis2.org/analysis      	|                        	|
| Event Fundamentals  	| Customization 	| Participants create event program metadata on this instance. A private user-role is available to ensure that most metadata is made private by default.    	| https://academy.events.dhis2.org/customization 	|                        	|
| Analytics Tools     	| Analysis      	| Participants create all of their analysis outputs using the core DHIS2 analysis apps (data visualizer, maps, dashboards, data quality) on this instance. It is the only instance required for this academy.	| https://academy.dev.dhis2.org/analytics_tools  	|                        	|
| Tracker Use         	|               	|                                                                                                                                                           	|                                                	|                        	|
| Tracker Config      	|               	|                                                                                                                                                           	|                                                	|                        	|
| Design for Data Use 	|               	|                                                                                                                                                           	|                                                	|                        	|

### Training Database Hosting

When performing training, consider having a separate server/instance/local copy of the database running that your learner's can connect to and utilize during the training. In the first run of a concept, ***do not perform your training directly on a production system*** if it will involve them making some type of modifications that are either not necessary or could result in additional problems later on (ex. entering data, creating or modifying parts of a configuration, saving duplicate charts, maps, tables, etc.). Removing or fixing these can be tricky later on due to the number of dependencies various objects in DHIS2 have with one another and can result in unnecessary modifications to your production configuration.

After the initial training it is always a good idea to have them log in to the system where they will actually be performing their day-to-day work and apply what they have learned during the training. If the training was on data entry, they should enter some real records on the production system if possible with some supervision to ensure they is no misunderstanding of this process. In the case of configuration, you can have them log in to the development instance. You can see the system they will use after the training is dependent on the training content and will have to be adjusted according to local requirements.

