
# Sharing - Session Summary

![](Images/sharingsessionsummary/image1.png)

* User roles can be thought of as the top layer restriction on what users can do in the system
* Sharing can be thought of as the second layer which more precisely restricts a user roles functions to specific objects in the system

![](Images/sharingsessionsummary/image2.png)

The sharing model has two levels, metadata and data sharing. Metadata sharing is focused on various elements of the configuration, while data sharing deals with how a person can interact with already existing, or, potentially add new data

In a tracker program, we can share the meta-data of following objects

* Data Elements
* Tracked Entity Attributes
* Option Sets
* Tracked Entity Types
* Programs
* Program Stages
* Program Indicators

In a tracker program, we can share the data of the following objects:



* Tracked entity types
* Programs
* Program Stages

The data level sharing can be described as follows

Tracked entity type

| Can view data                                                                                                                              	| Can capture data                                                                                                                                                                                                                                                             	|
|--------------------------------------------------------------------------------------------------------------------------------------------	|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| <br>Search for tracked entities with this tracked entity type<br><br>See tracked entity type attribute values for this tracked entity type 	| <br>Edit visible tracked entity attributes for tracked entity instances of this type<br><br>Register/create new tracked entity instances of this type<br><br>Delete tracked entity instances of this type<br><br>Deactivate/reactivate tracked entity instances of this type 	|

Tracker Program


| Can view data                                                                                                                                                                                       	| Can capture data                                                                                                                                                                                                                                                                                           	|
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| <br>Search for tracked entities within this program<br><br>See tracked entity attributes specific to this program<br><br>See enrollment details for the program<br><br>See notes for the enrollment 	| <br>Enroll entities into the program<br><br>Edit enrollment details for the program<br><br>Complete/reopen enrollments into the program<br><br>Add notes for the program<br><br>Edit relationships for the program<br><br>Send message to tracked entity instance<br><br>Delete enrollments in the program 	|


Program Stage
| Can view data                                                                                             	| Can capture data                                                                                                                                                                                                                                                                            	|
|-----------------------------------------------------------------------------------------------------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| <br>See the program stage and its events and data within an enrollment<br><br>See the program stage notes 	| <br>Add/schedule/refer a new event within the program stage<br><br>Complete/reopen the events within the program stage<br><br>Edit tracked entity data values within events in the program stage<br><br>Add notes for events in the program stage<br><br>Delete events in the program stage 	|

