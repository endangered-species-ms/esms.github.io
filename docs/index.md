---
title: Overview
description: An application used to manage endangered species investigation data
menu: Overview
order: 10
---

## Summary

_ESMS_ is a content management system designed to be used as an Android application for ease of
 use in the field, while traveling as well as in the office. A user, depending upon access rights, can 
 find and/or add/modify data regarding a given species of life. Personnel collect and organize data all 
 with the purpose of providing managers, administrators and legislators with the information needed 
 to determine the endangerment status of a species.

## Intended users &amp; user stories

* A field biologist.

    > As a field biologist specializing in studying the habitat, numbers etc. of endangered living organisms, the ease of 
using an app-based content management system to record and organize data would greatly improve the quantity and quality of
work I could accomplish.        
                        
* Department Head.

    > As a head of government department responsible for collecting, analyzing, and presenting data framed to make the case
that a given species should have a lawfully valid endangered designation, I need a easy to access and easy to use system
for managing both data collected and managing the personnel involved.

## ESMS details

- A user should have a secured account to access the application. 

	- The following are the types of accounts. 
		- VIEWER: The user can query the species data database to retrieve information. 
		- RESEARCHER: The user that can submit data, retrieve it for analysis and categorization, or return it to the 
		species data locker. 
		- ADMIN: An account with special privileges that can manage other users’ activities on the data system.

	- A researcher can have different access rights:
		- APPRENTICE: no access to the data system.
		- JUNIOR RESEARCHER: Read access to the data system.
		- RESEARCHER: Write access to the data system
		- PROJECT HEAD: Write access to the data system and read access to personnel system.
		- DEPARTMENT HEAD: Write access to the data system and write access to personnel system.

	- Species endangerment can be classified based on their severity as follows.
		- LEAST CONCERN: A species that has widespread and abundant population.
		- NEAR THREATENED: Likely to qualify for threatened category in the near future.
		- VULNERABLE:
		- ENDANGERED:
		- CRITICALLY ENDANGERED:
		- EXTINCT IN THE WILD:
		- EXTINCT:

	- Investigations can be classified by the research status as follows.
		- SUBMITTED: recently introduced into the system.
		- ACTIVE_RESEARCH: Data is being collected; the investigation/research is in some stage of process.
		- UNDER_REVIEW: All data has been submitted, conclusions have been drawn, administrators/legal experts are doing 
		what they do.
		- CLOSED: All data and specimens have been archived because status has been determined.

## Client component

* **Functionality**

    * The client app allows the user, depending on access rights, to enter data, access data already in the system, log and 
access physical data locations, look up and even add personnel.

    * If a user is in the field, data can be stored in the local Room database until a convenient place for uploading
data can be made available.

* **Data persistence**

    * Enter something here

* *Device or external services used*

    * Google Sign In
    
## Server component

* **Functionality**

    The server component is the heart of the content management system: coordinating, categorizing, and updating persisted 
    data and personnel:
    
    * Transition a person to researcher status.
    
    * Setting information about a researcher such as name, id number, access rights, job assignment, etc.
    
    * Setting information about individual species under investigation, such as scientific name, common name, habit, current 
    endangerment status, etc.
    
    * Set up and access storage places containing collections of physical data.

    * Criteria check off to determine the stage of an investigation.
    
* **Data persistence**

    * User registry w/ user profiles &amp; preferences.

* **Device or external services used**

    * Google OAuth 2.0 provider
