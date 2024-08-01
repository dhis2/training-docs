# Trainer's Guide to Setting up the Android Database and Instances for use in the Android Academy

The Android academy requires some considerations to make when deciding what is needed regarding the infrastructure for the academy. The sessions and exercises are complicated by the fact that 

1. Some sessions require you to make instance-wide changes (anything to do with the Android Settings Web App and APK distribution web app)
2. The participants themselves need copies of their own metadata (programs, datasets, related metadata) and users that have access to these program and datasets in orer to make various configuration changes and view their effect on the android device

In order to mitigate some of the challenges associated with these tasks, the team conducting this academy needs to:

1. Consider how many instances you will have based on the number of participants attending
2. Have them work in groups for parts of the academy
3. Use a specialized cloning metadata tool in order to create the duplicated metadata within the instances you have deployed

A listing of each session, along with special considerations that are needed for each, is listed in the table below.

| Session                                     | Considerations                                                                                                                                                                                                                                                                                                                                                       |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| DHIS2 Android App                           | This is meant as a demo for you to show them features. There are no exercises for the participant in this session.                                                                                                                                                                                                                                                   |
| Aggregated Data                             | The participants can use the demo account to follow along with this session. Username: android Password: Android123!                                                                                                                                                                                                                                                 |
| Individual Data                             | The participants can use the demo account to follow along with this session. Username: android Password: Android123!                                                                                                                                                                                                                                                 |
| Maps - Geospatial considerations            | The participants will have to switch between using the demo account and accessing an account that can edit data in maintenance. The trainer/learner’s guide prompts when different accounts are needed.                                                                                                                                                              |
| DHIS2 Relationships & Android               | The participants can use the demo account for parts Exercise 1 and Exercise 2. For Exercise 3, they will have to use THEIR copy of the program metadata. They will need access to an account that can edit program metadata.                                                                                                                                         |
| Program Rules Demo                          | They will have to use THEIR copy of the program metadata. They will need access to an account that can edit program metadata, as well as an android account with access to their program. They are prompted several times in the learner’s guide.                                                                                                                    |
| Visual Configurations                       | They will have to use THEIR copy of the program AND dataset metadata.  They will have to use 2 separate accounts to review the program and dataset respectively. They will need access to an account that can edit program metadata, as well as an android account with access to their program and dataset. They are prompted several times in the learner’s guide. |
| Visual Data Entry                           | They will have to use THEIR copy of the program AND dataset metadata.  They will have to use 2 separate accounts to review the program and dataset respectively. They will need access to an account that can edit program metadata, as well as an android account with access to their program and dataset. They are prompted several times in the learner’s guide. |
| Android Settings Webapp Part 1              | The Android settings web app makes instance wide changes to the system. They will need to be placed in groups, with each group modifying the app on their own instance together. They will need an administrator account with the “ALL” authority in order to make changes in this app.                                                                              |
| Program Indicators in Android               | They will have to use THEIR copy of the program metadata. They will need access to an account that can edit program metadata, as well as an android account with access to their program. They are prompted several times in the learner’s guide.                                                                                                                    |
| Offline Analytics- How to configure and use | In Exercise 1, they will use the shared demo account.                                                                                                                                                                                                                                                                                                                |
| Going Mobile (Global Fund Extended) - 60    | This is just a presentation.                                                                                                                                                                                                                                                                                                                                         |
| Android APK Distribution Web App            | The APK distribution web app makes instance wide changes to the system. They will need to be placed in groups, with each group using the app on their own instance together. They will need an administrator account with the “ALL” authority in order to use this app.                                                                                              |
| Android Release Cycles and Roadmap          | This is just a presentation.                                                                                                                                                                                                                                                                                                                                         |
| Community: Contribute and engage            | This is just a presentation.                                                                                                                                                                                                                                                                                                                                         |
| Troubleshooting the android app             | Presentation and demo.|                            


## Setting up the instances




## Cloning the accounts



## Instructing on which accounts to use