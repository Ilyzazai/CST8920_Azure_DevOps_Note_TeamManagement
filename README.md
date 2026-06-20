# CST8920 Assignment 2: Azure DevOps Board

**Project Name:** Smart Campus IT Service Portal  
**Course:** CST8920 - Highly Effective Teams  
**Student:** Ilyas Zazai  
**Tool Used:** Azure DevOps Boards  
**Assignment Focus:** Project planning, team workflow, swimlanes, columns, tickets, priority, effort, and business value  

---

## 1. Purpose of This Assignment

This assignment was not about coding an application. The main purpose was to understand how an IT team plans, organizes, and tracks project work using a board tool like Azure DevOps.

In real IT teams, developers, DevOps engineers, testers, business analysts, and project managers do not usually start working randomly. First, they need to understand:

- What system is being built
- What features are required
- What work should be done first
- How difficult each task is
- Which stage each task is currently in
- What is already completed and what is still pending

For this assignment, I used Azure DevOps Boards to create a project board with columns, swimlanes, and tickets. This helped me understand how a larger IT use case can be broken down into smaller work items.

---

## 2. Tool Used: Azure DevOps Boards

Azure DevOps is a Microsoft platform used by software and IT teams for planning, coding, building, testing, and deploying applications.

For this assignment, I only used **Azure Boards**.

Azure Boards is used for:

- Creating project boards
- Creating tickets or work items
- Tracking work progress
- Organizing tasks by feature area
- Estimating effort
- Assigning priority
- Supporting team communication

I did not create cloud resources such as virtual machines, storage accounts, databases, or AKS clusters. This project was only for planning and work tracking.

---

## 3. Difference Between Azure Portal and Azure DevOps

At first, it was confusing because Azure Portal and Azure DevOps both use the Microsoft account. However, they are different tools.

| Tool | Purpose |
|---|---|
| Azure Portal | Used to create and manage cloud resources such as VMs, storage, databases, App Services, and AKS |
| Azure DevOps | Used to plan software work, create boards, manage tickets, repositories, pipelines, and team workflows |

For this assignment, the correct tool was **Azure DevOps**, not the normal Azure Portal.

The correct website was:

```text
https://dev.azure.com
```

---

## 4. Project Use Case

The project use case I selected was:

## Smart Campus IT Service Portal

The Smart Campus IT Service Portal is a proposed web-based system that can help students and staff submit and track IT support requests in one place.

The system would allow users to:

- Log in using their college account
- Submit IT support requests
- Track the status of submitted requests
- Receive notifications when status changes
- Allow IT administrators to review requests
- Allow IT administrators to check audit logs and recent activity

This use case was selected because it is realistic for a college environment and provides enough feature areas to create proper swimlanes and detailed tickets.

---

## 5. Azure DevOps Project Setup

The project was created in Azure DevOps using these details:

| Item | Value |
|---|---|
| Organization | `ilyas-cst8920` |
| Project Name | `Smart Campus IT Service Portal` |
| Visibility | Private |
| Board Type | Issues board |
| Main Tool Used | Azure Boards |

Even though the board showed **Issues**, I used each issue as a project ticket/work item. This still matched the assignment because the requirement was to create tickets with details, fields, priority, and effort.

---

## 6. Board Concept

The Azure DevOps board was used like a project planning board.

Simple example:

| Real Life Example | Azure DevOps Example |
|---|---|
| Whole house | Whole project |
| Rooms/kitchen/bathroom | Swimlanes or feature areas |
| Small construction tasks | Tickets |
| Work progress | Columns |

In my project:

| Concept | Example |
|---|---|
| Whole project | Smart Campus IT Service Portal |
| Swimlanes | Login, Database, Audit Logs |
| Tickets | Login page, database storage, email notification |
| Columns | Backlog, Analysis, Development, Testing, Security Review, Deployment, Done |

---

## 7. Columns Used in the Board

Columns show the stage of work. I customized the board columns to follow an IT/DevOps lifecycle.

The columns used were:

1. Backlog
2. Analysis / Design
3. Development
4. Testing / QA
5. Security Review
6. Deployment
7. Done

### Meaning of Each Column

| Column | Meaning |
|---|---|
| Backlog | Work is planned but not started yet |
| Analysis / Design | Requirements and design are being reviewed |
| Development | The feature is being built |
| Testing / QA | The feature is being tested |
| Security Review | Security, access, and privacy are being checked |
| Deployment | The feature is ready to release |
| Done | The work is completed |

The final workflow was:

```text
Backlog → Analysis / Design → Development → Testing / QA → Security Review → Deployment → Done
```

This shows how a ticket moves from planning to completion.

---

## 8. Swimlanes Used in the Board

Swimlanes are horizontal sections of the board. They group tickets by feature area.

The assignment asked for 3 swimlanes related to feature requests. I created these 3 swimlanes:

1. Login and Access Management
2. Service Request Database
3. Audit Logs and Notifications

### Meaning of Each Swimlane

| Swimlane | Purpose |
|---|---|
| Login and Access Management | Handles user login, roles, logout, and session security |
| Service Request Database | Handles request form, database storage, and request status tracking |
| Audit Logs and Notifications | Handles audit logs, email notifications, and admin monitoring |

These swimlanes represent the main parts of the Smart Campus IT Service Portal.

---

## 9. Tickets Created

The assignment required 3 tickets in each swimlane.

Total tickets created:

```text
3 swimlanes × 3 tickets = 9 tickets
```

---

## 10. Ticket List by Swimlane

### Swimlane 1: Login and Access Management

| Ticket | Priority | Effort | Business Value |
|---|---:|---:|---:|
| Implement college email login page | 1 | 5 | 100 |
| Add role-based access for students and IT admins | 1 | 8 | 95 |
| Add secure logout and session timeout | 2 | 3 | 80 |

### Swimlane 2: Service Request Database

| Ticket | Priority | Effort | Business Value |
|---|---:|---:|---:|
| Create IT service request form | 1 | 5 | 100 |
| Store service requests in database | 1 | 8 | 95 |
| Add status tracking for submitted requests | 2 | 5 | 85 |

### Swimlane 3: Audit Logs and Notifications

| Ticket | Priority | Effort | Business Value |
|---|---:|---:|---:|
| Record audit logs for ticket updates | 2 | 5 | 90 |
| Send email notification when ticket status changes | 2 | 3 | 85 |
| Create admin dashboard for recent activity | 3 | 8 | 75 |

---

## 11. Effort Estimation

I used Fibonacci-style effort values for estimating the tickets.

Common Fibonacci effort values are:

```text
1, 2, 3, 5, 8, 13
```

For this board, I mainly used:

| Effort | Meaning |
|---|---|
| 3 | Smaller task with lower complexity |
| 5 | Medium task with some complexity |
| 8 | Larger task with more complexity and risk |

Example:

- Secure logout was estimated as **3** because it is smaller.
- Login page was estimated as **5** because it needs design and validation.
- Role-based access was estimated as **8** because it includes security and permission rules.

---

## 12. Priority Meaning

Priority was used to show which work is most important.

| Priority | Meaning |
|---|---|
| 1 | Very important / core feature |
| 2 | Important but not first priority |
| 3 | Useful feature but lower priority |

For example:

- Login and request form were Priority 1 because the system cannot work properly without them.
- Notifications were Priority 2 because they improve communication but are not the first core feature.
- Admin dashboard was Priority 3 because it is useful but can be built after core features.

---

## 13. Business Value Meaning

Business value shows how important a ticket is to the project and users.

Higher business value means the feature gives more benefit to students, staff, or IT administrators.

Examples:

| Business Value | Meaning |
|---|---|
| 100 | Very high value, required for core system |
| 95 | High value, important for security or storage |
| 85–90 | Useful and important supporting feature |
| 75–80 | Helpful feature but lower than core functions |

---

## 14. Ticket Details Template

Each ticket should include:

- Title
- Description
- Acceptance Criteria
- Priority
- Effort
- Business Value
- Start Date
- End Date
- Tags

If Azure DevOps does not show a separate field for Business Value, Start Date, or End Date, these can be added inside the description.

Example format:

```text
Business Value: 100
Start Date: June 20, 2026
End Date: June 24, 2026
```

---

## 15. Detailed Ticket Content

## Ticket 1: Implement college email login page

**Swimlane:** Login and Access Management  
**Column:** Analysis / Design  
**Priority:** 1  
**Effort:** 5  
**Business Value:** 100  
**Start Date:** June 20, 2026  
**End Date:** June 24, 2026  
**Tags:** login, authentication, student-access  

### Description

This ticket creates the login page for the Smart Campus IT Service Portal. Students and IT staff need a secure way to access the portal using their college email account. The login page should include the portal name, email sign-in option, clear error messages, and a simple user-friendly layout.

### Acceptance Criteria

- User can access the login page from the portal homepage.
- User can sign in using a valid college email account.
- Invalid login attempts show a clear error message.
- Page works on desktop and mobile.
- Login page supports keyboard navigation and readable labels.

---

## Ticket 2: Add role-based access for students and IT admins

**Swimlane:** Login and Access Management  
**Column:** Development  
**Priority:** 1  
**Effort:** 8  
**Business Value:** 95  
**Start Date:** June 24, 2026  
**End Date:** June 28, 2026  
**Tags:** roles, access-control, security  

### Description

This ticket adds role-based access control to separate student users from IT admin users. Students should only see their own service requests, while IT admins should be able to view, update, and manage all submitted requests. This improves security and protects user information.

### Acceptance Criteria

- Student users can only view and update their own requests.
- IT admins can view all service requests.
- Unauthorized users cannot access admin pages.
- Access control rules are documented clearly.
- Role permissions are tested with student and admin accounts.

---

## Ticket 3: Add secure logout and session timeout

**Swimlane:** Login and Access Management  
**Column:** Testing / QA  
**Priority:** 2  
**Effort:** 3  
**Business Value:** 80  
**Start Date:** June 28, 2026  
**End Date:** June 30, 2026  
**Tags:** logout, session, security  

### Description

This ticket adds secure logout and automatic session timeout to the portal. Users should be able to safely end their session, and inactive users should be logged out after a set time. This helps protect student and staff information if a device is left unattended.

### Acceptance Criteria

- User can log out from any page.
- Session ends after logout.
- Inactive users are automatically logged out after the timeout period.
- User is redirected to the login page after logout.
- Session timeout behaviour is tested.

---

## Ticket 4: Create IT service request form

**Swimlane:** Service Request Database  
**Column:** Analysis / Design  
**Priority:** 1  
**Effort:** 5  
**Business Value:** 100  
**Start Date:** June 21, 2026  
**End Date:** June 25, 2026  
**Tags:** form, service-request, student-support  

### Description

This ticket creates a service request form where students and staff can submit IT issues. The form should collect important information such as issue category, description, urgency level, contact information, and optional attachment details. This is the main feature of the portal.

### Acceptance Criteria

- User can open and complete the service request form.
- Required fields are clearly marked.
- Form validates missing or incorrect information.
- User can choose issue category and urgency level.
- Submitted form creates a new service request ticket.

---

## Ticket 5: Store service requests in database

**Swimlane:** Service Request Database  
**Column:** Development  
**Priority:** 1  
**Effort:** 8  
**Business Value:** 95  
**Start Date:** June 25, 2026  
**End Date:** June 30, 2026  
**Tags:** database, storage, service-request  

### Description

This ticket stores submitted service requests in a database so the information can be retrieved, updated, and tracked. Each request should include a unique ticket ID, user information, issue description, category, urgency, status, and created date.

### Acceptance Criteria

- Each submitted request is saved in the database.
- Each request receives a unique ticket ID.
- Request data includes user, category, urgency, status, and date.
- IT admins can retrieve saved requests.
- Database storage is tested with multiple sample requests.

---

## Ticket 6: Add status tracking for submitted requests

**Swimlane:** Service Request Database  
**Column:** Testing / QA  
**Priority:** 2  
**Effort:** 5  
**Business Value:** 85  
**Start Date:** June 30, 2026  
**End Date:** July 3, 2026  
**Tags:** status-tracking, support, workflow  

### Description

This ticket allows users to track the status of their submitted IT service requests. Status options should include Submitted, In Review, In Progress, Waiting for User, Resolved, and Closed. This helps students and staff understand what is happening with their request.

### Acceptance Criteria

- User can view the current status of a request.
- IT admins can update request status.
- Status changes are saved correctly.
- Status history is visible to admins.
- Users can easily understand what each status means.

---

## Ticket 7: Record audit logs for ticket updates

**Swimlane:** Audit Logs and Notifications  
**Column:** Testing / QA  
**Priority:** 2  
**Effort:** 5  
**Business Value:** 90  
**Start Date:** July 1, 2026  
**End Date:** July 4, 2026  
**Tags:** audit-logs, compliance, tracking  

### Description

This ticket records audit logs when an IT service request is created, updated, assigned, or closed. The audit log should track who made the change, what was changed, and when the change happened. This supports accountability and helps investigate issues.

### Acceptance Criteria

- Audit log is created when a request is submitted.
- Audit log is updated when status changes.
- Log records user, action, timestamp, and ticket ID.
- IT admins can review audit log entries.
- Audit log data cannot be edited by normal users.

---

## Ticket 8: Send email notification when ticket status changes

**Swimlane:** Audit Logs and Notifications  
**Column:** Security Review  
**Priority:** 2  
**Effort:** 3  
**Business Value:** 85  
**Start Date:** July 4, 2026  
**End Date:** July 6, 2026  
**Tags:** email, notification, status-update  

### Description

This ticket sends an email notification to the user when the status of their IT service request changes. The email should include the ticket ID, new status, short message, and portal link. This reduces confusion and keeps users informed.

### Acceptance Criteria

- User receives email when ticket status changes.
- Email includes ticket ID and new status.
- Email message is clear and professional.
- Notification is not sent for duplicate unchanged status.
- Email notification is tested with sample tickets.

---

## Ticket 9: Create admin dashboard for recent activity

**Swimlane:** Audit Logs and Notifications  
**Column:** Analysis / Design  
**Priority:** 3  
**Effort:** 8  
**Business Value:** 75  
**Start Date:** July 6, 2026  
**End Date:** July 10, 2026  
**Tags:** activity, admin-dashboard, monitoring  

### Description

This ticket creates an admin dashboard where IT staff can view recent portal activity. The dashboard should show new requests, status changes, recent audit log entries, and high-priority tickets. This helps IT admins monitor workload and respond faster.

### Acceptance Criteria

- Admin dashboard shows recent service requests.
- Dashboard shows recent status changes.
- Dashboard highlights high-priority tickets.
- Only IT admins can access the dashboard.
- Dashboard information updates correctly after ticket changes.

---

## 16. Screenshot Headings Used in the Report

The report should include screenshots with clear figure headings.

```text
Figure 1: Full Azure DevOps Board

Figure 2: Ticket 1 - Implement college email login page

Figure 3: Ticket 2 - Add role-based access for students and IT admins

Figure 4: Ticket 3 - Add secure logout and session timeout

Figure 5: Ticket 4 - Create IT service request form

Figure 6: Ticket 5 - Store service requests in database

Figure 7: Ticket 6 - Add status tracking for submitted requests

Figure 8: Ticket 7 - Record audit logs for ticket updates

Figure 9: Ticket 8 - Send email notification when ticket status changes

Figure 10: Ticket 9 - Create admin dashboard for recent activity
```

---

## 17. Written Report Used for Assignment

## IT Use Case Report: Smart Campus IT Service Portal

The Smart Campus IT Service Portal is a proposed web-based system that can help students and staff submit and track IT support requests in one place. The main purpose of this system is to make the support process more organized and easier for both users and IT administrators. Instead of only depending on email or asking in person, students and staff can log in with their college account, submit an IT issue, check the request status, and receive updates when there is progress.

For this assignment, I created an Azure DevOps board to organize the project work into three main feature areas: Login and Access Management, Service Request Database, and Audit Logs and Notifications. These swimlanes show the major parts of the system. The Login and Access Management swimlane is about secure login, user roles, logout, and session timeout. The Service Request Database swimlane is about creating request forms, saving submitted requests, and tracking their status. The Audit Logs and Notifications swimlane is about keeping records of changes, sending status notifications, and helping admins monitor recent activity.

The board columns were also customized to follow an IT DevOps lifecycle. The columns used are Backlog, Analysis / Design, Development, Testing / QA, Security Review, Deployment, and Done. This helps show how the work moves from planning to completion. Each ticket includes important details such as description, priority, effort estimate, business value, start date, end date, acceptance criteria, and tags. I used Fibonacci-style effort values such as 3, 5, and 8 because this is a common way to estimate how much work or complexity a ticket may have. Priority was added based on how important each feature is for the main system.

This board shows how an IT team can take a larger system and break it into smaller manageable work items. It also shows the importance of planning, communication, estimation, and tracking in a team project. The tickets are connected to the use case because each ticket represents a feature that would be needed to make the Smart Campus IT Service Portal useful, secure, and easier to manage for students, staff, and IT administrators.

---

## 18. AI Assistance Statement

I used ChatGPT as a learning and drafting support tool to understand the Azure DevOps board structure, organize the ticket ideas, and improve wording and grammar. I reviewed, edited, and finalized the board, tickets, screenshots, and report myself.

---

## 19. Small Mistake I Learned From

At the beginning, I accidentally created some columns as tickets, such as Security Review and Deployment. Later, I understood the difference:

| Item | Meaning |
|---|---|
| Column | Shows the work stage |
| Swimlane | Shows the feature area |
| Ticket | Shows the actual task/work item |

After understanding this, I deleted the incorrect test tickets and created the correct board structure.

This is why some Azure DevOps ticket numbers may not start from 1. Azure DevOps keeps the old work item ID numbers even if earlier test items are deleted. This does not affect the final board because the final board contains the required 9 valid tickets.

---

## 20. Final Board Structure

Final structure:

```text
Smart Campus IT Service Portal
│
├── Login and Access Management
│   ├── Implement college email login page
│   ├── Add role-based access for students and IT admins
│   └── Add secure logout and session timeout
│
├── Service Request Database
│   ├── Create IT service request form
│   ├── Store service requests in database
│   └── Add status tracking for submitted requests
│
└── Audit Logs and Notifications
    ├── Record audit logs for ticket updates
    ├── Send email notification when ticket status changes
    └── Create admin dashboard for recent activity
```

---

## 21. What I Learned

From this assignment, I learned that Azure DevOps Boards can be used to organize IT project work in a clear and structured way. I learned the difference between columns, swimlanes, and tickets. I also learned that a larger system should be broken into smaller work items so that a team can plan, estimate, track, and complete the work more effectively.

This assignment also helped me understand how team communication and project tracking are connected. A good board makes it easier for everyone to see what needs to be done, what is in progress, and what has already been completed.

---

## 22. Cost and Cleanup Notes

For this assignment, I only used Azure DevOps Boards. I did not create paid Azure cloud resources.

This type of board project should not create normal Azure cloud charges because it is not creating resources such as:

- Virtual machines
- Databases
- Storage accounts
- AKS clusters
- App Services

To avoid unnecessary cost, I should not enable paid services unless required, such as:

- Extra paid users
- Test Plans
- Paid extensions
- Heavy pipeline usage
- Azure cloud infrastructure resources

If I want to delete the project later, I can go to:

```text
Project settings → Overview → Delete project
```

However, it is better to keep the project until the assignment is graded.

---

## 23. Future Use

This Markdown file can be saved in GitHub as a learning note for Azure DevOps Boards and project planning. It can also be useful for future assignments, team projects, and interview preparation because it shows how to explain:

- Azure DevOps Boards
- Project planning
- Swimlanes
- Columns
- Tickets/work items
- Effort estimation
- Priority
- Business value
- IT DevOps lifecycle
