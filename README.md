# 🎓 Online Courses Platform

<p align="center">
  <b>A Learning Management System (LMS) built with ASP.NET Core MVC</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/.NET-ASP.NET%20Core-blue?style=for-the-badge&logo=dotnet" />
  <img src="https://img.shields.io/badge/Architecture-Layered-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/ORM-Entity%20Framework%20Core-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Database-SQL%20Server-red?style=for-the-badge" />
</p>

---

# 🚀 Overview

Online Courses Platform is a Learning Management System (LMS) developed using ASP.NET Core MVC. The platform provides a complete learning environment where students can enroll in courses, instructors can create and manage educational content, and administrators can oversee and moderate the platform.

The project was built to simulate a real-world online learning system while applying modern backend development practices and scalable application architecture.

---

# 👥 User Roles

## 🎓 Student

* Browse available courses
* Search and filter courses
* Enroll in courses
* Track learning progress
* Complete lessons and quizzes
* Continue learning from the last completed lesson
* Submit course reviews and ratings

## 👨‍🏫 Instructor

* Create and manage courses
* Upload course thumbnails
* Organize courses into sections and lessons
* Add educational content
* Track instructor statistics
* Manage personal course catalog

## 🛡️ Admin

* Manage users and roles
* Approve or reject submitted courses
* Manage categories
* Manage tags
* Manage currencies
* Monitor platform activities

---

# ✨ Key Features

## 🔐 Authentication & Authorization

* ASP.NET Identity integration
* Registration and login system
* Role-Based Authorization
* Protected resources and actions
* User profile management
* Password reset functionality
* Change password support

---

## 📚 Course Management

* Create courses
* Edit courses
* Delete courses
* Upload course images
* Assign categories and tags
* Set course pricing and currencies

### Course Workflow

```text
Pending
   ↓
Approved
   ↓
Rejected
```

Courses must be reviewed and approved by administrators before becoming publicly available.

---

## 🎥 Learning Content System

Each course is structured as:

```text
Course
 └── Sections
      └── Lessons
```

Supported lesson types:

* Video Lessons
* Article Lessons
* PDF Resources
* Quiz Lessons

---

## 📝 Quiz Engine

The platform includes an integrated quiz system:

* Multiple Choice Questions
* True / False Questions
* Answer Validation
* Progress Integration

---

## 📈 Learning Progress Tracking

Students can:

* Track completed lessons
* View course completion percentage
* Continue learning from the next lesson
* Monitor learning progress through dashboards

---

## ⭐ Reviews & Ratings

Students can:

* Rate courses
* Write reviews
* Update existing reviews

The platform automatically calculates:

* Average rating
* Total review count

---

## 🔍 Search & Filtering

Courses can be filtered using:

* Search keywords
* Categories
* Tags

Additional features:

* Pagination
* Dynamic filtering
* Course discovery

---

# 🏗 Architecture

The project follows a layered architecture that separates concerns and improves maintainability.

```text
Presentation Layer
├── Controllers
├── Views
└── ViewModels

Business Layer
├── Services
├── DTOs
└── AutoMapper Profiles

Data Access Layer
├── Repositories
├── Entity Framework Core
└── SQL Server

Infrastructure Layer
├── ASP.NET Identity
├── File Storage
└── Content Management

Domain Layer
└── Models
```

---

# 🛠 Design Patterns & Practices

* Repository Pattern
* Service Layer Pattern
* DTO Pattern
* Dependency Injection
* AutoMapper
* Role-Based Authorization
* Entity Framework Core
* Separation of Concerns

---

# ⚙️ Tech Stack

## Backend

* ASP.NET Core MVC
* Entity Framework Core
* ASP.NET Identity
* SQL Server
* AutoMapper

## Frontend

* Razor Views
* Bootstrap
* JavaScript
* AJAX

## Development Tools

* Visual Studio
* Git
* GitHub

---

# 🗄 Database Design

### Core Entities

```text
User
AdminProfile

Course
Category
Tag
CourseTag

Section
Lesson

Enrollment
UserProgress

Review

Currency
```

Entity relationships are managed using Entity Framework Core and SQL Server.

---

# 📂 Project Structure

```text
OnlineCoursesPlatform
│
├── Controllers
├── Data
├── Dtos
├── Infrastructure
├── Mappings
├── Models
├── Repositories
│   ├── Interfaces
│   ├── Repository.cs
│   └── CourseRepository.cs
│
├── Services
│   ├── Interfaces
│   ├── AccountService.cs
│   ├── AdminService.cs
│   ├── CourseService.cs
│   ├── EnrollmentService.cs
│   ├── InstructorService.cs
│   ├── LearningService.cs
│   └── LessonService.cs
│
├── ViewModels
├── Views
├── wwwroot
└── Migrations
```

---

# 🔥 Highlights

* Multi-role platform (Student, Instructor, Admin)
* Course approval workflow
* Enrollment system
* Learning progress tracking
* Quiz-based learning experience
* Reviews and ratings system
* File upload support
* Search, filtering, and pagination
* Layered architecture
* ASP.NET Identity integration
* Repository & Service patterns

---

# 📸 Screenshots

## Home Page

<p align="center">
  <img src="./screenshots/Home.jpeg" width="85%">
</p>

## Courses Listing

<p align="center">
  <img src="./screenshots/courses.jpeg" width="85%">
</p>

## Course Details

<p align="center">
  <img src="./screenshots/course-details.jpeg" width="85%">
</p>

## Enrollment Flow

<p align="center">
  <img src="./screenshots/enrollment.jpeg" width="85%">
</p>

## Learning Experience

<p align="center">
  <img src="./screenshots/learning.jpeg" width="85%">
</p>

## Instructor Dashboard

<p align="center">
  <img src="./screenshots/instructor-dashboard.jpeg" width="85%">
</p>

## Admin Dashboard

<p align="center">
  <img src="./screenshots/admin-dashboard.jpeg" width="85%">
</p>

---

# 👨‍💻 Team

* Ahmed Aldsoaky
* Amr Alsaftawi
* Mohamed Elsheikh

---

# 🚀 Getting Started

## Clone Repository

```bash
git clone https://github.com/amralsaftawi/OnlinCoursesPlatform.git
```

## Apply Migrations

```bash
Update-Database
```

## Run Application

```bash
dotnet run
```

---

# 📌 Educational Purpose

This project was developed as a team-based academic project to simulate a real-world Learning Management System using ASP.NET Core MVC and modern backend development practices.

It demonstrates:

* Layered Architecture
* Authentication & Authorization
* Entity Framework Core
* Repository Pattern
* Service Layer
* Learning Management Workflows
* Real-world Business Logic

---

<p align="center">
  Built with ❤️ using ASP.NET Core MVC
</p>
