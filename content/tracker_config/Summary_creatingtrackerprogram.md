# Creating a multiple stage tracker program - Summary session

## Step-by-Step Guide for Creating a Multiple-Stage Tracker Program

### Step 1: Identify and Create the Tracked Entity

* Objective: Ensure a tracked entity type "Person" exists.
* Navigation: Go to the Tracked Entity section from the maintenance app.
* Action: Confirm that you are tracking a "Person." No new entity types are needed.
S
### Step 2: Identify and Create Relationship Types

* Objective: Define relationships to link entities.
* Navigation: Go to the Relationship Type section from the apps menu.
    * 
    Example: Utilize existing relationship types (e.g., Mother-Child) for linking entities in the TB program.

### Step 3: Identify and Create Option Sets

* Objective: Review attributes and data elements needing option sets.
    * Attributes: Sex (Male/Female).
    * Data Elements:
        1. TB Patient Type
        2. Disease Site
        3. Extra Pulmonary TB Site
        4. Type of Treatment
        5. Sputum Smear Result
        6. Culture Result
        7. GeneXpert Result
* Navigation: Go to the Option Set page and check existing option sets.
* Action: Add new option sets as needed and populate them with options.

### Step 4: Identify and Create Entity Attributes

* Objective: Define the attributes for registering the entity in the program.
    * Attributes to Create:
        1. Registration Number
        2. First Name
        3. Last Name
        4. Age (in years)
        5. Date of Birth
        6. Sex (Male/Female)
        7. Address
        8. Phone Number
* Navigation: Go to the Tracked Entity Attribute section.
* Action: Create 1-2 new attributes and explain the configuration process.

### Step 5: Create Data Elements with Domain Type "Tracker"

* Objective: Create data elements for the program.
     * Data Elements to Create:
        1. TB Patient Type
        2. TB Disease Site
        3. EPTB Site
        4. Type of Treatment
        5. Sputum Smear Result
        6. Culture Result
        7. GeneXpert Result
        8. Treatment Outcome
        9. Weight (kg)
* Navigation: Go to the Data Element section.
* Action: Create necessary data elements, ensuring to assign prefixes for organization.

### Step 6: Create Data Element Groups

* Objective: Organize data elements into groups for better management.
* Navigation: Access the Data Element Group section.
* Action: Create a data element group, assigning all relevant data elements to it, and save.