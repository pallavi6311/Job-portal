# Job-portal
A web-based Job Portal System built with Java Swing (frontend) and MySQL (backend). The system connects job seekers and employers by enabling job posting, job applications, and user profile management with secure authentication.

# Job Portal System

## 📌 Project Overview

The **Job Portal System** is a web-based application designed to connect job seekers with employers.
Employers can post job vacancies, and job seekers can search and apply for jobs through an interactive platform.
The system manages job postings, applications, and user profiles securely using a Java Swing frontend and MySQL backend.

---

## 🎯 Objectives

* Provide a platform for employers to post job vacancies.
* Enable job seekers to search and apply for jobs.
* Manage user profiles and job applications efficiently.
* Ensure secure authentication and data storage.

---

## 🛠️ Technologies Used

* **Frontend:** Java Swing (GUI)
* **Backend:** MySQL
* **IDE/Tools:** Visual Studio Code / NetBeans / Eclipse
* **Languages:** Java, SQL

---

## 🧩 Modules

1. **Login Module** – Secure user login with role-based redirection (Employer / Job Seeker).
2. **Registration Module** – New user registration with validation and database storage.
3. **Job Posting Module** – Employers can post jobs with details (title, description, salary, skills, deadline).
4. **Apply Job Module** – Job seekers can browse, apply, and upload resumes.

---

## 📊 ER Diagram

(Insert your ER diagram image here – e.g., `docs/ER_diagram.png`)

---

## 🚀 How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/job-portal-system.git
   cd job-portal-system
   ```
2. Import the project into your IDE (Eclipse / NetBeans / VS Code).
3. Configure the database:

   * Create a new MySQL database (e.g., `job_portal`).
   * Import the provided `job_portal.sql` file from the `database/` folder.
4. Update database credentials in the Java code (`DBConnection.java`).
5. Run the application.

---

## 📷 Screenshots

(Add screenshots of Login, Registration, Job Posting, and Job Apply pages here in a `screenshots/` folder.)

---

## 📌 Queries (Sample SQL)

Examples of queries used in the project:

```sql
-- Fetch all available jobs
SELECT * FROM jobs;

-- Insert new job posting
INSERT INTO jobs (title, description, location, salary, skills)
VALUES ('Software Engineer', 'Backend Developer Role', 'Chennai', 40000, 'Java, SQL');

-- Get applications for a specific job
SELECT * FROM applications WHERE job_id = 1;
