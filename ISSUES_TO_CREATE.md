# Issue drafts for extracurricular activity management

## 1. Add persistent database support and attendance tracking
### Description
Right now the app stores activities in memory only. Add a persistent backend so activity data, signups, and attendance records survive server restarts.

### Acceptance criteria
- Add a database connection (SQLite, PostgreSQL, etc.)
- Store activities, participants, and attendance records in the database
- Replace in-memory activity dictionary with persisted records
- Add endpoints for creating and querying attendance entries

---

## 2. Add role-based authentication and admin control
### Description
The club management repo supports different user roles and protected pages. Add login/authentication and admin-only endpoints so only authorized users can manage events and attendance.

### Acceptance criteria
- Add login and logout endpoints
- Support at least two roles: normal user and admin
- Protect management endpoints behind role checks
- Add password recovery or admin contact flow if possible

---

## 3. Add club and event role management
### Description
Support adding and managing club coordinators, club secretaries, event coordinators, and event assistants.

### Acceptance criteria
- Add models/endpoints for coordinator, secretary, and event assistant records
- Allow admins to add/update role assignments
- Track which users are assigned to each club or event role

---

## 4. Add reporting and export tools for attendance
### Description
Provide admin-facing reporting and export capabilities, such as viewing attendance records and exporting them as CSV.

### Acceptance criteria
- Add endpoint(s) for retrieving attendance reports
- Support filtering by student, event, or date
- Add CSV export endpoint or file download
- Add UI or API documentation for report generation
