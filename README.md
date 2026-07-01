# CourseTrack — Student Course Management & Learning Progress Tracking System

A full-stack web application for course enrollment and learning progress tracking, built for students to manage their courses and for administrators to manage students, courses, and enrollments.

## Problem Statement

In many educational institutions, students struggle to:

- Find available courses
- Register for courses efficiently
- Monitor their learning progress
- Access course information in one place
- Track completed and pending modules

Administrators, in turn, face difficulty managing course enrollments and monitoring student performance across many students and courses at once.

**CourseTrack** solves this by providing a centralized, web-based platform where students can browse, enroll, and track progress, and administrators can manage the entire course lifecycle from one dashboard.

## Objectives

- Provide secure student registration and login
- Allow students to view and enroll in courses
- Enable administrators to create and manage courses
- Track student learning progress module by module
- Generate progress reports
- Provide real-time notifications and updates
- Maintain secure access to academic data

## User Roles

**Student** — register/login, view profile, browse and enroll in courses, access course content, track progress, view completion percentage, receive notifications.

**Administrator** — secure login, add/edit/delete courses, manage students, monitor enrollments, generate reports, update course content, view an analytics dashboard.

## Features

| Module | Features |
|---|---|
| User Authentication | Registration, login, password encryption, forgot password, JWT authentication |
| Course Management | Add / update / delete courses, view course details |
| Course Enrollment | Browse, search, enroll, view enrolled courses |
| Learning Management | View modules, access materials, mark modules complete, continue learning |
| Progress Tracking | Completion percentage, progress bar, completed/pending modules |
| Dashboards | Student dashboard (enrolled/completed/ongoing/stats), Admin dashboard (students/courses/enrollments/reports) |
| Notifications | New course alerts, enrollment confirmations, reminders, completion certificates (Socket.IO) |

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, JavaScript, React.js |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| Authentication | JWT, bcrypt |
| Real-time Communication | Socket.IO |
| API Testing | Postman |
| Version Control | Git, GitHub |
| Deployment | Render / Vercel / Railway |

## Database Design (overview)

**Students** — `student_id`, `name`, `email`, `password`, `department`
**Courses** — `course_id`, `course_name`, `instructor`, `duration`, `description`
**Enrollment** — `enrollment_id`, `student_id`, `course_id`, `enrollment_date`
**Progress** — `progress_id`, `student_id`, `course_id`, `completed_modules`, `progress_percentage`

## Project Structure

```
coursetrack/
├── README.md
├── index.html          # Home page
├── login.html           # Login page
├── register.html        # Registration page
├── dashboard.html        # Student dashboard
├── css/
│   └── style.css
├── js/
│   └── script.js
├── backend/              # (to be added in the backend phase)
│   ├── server.js
│   ├── routes/
│   ├── models/
│   └── controllers/
└── docs/
    └── Full_stack_detailed_explanation.docx
```

## Current Status

- [x] Repository created and documented
- [x] Static frontend structure: Home, Login, Register, Dashboard
- [ ] Backend API (Node.js/Express)
- [ ] Database integration (MongoDB)
- [ ] Authentication (JWT)
- [ ] Real-time notifications (Socket.IO)
- [ ] Deployment

## Getting Started

Clone the repo and open `index.html` in a browser — no build step is required for the current static frontend.

```bash
git clone https://github.com/<your-username>/coursetrack.git
cd coursetrack
```
