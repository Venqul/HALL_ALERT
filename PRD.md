# Product Requirements Document
# Product name: Hall Alert
## 1. Product Overview

A university hostel maintenance mobile app that lets students log room faults with photos, track repair progress, and see estimated repair times right from their phones. It gives Hall Administrators a central dashboard of all the reported faults, so they can better prioritize urgent issues, assign artisans, search with priority filters and monitor how long each complaint has been opened for. The goal is to replace the old physical logbook approach with a trackable automated process that improves efficiency, speeds up repairs and keeps students informed without repeated trips to the reception.

## 2. Problem Statement

Hostel faults are currently recorded in a physical log book causing two problems for two categories of people:
- **Students** have no idea of when the artisans would come, so they must keep visiting the Hall Porters at the reception for updates
- **Hall Administrators** cannot easily tell which faults have been fixed, which ones are urgent, and how long a complaint has been open for. Every complaint is buried among others in one big book.
As a result, repairs are delayed, urgent issues can go unresolved, resulting in no organized way to track progress

## 3. Business objectives

| ID   | Objective                                                 | Success Metric                                                                                   | Target                                             |
| ---- | --------------------------------------------------------- | ------------------------------------------------------------------------------------------------ | -------------------------------------------------- |
| BO-1 | Replace the physical log book                             | Share of new hostel complaints logged in the app instead of the log book                         | 95% within the first month of the pilot            |
| BO-2 | Let students know when their repair is coming             | Share of complaints that show the student an estimated repair time within 24 hours of submission | 90% of complaints                                  |
| BO-3 | Stop students chasing the Hall Porters for updates        | Number of in-person status enquiries at reception each week                                      | 50% fewer than the baseline recorded before launch |
| BO-4 | Give Hall Administrators a clear view of every open fault | Share of open complaints shown on the admin dashboard with status and submission date            | 100%                                               |
| BO-5 | Get urgent faults handled first                           | Average time to resolve urgent complaints                                                        | Under 24 hours on average                          |
| BO-6 | Resolve faults faster overall                             | Average days from submission to marked resolved                                                  | Under 1 week within one semester                   |
| BO-7 | Reduce repeat faults                                      | Repeat complaints about the same item in the same room within 30 days                            | Under 10% of complaints                            |
| BO-8 | Get students using the app                                | Share of residents in the pilot hostel who submit at least one complaint in the first month      | 50% of residents                                   |
| BO-9 | Get artisans and porters updating the app                 | Share of repairs with a status update from the artisan or porter within two weeks of launch      | 80% of repairs.                                    |

## 4. Target Users

1. **Students (Hostel Residents):** Students are our primary target users, they report room faults, track and receive updates on the repair progress
2. **Hall Administrators:** Hall Administrators are also major target users because they are responsible for managing hostel maintenance complaints, assigning artisans, confirmation and closure of completed repairs, prioritization of complaints.
3. **Maintenance Personnel (Artisans):** These are the people responsible for fixing the problems reported by students. They view assigned jobs and schedule repairs for review by hall porters.
4. **Hall porters:** Serve as on-site support between students and the hall administrators. They view logged complaints, assign artisans, and confirm and close completed repairs.

## 5. Stakeholders

| Stakeholder         | Interest in BU Hall Alert                                                                                                                                  |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Students            | Major beneficiaries. They expect complaints to be attended to on time and want to know when repairs will happen.                                           |
| Hall administrators | Want complaints properly recorded, prioritized, assigned, and resolved.                                                                                    |
| Hostel management   | Want well-maintained hostel facilities and a comfortable environment for students. BU Hall Alert helps them monitor maintenance activity more effectively. |
| Artisans            | Carries out repairs. BU Hall Alert helps them to get an overview of all items they need to fix.                                                            |

## 6. User Stories
### Students
- As a student, I want to report a fault from my phone, so that I don't have to go to the reception to write it down.
- As a student, I want to attach photos of the fault, so that the problem is clear to the hall admins and porters.
- As a student, I want to track the status of my complaint, so that I know when it is being fixed.
- As a student, I want to see the estimated repair time, so that I know when the artisan will come.
- As a student, I want to be notified when my complaint's status changes, so that I don't have to keep checking.
### Hall Admins
- As a hall admin, I want to see which rooms have faults and who reported them, so that I don't have to search through a logbook.
- As a hall admin, I want to be notified of urgent faults, so that I can act on them immediately.
- As a hall admin, I want to assign artisans to complaints, so that every fault has someone responsible for fixing it.
- As a hall admin, I want a record of resolved and unresolved faults in my hall, so that I know what has been fixed and what remains.
### Hall Porters
- As a hall porter, I want to view logged complaints, so that I can answer students' questions without searching a logbook.
- As a hall porter, I want to assign artisans to complaints, so that repairs start quickly.
- As a hall porter, I want to confirm and close completed repairs, so that students can see their complaints are resolved.

## 7. Functional Requirements 

1. **User account and Login:** The app should allow students, porters, artisans and hall admins to create accounts and login successfully 
2. **Report Faults:** Students should be able to report problems in their rooms.
3. **Upload Evidence:** Students should be able to attach pictures of damaged facilities when submitting complaints to show evidence.
4. **Manage Complaints:** Hall admins should be able to view, respond to, and update students complaints and therefore contact artisans for follow up.
5. **Track Complaint Status:** Students should be able to check the progress of their complaints.
6. **Urgency Labelling:** Each complaint should have a priority level (low, medium, urgent) that hall administrators & porters can set and change.
7. **Sort and Filter:** Hall administrators should be able to filter and sort complaints by status, urgency, and date.
8. **Time Open:** The app should show how long each complaint has been open. Non-urgent complaints (low and medium priority) that stay unresolved for more than 7 working days are automatically flagged as overdue.
9. **Assign Artisans:** Hall admins should be able to assign a complaint to an artisan and set an estimated repair time.
10. **Notifications:** Students should be notified when the status of their complaint changes.
11. **Three-Way Closure:** A complaint can only be closed when the artisan, the hall admin, and the student all agree that the fault has been fixed.

## 8. Non Functional Requirements 

1. **Security:** The app should protect students personal information like their course of study, matric number etc.
2. **Usability:** The app should be user-friendly and should be easy to understand for both hall admins and students. A student should be able to submit a complaint in under 1 minute stress-free
3. **Performance:** The app should load quickly(ideally less than 3 seconds).
4. **Reliability:** The app should be available whenever students need to report hostel issues. 
5. **Compatibility:** The app should work properly on current and older versions of Android and IOS.
6. **Latency:** The app should display search and filter results quickly (ideally in less than 5 seconds, even when there are many complaints are stored).

## 9. Scope & Priorities

### Priorities

1. Student, porter, artisan and hall administrator registration and login.
2. Ability to submit complaints.
3. Options to select the type of complaint to be made.
4. Ability to upload pictures and/or videos of reported problems.
5. Direct submission of complaints to the hall administrator.
6. Administrator dashboard for viewing complaints.
7. Complaint status tracking (Pending, In Progress and Resolved).
8. Priority levels for complaints, set and changed by hall administrators and porters.
9. Assigning complaints to artisans, with an estimated repair time that students can see.
10. Three-way closure, where the artisan, hall administrator, and student must all agree before a complaint is resolved.
11. Notifications to students, hall adminisrators, and artisans when a complaint's status changes.
12. Sorting and filtering of complaints by status, priority, and time opened.
13. Automatic overdue flag for non-urgent complaints unresolved for more than 7 working days.

### Out of Scope

1. In-app messaging between students, hall administrators, porters, and artisans.
2. Support for multiple languages.

## 10. Acceptance Criteria

**AC-01: Complaint Submission**
- Students must be able to submit hostel maintenance complaints.
- Students must provide their hostel name, room number and issue description.
- Students must be able to upload pictures of the maintenance fault.
- The system must reject incomplete complaint forms.
- A confirmation message must appear after successful submission.

**AC-02: Complaint Management**
- Hall administrators must be able to view submitted complaints.
- Hall administrators must be able to view relevant maintenance details, including hostel name, room number, issue description, uploaded pictures, complaint status and urgency level.
- Hall administrators must be able to update complaint statuses.
- Hall administrators must be able to set and change complaint urgency levels.
- Complaint urgency levels must include Low, Medium and Urgent.

**AC-03: Complaint Tracking**
- Students must be able to view their submitted complaints.
- Students must be able to track complaint progress.
- Complaint statuses must show Pending, In Progress or Resolved.

**AC-04: Estimated Resolution Time**
- Hall administrators must be able to provide an estimated resolution time.
- Students must be able to view the estimated resolution time.
- Changes to the estimated resolution time must be reflected on the platform.

**AC-05: Complaint Resolution**
- Hall administrators must be able to mark completed complaints as resolved after agreement by both students and artisans.
- Students must be able to view the resolved status.

**AC-06: Usability**
- The platform must provide a clear and easy-to-use interface.
- Students must be able to submit and track complaints without physically visiting the hall administrator’s office.

**AC-07: Anonymous Rating and Feedback**
- Students must be able to submit anonymous ratings after their complaints have been resolved.
- Students must be able to rate how quickly their maintenance issues were resolved.
- Students must be able to rate the overall quality of the maintenance service.
- The identity of students submitting anonymous ratings must not be displayed to hall administrators.

## 11. Assumptions and open questions

### Assumptions

| #   | Assumption                                                                                                                                                                              | Impact if wrong                                                                                             |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| 1   | When something in the hostel breaks (bed, socket, tap, door, toilet), students will report it instead of leaving it.                                                                    | Few reports would come in, so the app would add little value and problems would stay unfixed.               |
| 2   | Every student has a phone with a camera, and the hall admin has a phone too and can check reports without a computer.                                                                   | Students without a suitable phone cannot report, and an admin without a phone would need a web version.     |
| 3   | Students will come downstairs to show the hall admin the problem if he asks after the picture is sent.                                                                                  | Verification would be delayed, so the admin would have to visit rooms himself or rely on the picture alone. |
| 4   | There is stable internet in the hostel, so pictures can be sent and received quickly.                                                                                                   | Uploads would fail or be slow, so we would need offline saving and retry.                                   |
| 5   | One student can report many problems, and one hall admin can receive reports from many students in the same hall. Each report has a short description (what is broken and the room).    | Admins would be overloaded or miss reports, prompting a change in design                                    |
| 6   | Students will pick the correct category (electrical, plumbing, furniture, door and window) and state how urgent the problem is.                                                         | The wrong person gets called (e.g., an electrician for a burst pipe), which wastes time and delays repairs. |
| 7   | Basic reporting with a picture is enough for the first version, with no repairman tracking or payments. The hall admin marks a report as fixed after approval from students & artisans. | Users would expect features we haven't built, and fixed reports could be marked without proper checking.    |

### Open Questions

| #   | Open question                                                                                                                                                             |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Is it one admin per hall or one admin for all halls, and how will we know which admin to send the report to?                                                              |
| 2   | Do students need to register with their student ID or room number before they can report a problem, and how will we verify that they actually stay in that hall?          |
| 3   | Will the student be able to report without a picture, if their camera is bad or the problem cannot be seen in a picture, like a bad smell or no water?                    |
| 4   | After the student sends the report, what happens next, does the hall admin reply in the app, call the student, or just come to check it?                                  |
| 5   | If the hall admin wants to check the problem, does the student have to come downstairs to meet him, or will the hall admin go to the room directly?                       |
| 7   | Can a student edit or delete a report after they have sent it, if they sent the wrong picture or the wrong room?                                                          |
| 8   | Can students from different halls see each other's reports, or is each hall kept separate so only that hall admin sees reports from his own hall?                         |
| 9   | What happens if many students report the same broken thing, like one toilet for the whole floor, will it show as one report or many separate reports?                     |
| 10  | Will there be any time limit for how fast the hall admin should respond, and what happens if he does not respond?                                                         |
| 11  | How will the category and impact work, will the student pick the category and the impact level by themselves, or will the hall officer change it after he has checked it? |
