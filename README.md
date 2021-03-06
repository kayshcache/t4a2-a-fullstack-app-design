# T3A2-A Full Stack Application (Part A)
### Links
1. [See Repository for Part B](https://github.com/kayshcache/t4a2-b-fullstack-app)
2. [See Assignment specifications]()
## Assignment Requirements R1 - R6
## R1. Description
... | ...
--- | ---
Name (Acronym) | SATM
Full name | Security Awareness Training Manager
Category | Training Management Software
Sector / Tier | Corporate, Medium to large business
Industry | IT, Banking, Governance, Education
Purpose | Provide managers of staff a convenient way to schedule, deliver and manage training content for employees to meet security awareness compliancy
### Purpose of Application
This application is a training management platform for medium to large businesses and corporations operating under Australian legal requirements to meet minimum accreditation of risks and procedures relating to information security in the workplace. It delivers a number of content types to employee-trainees as well as track individual employee completion of required training material.
### Functionality & Features
1. Manage employees in the system as trainees (will refer to employees as trainees from here onward)
2. Allow registered trainees to access training materials
3. Curate training materials for delivery. Curated materials are organized into units ( will be referred to as Training Units [TU] from here). TUs contain a description and title as well as up to 10 content types linked. Trainers, Managers, or content experts will submit TUs using a form. They can also delete or update the TUs in the system.
4. Track employee completion of materials: when an employee accesses a TU, that is recorded. The next thing to be recorded is once the trainee has viewed all the materials in that TU they must confirm to have done so and understood the material in the TU - this is then also recorded and will display in the report. Each trainee must do that all TUs on their schedule.
5. Display an overview report of training unit completion for managers and trainers to review the progress of the trainees in the system.
### Target Audience
Medium to large businesses with a primarily white collar workforce and corporations in need of "Security Awareness Training" (SAT)
User need: track the delivery of training material to staff of Cyber Security and Social Engineering Attack Awareness.
How to meet that need: provide a simple platform to curate material into units and schedules. A schedule is like a course and contains units. Provide basic user management for trainees to login and complete their required schedule. Track the completion and progress of trainee activity on the platform.
Known issues with Training Management Software (TMS): 
1. Employee buy in; employees may not view the content as being relevant or important to the daily operations. SOLUTION: make the user experience as simple and painless as possible.
2. Managers are very busy and don't have time to learn most websites. The management/admin panel will be very limited options but diplay only the most important information for them. Reports will display trainee completion and progress figures.
#### Marketing Strategy
Marketing should appeal to middle and upper managers as well as CEOs looking for single solution to SAT management.
### Technology Stack Description
2 Servers: React Frontend and Node/Express API
Primary datastore: Mongo
Backend for managing users and content
Frontend for delivering content to users and trainee administration
TMS example of commercial product https://www.arlo.co/training-management-system
Mongo, Express, React, Node
## R2. Dataflow Diagram
![dataflow](/docs/flow-diagram.png)
## R3. Application Architecture Diagram
![security awareness training management application architecture stack diagram](/docs/satm-app-architecture-diagram.png)
## R4. User Stories
### Initial User Stories
No. | User Story | Associated Feature
--- | --- | ---
1 | Employees want to track their progress to fulfill their requirement to complete the training. They want a simple user experience. | Trainee view shows progress in a list. Star indicated completed units, dot indicates current
2 | Managers want to see the progress overview report of all the employees they need to tick off the list. They have to verify to their leadership that the company's employees have had the required SAT. | User management view where they can go through and see progress reports for each employee.
3 | Trainer might also be the manager or even an outside contractor wants to put the content in the system and make it available for the company's employees to access. | Content curation page for uploading SCORM, PDF, text or other content for each unit in the training program.
4 | CEO wants to see the report that shows the progress of the employees to complete the training so they can estimate schedule for other coming company priorities. They are busy and want a simple report. | A csv file showing employee name and progress statistics in simple format, middle managers can also use it to prepare more readable reports for upper management.
5 | Managers want to export simple data from the progress of the employees to view the content so they can prepare their report to the leadership. | Export button exports all data from the progress report screen to CSV
6 | Managers want to know which employees are not completing the course in time so they can contact that individual and discuss with them | Overview shows stats and shortlist of employees who have not progressed as far as others.

## R5. Wireframes
![wf1.1 login](/docs/wf1-1-login.png)
![wf1.2 trainee view](/docs/wf1-2.png)
![wf2 mobile](/docs/wf2.png)
![wf3 management](/docs/wf3.png)
![wf4 content curation](/docs/wf4.png)
## R6. Project Management (Screenshots)
![agile project management view 1](/docs/agile-1.png)
![agile project management view 2](/docs/agile-2.png)
![agile project management view 3](/docs/agile-3.png)
## Marking Criteria
1. CMP1043-4.2 Dataflow Diagram: Provides dataflow diagram(s) that strictly follow the standard convensions to clearly identify the processes within your application. Clearly depicts where data is coming from, where it is going and how it is being stored.
2. CMP1043-4.3 Application Architecture Diagram: Shows almost flawless understanding of the high level structure of the app
3. CMP1043-5.1 Provide UX/UI design documentation(user stories) that adequately show Agile methodology implementation: Provides multiple user stories that use ‘persona, what and why’ that outline meaningful features of the project. Shows evidence of user story revision and refinement.
4. CMP1043-4.1 Utilise an industry standard program for creation of wireframes & CMP1043-5.3 Provide UX/UI design documentation(wireframes) that adequately show Agile methodology implementation: Provides wireframes that show exceptional planning of project flow and structure including but not limited to space distribution, content prioritisation, intended actions, functions, relationships between screens.
5. CMP1043-5.2 Select and follow a commonly used planning methodology, such as Kanban, Trello, Jira, or Asana: Simple and clear standards for planning methodology chosen and adhered to
