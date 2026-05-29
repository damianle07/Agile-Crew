# ELEC1005 Assignment 2 - Volunteer Safety Response App

## Project Overview

This repository contains the source files for our ELEC1005 Assignment 2 Power Apps project.

The app is designed for a community safety volunteer organisation. It allows users to report hazards, managers to view the latest submitted incidents, assign volunteers, and volunteers to accept or decline their assigned incidents.

## Main Features

- Report Hazard screen
- SharePoint data storage
- GPS and submitted time capture
- Manager Dashboard protected by access code
- Latest 4 incidents displayed on dashboard
- Incident detail view
- Assign Volunteer workflow
- My Assignments screen for volunteers
- Accept / Decline assignment function
- Directions screen after accepting an assignment
- Help screen explaining how to use the app

## Technology Used

- Microsoft Power Apps
- SharePoint Lists
- Power Fx formulas
- GitHub
- Power Platform CLI

## SharePoint Lists Used

The app uses the following SharePoint lists:

1. List 1: Incidents
2. Volunteers
3. Assignments

## Main Screens

- WelcomeScreen
- ReportHazardScreen
- ConfirmationScreen
- ManagerDashboardScreen
- IncidentDetailScreen
- VolunteerAssignmentScreen
- MyAssignmentsScreen
- IncidentDirectionsScreen
- HelpScreen

## Power App Source Export Note

The team attempted to unpack the Power App using Power Platform CLI:

pac canvas unpack --msapp "Agile Crew.msapp" --sources powerapp-source

However, the CLI returned a System.NullReferenceException. As a workaround, the `.msapp` file was manually extracted into the `powerapp-source` folder. This follows Microsoft’s documented fallback approach that `.msapp` files can be extracted manually to access source files.


## Repository Structure

```text
ELEC1005-agilecrew67-safety-app/
├── README.md
└── powerapp-source/
    └── unpacked Power App source files

