# CAS Reminders and Monitoring (CRM)

An automated, rule-based Make.com workflow designed for IB Diploma Programme CAS Coordinators. This system reads exported ManageBac CAS data, checks it against customizable rules, and sends targeted email reminders to students, CAS advisors, and the CAS Coordinator.

## The Problem
Monitoring CAS across an entire DP cohort is difficult due to scale and visibility. Each student may have 10-30+ individual CAS experiences, and ManageBac does not provide automated alerts for gaps in activity, falling behind on Learning Outcomes, or experiences sitting unapproved for weeks.

## The Solution
CRM is a fully automated, rule-based evaluation and reminder programme (not an AI system) that flags issues early. It requires only about five minutes of manual work per run, significantly reducing the administrative burden on coordinators.

### Core Features: The Seven Checks
The system performs seven independent checks, each of which can be toggled on or off per year level:
* **Unapproved CAS:** Flags experiences submitted by students but not yet approved.
* **Unreviewed CAS:** Flags completed experiences that advisors have not yet reviewed.
* **Missing Supervisor:** Identifies experiences missing a named supervisor.
* **CAS Project:** Checks if the student has a registered CAS Project.
* **Outcomes:** Monitors if achieved Learning Outcomes are on track for the elapsed time.
* **Timeline Gaps:** Flags long periods of inactivity.
* **Reflections:** Checks if the average number of reflections per experience meets a minimum threshold.

### Flexible Email Routing
The system allows for independent routing of warning emails to students, CCs to advisors, and a master digest email to the CAS Coordinator.

## Prerequisites
To use this system, you will need:
1. **Make.com Account:** A free tier is sufficient for testing; a Core plan is recommended for regular use.
2. **Google Workspace / Gmail:** To host the settings/export sheets and send the automated emails.
3. **ManageBac Access:** To export the standard CAS Excel files.

## Installation and Setup
1. Clone or download this repository.
2. Upload the `CAS_Scenario_Settings.xlsx` file to your Google Drive and convert it to a Google Sheet.
3. Create two blank Google Sheets named `CAS_Export_Y11` and `CAS_Export_Y12` in the same folder.
4. Import the `CAS Monitor 2.1.blueprint.json` file into a new Make.com scenario.
5. Follow the detailed setup instructions in the provided PDF documentation.

## Documentation
For full setup instructions, workflow details, and troubleshooting, please refer to the included PDF document in this repository.

## License and Disclaimer
This project is licensed under the MIT License. Please see the `LICENSE` file for full details. 

**Note on Data Privacy:** The user of this software is solely responsible for ensuring that their use complies with all applicable local, national, and international data protection and privacy laws. The creator assumes no liability for any data breaches or mishandling of student information.
