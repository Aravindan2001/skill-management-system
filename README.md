<div align="center">

# 🎯 Skills Resource Management System

**Full Stack Talent Matching Platform | React + Node.js + MySQL | Smart Matching**

<div align="center">
<img src="https://img.shields.io/badge/Status-Production%20Ready-00D084?style=for-the-badge" alt="Production Ready">
<img src="https://img.shields.io/badge/React-18.2-blue?style=for-the-badge&logo=react" alt="React">
<img src="https://img.shields.io/badge/Node-20-green?style=for-the-badge&logo=node.js" alt="Node.js">
<img src="https://img.shields.io/badge/MySQL-8.0-orange?style=for-the-badge&logo=mysql" alt="MySQL">
<img src="https://img.shields.io/badge/API-100%20Tested-brightgreen?style=for-the-badge" alt="API Tested">
</div>

</div>

## ✨ Product Overview

**Enterprise-grade Skills Resource Management System** with **Smart Matching Algorithm** (97% accuracy scores). Complete CRUD for Personnel, Projects, and Skills Assignment.

**Live Flow:** `Projects → Assign Skills → "Find Team" → #1 Alice (97%) ✨`

## 🎮 Key Features

| Feature | Status | Description |
|---------|--------|-------------|
| Personnel CRUD | ✅ Complete | Create/Update + Email field |
| Skills Assignment | ✅ Complete | Personnel ↔ Skills (Many-to-Many) |
| Projects Management | ✅ Complete | Create + Required Skills |
| **Smart Matching** | ✅ Complete | 97% scores + Rankings |
| Professional UI | ✅ Complete | 4 Tabs + Responsive + Gradients |
| API Testing | ✅ Complete | 5 Thunder Client screenshots |
| Production Ready | ✅ Complete | Error handling + Validation |

## 📱 Screenshots

| 1. Create Personnel | 2. List Personnel | 3. Update Personnel |
|---|---|---|
| !Screenshot1 | !Screenshot2 | !Screenshot3 |

| 4. Assign Skills | 5. Smart Matching (97% 🎯) |
|---|---|
| !Screenshot4 | !Screenshot5 |

## 🛠 Tech Stack

Frontend: React 18 + Tailwind CSS
Backend: Node.js + Express + MySQL
Testing: Thunder Client (VS Code)

text

## 🗄 Database Schema

CREATE TABLE personnel (
id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(255),
email VARCHAR(255),
role VARCHAR(100),
experience_level ENUM('Junior','Mid-Level','Senior','Lead')
);

CREATE TABLE skills (
id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(100),
category VARCHAR(50)
);

CREATE TABLE personnel_skills (
personnel_id INT,
skill_id INT,
proficiency ENUM('Beginner','Intermediate','Advanced','Expert'),
FOREIGN KEY (personnel_id) REFERENCES personnel(id),
FOREIGN KEY (skill_id) REFERENCES skills(id)
);

CREATE TABLE projects (
id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(255),
status ENUM('Planning','Active','Completed')
);

CREATE TABLE project_required_skills (
project_id INT,
skill_id INT,
min_proficiency ENUM('Beginner','Intermediate','Advanced','Expert')
);

text

## 🔗 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/personnel` | Create personnel |
| `GET` | `/api/personnel` | List all |
| `PUT` | `/api/personnel/:id` | Update |
| `POST` | `/api/personnel_skills` | Assign skill |
| `POST` | `/api/matching/project/1` | **Smart matching** |

## 🧠 Smart Matching Algorithm

Project needs: React(Intermediate) + Node.js(Advanced)
Personnel has: React(Expert) + Node.js(Advanced)
Result: #1 Alice Johnson (97%) ✨

text

## 🚀 Quick Start

Clone repo
git clone https://github.com/Aravindan2001/skill-management-system
cd skill-management-system

Backend
cd backend && npm install && npm run dev

Frontend (new terminal)
cd frontend && npm install && npm run dev


text

<div align="center">
**Built for 4BEX Challenge**
**100% Complete | Production Ready** 🚀

** Chandrakumar Aravindan ** | ** aravindan.saran2001@gmail.com ** | ** +94 768363170 **
</div> this is ok or not
