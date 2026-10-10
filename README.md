# EduPulse | Student Management System (SMS)

A modern, responsive, zero-backend Student Management System website built with **HTML5**, **Tailwind CSS**, and **vanilla JavaScript (ES6+)**. The system uses the browser's **LocalStorage** for persistent storage, making it completely self-contained with no servers or build tools required.

---

## 🌟 Key Features

1. **Executive Dashboard**:
   - Institutional KPIs: Total Enrolled Students, Active Courses, Average Attendance Rate, Cumulative Institutional GPA.
   - Real-time interactive charts (Department enrollment bar chart and Attendance ratio doughnut chart powered by Chart.js).
   - Top academic performers leaderboard and course capacity meters.

2. **Student Directory & Profile Management (CRUD)**:
   - Full student profile management: ID, First/Last Name, Email, Phone, Date of Birth, Gender, Department/Major, Academic Year, Status (Active/Suspended/Graduated), Guardian details, and Residential Address.
   - Live real-time search across student names, IDs, and emails.
   - Filter by Academic Department and Enrollment Status.
   - Add, Edit, View, and Delete students.
   - One-click CSV export of student directory.
   - Comprehensive student profile modal featuring course breakdown, attendance standing, and transcript summary.

3. **Course Catalog & Class Enrollment**:
   - Course tracking: Course Code, Course Name, Credits, Instructor, Semester, Capacity, and Course Descriptions.
   - Capacity progress bars showing current enrollment ratios.
   - Interactive enrollment roster modal allowing one-click toggling of enrolled students per course.

4. **Attendance Tracking**:
   - Daily/session-based attendance recording by course and date.
   - Quick bulk status buttons: "All Present", "All Absent".
   - Individual status choices: **Present**, **Late**, **Absent**, and **Excused**.
   - Automatic student attendance percentage calculations with color-coded badges.

5. **Grades & Academic Report Cards**:
   - Record assessment scores (Midterms, Finals, Quizzes, Projects, Assignments).
   - Automatic percentage computation and letter grade mapping (A, A-, B+, B, C, D, F) with 4.0 GPA scale points.
   - **Official Printable Report Card / Transcript**:
     - Formal academic transcript layout with university header, student details, course-by-course grades, credit hours, cumulative GPA, attendance summary, honor roll / academic standing, and registrar signatures.
     - Print-ready with CSS `@media print` styling (click "Print Transcript" or press `Ctrl + P`).

6. **Data Portability & Dark Mode**:
   - Light & Dark mode toggle with persistent preferences.
   - Full JSON database backup export and restore file uploader.
   - One-click demo dataset reset.

---

## 🚀 How to Run the Website

Because this is a pure client-side web application, you do not need Node.js, Python, or any web server to get started!

### Option 1: Open Directly in Any Browser
Simply double-click [`index.html`](file:///C:/Users/ABC/.gemini/antigravity/scratch/student-management-system/index.html) or right-click and choose **Open With -> Google Chrome / Microsoft Edge / Firefox / Brave**.

### Option 2: Run with a Local Static Server (Optional)
If you prefer running via a local HTTP server:
```powershell
# Using Python
cd "C:\Users\ABC\.gemini\antigravity\scratch\student-management-system"
python -m http.server 8000
```
Then visit: `http://localhost:8000`

---

## 📁 File Structure

```text
student-management-system/
├── index.html          # Main application structure, layouts, navigation, and modals
├── css/
│   └── style.css       # Custom styles, animations, scrollbars, and print layout
├── js/
│   ├── data.js         # Initial seed dataset, data models, and LocalStorage service
│   └── app.js          # Controllers, navigation, Chart.js integrations, CRUD logic, and events
└── README.md           # Documentation and guide
```
