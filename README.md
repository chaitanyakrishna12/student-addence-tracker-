# student-addence-tracker-
A project to track student addence tracker 
Build a polished, responsive **Student Attendance Tracker** website for schools, colleges, and training centers. The site should make it easy for teachers to record attendance and for administrators to review attendance trends.

## Product goals

- Make taking attendance quick and intuitive.
- Help staff find students and classes without digging through menus.
- Show useful attendance summaries and flag students who may need follow-up.
- Work well on desktop, tablet, and mobile.

## Users and roles

- **Administrator:** manages users, classes, subjects, students, and academic terms; can view reports across the institution.
- **Teacher:** views assigned classes and records or edits attendance for their classes.
- **Student or parent (optional):** can view attendance history and summaries, but cannot edit records.

Use role-based permissions throughout the interface. If authentication or a real database is outside the builder’s capabilities, create a realistic demo experience and clearly identify placeholder data.

## Main pages

1. **Sign in**
   - Email and password fields, show/hide password, validation, and a clear error state.
   - Include demo sign-in options for administrator and teacher if this is a prototype.

2. **Dashboard**
   - Today’s attendance rate, present, absent, and late counts.
   - Classes scheduled today and their attendance status.
   - A simple attendance trend chart.
   - A “needs attention” list for students below a configurable attendance threshold.
   - Date and class filters where relevant.

3. **Take attendance**
   - Choose class, subject, and date.
   - Show a searchable student roster with photo or initials, student ID, and attendance status.
   - Provide clear **Present**, **Absent**, **Late**, and **Excused** controls.
   - Include “Mark all present,” but require a review before saving.
   - Show an unsaved-changes warning and a confirmation after saving.
   - Prevent duplicate records for the same student, class, subject, and date.

4. **Students**
   - Searchable, sortable student list with class, student ID, and attendance percentage.
   - Student detail page with attendance history, summary, and relevant notes.
   - Add, edit, and archive students.

5. **Classes and subjects**
   - View classes, enrolled students, assigned teachers, and subjects.
   - Allow authorized staff to create and edit these records.

6. **Attendance reports**
   - Filter by date range, class, subject, student, and status.
   - Show attendance summaries and trends.
   - Support CSV export if possible.
   - Make empty, loading, and error states clear.

7. **Settings**
   - Manage academic terms and configurable attendance thresholds.
   - Manage users and roles for administrators.
   - Provide a clear sign-out action.

## Design direction

Create a calm, professional education-focused interface. Use a light background, readable typography, strong contrast, and a restrained accent color. Use consistent spacing, clear page titles, accessible form labels, visible keyboard focus, and status indicators that do not rely on color alone. Include a sidebar on desktop and a compact navigation pattern on mobile. Avoid clutter, tiny text, and unnecessary animation.

## Behavior and data

- Use realistic sample data for students, classes, subjects, and attendance.
- Keep filters, search, navigation, and attendance controls functional.
- Validate required fields and show helpful inline messages.
- Ask for confirmation before destructive actions such as deleting or archiving.
- Display dates consistently and make the selected date obvious.
- Preserve entered data if the user navigates away accidentally, where the platform allows.
- Do not expose one user’s records to another role without permission.

## Technical requirements

Use the platform’s recommended stack and conventions. Build reusable components and keep the project organized. If a backend is supported, use secure authentication, a persistent database, and server-side role checks. Model attendance so each record connects a student, class, subject, date, status, and the staff member who recorded it. Handle loading, empty, validation, and failure states.

If a real backend is not available, use local demo data and make the prototype usable without external services. Do not claim that authentication, persistence, or data exports are production-ready unless they actually work.

## Acceptance criteria

- A teacher can select a class and date, mark attendance, review it, and save it.
- A teacher can search the roster and change an individual student’s status.
- An administrator can find a student and review attendance trends.
- Filters and reports produce consistent results from the available data.
- The interface is responsive, accessible, and understandable without instructions.
- The finished site includes realistic sample data and no dead-end buttons.
