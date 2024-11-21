# Program Access - Session Summary


## Part 1: Register an Individual in the TB Treatment Card Program

* Log in as a user with access to register a tracked entity in the organization unit.
* Select Parrot District Hospital and register an individual in the TB Treatment Card program.
* Fill in initial data for the first stage of the program.

## Part 2: Search for TEI Using "Break Glass" Access

* Log out and log back in using the credentials:
    Username: breakglass
    Password: District1#
* Clear the cache and navigate to Tracker Capture.
* Search for the previously registered record by selecting the appropriate organization unit and program.
* Enter a reason for accessing records outside the assigned data capture unit if prompted.
* Access the individual's tracker dashboard and enter new stage data, noting the limitations on editing data from outside organization units.

## Part 3: Review Records for Immunization and ANC

* Log in with access to all org units.
* Select Cardinal Hospital and the Immunization program to find Jayden Thomas (Open access).
* For ANC (closed access), search for Sheila Smith. Attempting to open this record will result in an access denial message.

## Part 4: Review Open Access

* Log in again as breakglass.
* Navigate to Tracker Capture and access Jayden Thomas's record without needing to enter a reason.

## Part 5: Review Closed Access

* Search for Sheila Smith in the ANC program. Attempting to open this record will show that access is denied.

## Part 6: Configure Access Levels

* Log in as an admin user.
* Navigate to the TB Treatment Card Program in Maintenance to review and discuss the access level settings.
* Review the “breakglass” user to understand their organizational unit assignments and how they relate to access levels.

## Summary of Access Levels

* Closed: Cannot open TEI outside data capture scope.
* Protected: Can open TEI outside scope with a reason; access expires after 3 hours.
* Audited: Can open TEI with log entries made.
* Open: Can open TEI without additional requirements.