# CSE302: Database Systems Project
Academic & Project Performance Management System (Oracle APEX)

## Project Overview
This project is a web-based database application developed using Oracle APEX. The application manages student academic records, project group allocations, marks distribution, and course outcomes. It bridges the gap between students, instructors, and supervisors by providing a centralized platform for academic data management.

Platform: Oracle APEX  
Database: Oracle SQL  
Role Management: Admin, Instructor, and Student roles with specific authorization levels  
Application URL: Live Demo  

## Database Architecture

### 1. E-R Model Highlights
The E-R diagram was designed based on complex academic constraints:

- Project Groups: Each project group must have at least one Project ID  
- Student Allocation: Many-to-one relationship between students and project groups  
- Marks Distribution: Multi-criteria marks assignment involving instructors and supervisors  
- Course Relationships: Many-to-many relationship between Students and Courses implemented via a Registration bridge table  

### 2. Relational Model
Key implementation features include:

- Registration Table: Tracks student-course enrollment  
- CO-Domain Mapping: Many-to-many relationships between Course Outcomes (CO), Affective Domains, and Psychomotor Domains  

## Features & Functionalities

### Authentication & Authorization
- Secure login system with role-based access control:
  - Admin  
  - Instructor  
  - Student  

### Master-Detail Forms
- Course ↔ Section Details  
- Board ↔ Instructor Details  
- Supervisor ↔ Course Outcome Details  

### Comprehensive Reporting
- 31 reports with integrated forms for data entry  

### Image Management
- Upload and display:
  - Instructor images  
  - Supervisor images  

### Marks Management
- Dynamic marks distribution system  
- Marks assigned by multiple evaluators  

## Login Credentials (Testing Purpose)

Administrator:
Username: admin
Password: admin123

Student:
Username: student
Password: student123

Instructor:
Username: instructor
Password: instructor123  

## Implementation Details

- Total Report-Forms: 31  
- Master-Detail Forms: 3  
- Image Handling: Image upload and display implemented  
- Page-level Security: Admin-only restricted pages enabled  
