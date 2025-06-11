# 🌟 HireHub

A clean, modern job portal web application built with **HTML5** and **Tailwind CSS**.  
HireHub lets **job seekers** browse and apply for positions, and **companies** view applicants—all in a responsive, professional UI.  

---

## 📝 Project Overview

- **Purpose**: Connect job seekers and recruiters on one platform  
- **Users**:-
  - **Job Seekers** browse, search, and apply to jobs  
  - **Companies** post jobs and manage applications  
  - **Admins** (optional) oversee users, companies, and listings  

---

## 📄 Frontend Pages

| #  | Page Name         | Role          | Description                                 |
|---:|-------------------|---------------|---------------------------------------------|
| 1️⃣ | **index.html**     | Shared        | Landing page with navigation                |
| 2️⃣ | **login.html**     | Shared        | User/Company login form                     |
| 3️⃣ | **register.html**  | Shared        | User & Company sign-up (tabs or dropdown)   |
| 4️⃣ | **jobs.html**      | Job Seeker    | Search, filter, and list active jobs        |
| 5️⃣ | **apply.html**     | Job Seeker    | Apply to a job with cover letter/resume URL |
| 6️⃣ | **applications.html** | Job Seeker | View submitted applications & statuses      |
| 7️⃣ | **dashboard.html** | User & Company| Profile, stats, and quick links             |
| 8️⃣ | **post-job.html**  | Company       | Create/Edit job postings                    |
| 9️⃣ | **manage-jobs.html** | Company     | View/Edit/Delete job listings               |
| 🔟 | **admin.html**      | Admin (opt.)  | Manage users, companies & jobs              |
| 1️⃣1️⃣ | **404.html**    | Shared        | Fallback for broken links                   |

---

## 🔧 Backend API Endpoints

> Implement these with **Spring Boot + Spring Security (JWT)** or similar.

| Action                    | HTTP Method | Endpoint                  | Role        |
|---------------------------|------------:|---------------------------|-------------|
| **Register**              | POST        | `/api/auth/register`      | Public      |
| **Login**                 | POST        | `/api/auth/login`         | Public      |
| **Get Current User**      | GET         | `/api/user/me`            | Authenticated |
| **List All Jobs**         | GET         | `/api/jobs`               | Public      |
| **Get Job Details**       | GET         | `/api/jobs/{id}`          | Public      |
| **Search/Filter Jobs**    | GET         | `/api/jobs?keyword=&loc=` | Public      |
| **Post New Job**          | POST        | `/api/jobs`               | Company     |
| **Update Job**            | PUT         | `/api/jobs/{id}`          | Company     |
| **Delete Job**            | DELETE      | `/api/jobs/{id}`          | Company     |
| **Apply to Job**          | POST        | `/api/applications`       | Job Seeker  |
| **Get User Applications** | GET         | `/api/applications/me`    | Job Seeker  |
| **Get Company Applicants**| GET         | `/api/applications/job/{id}` | Company   |
| **Admin: List Users**     | GET         | `/api/admin/users`        | Admin       |
| **Admin: List Companies** | GET         | `/api/admin/companies`    | Admin       |

---

## ⚙️ Tech Stack

- **Frontend**: HTML5, Tailwind CSS (CDN), JavaScript  
- **Backend**: Java, Spring Boot, Spring Security (JWT)  
- **Database**: MySQL / PostgreSQL + JPA/Hibernate  
- **Version Control**: Git & GitHub  

---

## 🚀 Getting Started

1. **Clone Repo**  
   ```bash
   git clone https://github.com/ThakareYashodip/hirehub.git
   cd hirehub
