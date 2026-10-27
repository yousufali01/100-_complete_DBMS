# 🎓 MicroTeach — Academic Peer Tutoring Platform

MicroTeach is a database-driven academic peer tutoring platform designed to connect students with tutors, help learners discover academic support, and manage tutoring activities through a centralized system.

The project was developed as part of a Database Management Systems (DBMS) course, focusing on relational database design, data integrity, and backend integration with MySQL.

## 📖 Project Overview

MicroTeach provides a platform where learners can explore tutoring opportunities, apply for tutoring posts, communicate with other members, and participate in tutoring sessions.

The system supports multiple user roles and manages related academic activities through a structured relational database. It uses foreign keys, constraints, and indexes to maintain data consistency and support efficient data access.

## ✨ Key Features

- 👥 **User Management** — Manage platform users and their roles.
- 🧠 **Skills Management** — Store and organize user skills.
- 📚 **Tutoring Posts** — Create and manage tutoring opportunities.
- 📝 **Tutor Applications** — Support teacher applications and applications to tutoring posts.
- 📅 **Tutoring Sessions** — Manage tutoring session records.
- ⭐ **Reviews and Ratings** — Store reviews associated with the tutoring experience.
- 💬 **Messaging System** — Manage conversations, conversation members, and messages.
- 🚩 **Reporting System** — Maintain reports related to platform activities.
- 💰 **Wallet Transactions** — Track wallet-related transaction records.
- 🔐 **Password Security** — Use bcrypt-based password hashing.
- 🗄️ **Relational Data Management** — Maintain relationships between database entities using foreign keys and constraints.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Node.js | Backend runtime environment |
| MySQL | Relational database management |
| mysql2/promise | MySQL connectivity and promise-based database operations |
| bcryptjs | Password hashing |
| dotenv | Environment variable configuration |
| SQL | Database schema and data management |

## 🗄️ Database Design

The project uses a MySQL database named `microteach_db`.

The database organizes information into related tables to support the platform's core functionality.

### Main Database Entities

- Users and user roles
- Skills
- Tutoring posts
- Sessions
- Teacher applications
- Post applications
- Reports
- Wallet transactions
- Reviews
- Conversations
- Conversation members
- Messages

### Database Integrity and Optimization

The database schema includes:

- **Primary keys** to identify records.
- **Foreign keys** to establish relationships between entities.
- **Unique constraints** to prevent duplicate values where required.
- **Cascade rules** to manage related records during applicable operations.
- **Indexes** to support efficient database queries.

The database structure is designed to keep related records consistent and support the platform's interconnected features.

## 🏗️ Project Structure

The project is organized into separate frontend and backend directories.

```text
MicroTeach/
├── front_end/
└── back_end/
    ├── seed.js
    └── ...
```

The backend contains the database setup and seeding script. Additional files and folders are omitted from this simplified structure.

## 🚀 Getting Started

Follow these steps to configure the backend locally.

### Prerequisites

Make sure you have installed:

- [Node.js](https://nodejs.org/)
- [MySQL](https://www.mysql.com/)
- npm
- Git

### 1. Clone the Repository

Replace the placeholder URL below with the actual GitHub repository URL.

```bash
git clone YOUR_REPOSITORY_URL
```

### 2. Navigate to the Backend

```bash
cd MicroTeach/back_end
```

If your cloned repository already opens inside the `MicroTeach` directory, use `cd back_end` instead.

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment Variables

Create a `.env` file in the backend directory and configure the database connection settings required by your application.

Example:

```env
DB_HOST=localhost
DB_USER=your_mysql_username
DB_PASSWORD=your_mysql_password
DB_NAME=microteach_db
```

These variable names are illustrative. Use the exact environment variable names expected by your backend code.

Never commit real database passwords or other secrets to GitHub.

### 5. Create and Initialize the Database

Ensure that MySQL is running and that the database setup script has the permissions it needs to initialize `microteach_db`.

Inspect `seed.js` to understand its setup and seeding behavior before executing it.

The script supports the following modes:

```bash
node seed.js
node seed.js --force
node seed.js --fresh
```

Review the script before using `--force` or `--fresh`, as these options may modify or reset existing database data depending on their implementation.

### 6. Run the Backend

Check the backend's `package.json` for the available scripts and start command. Run the appropriate command after completing the database configuration.

## 🔒 Security Considerations

- Passwords are handled using bcrypt-based hashing.
- Database credentials should be stored in environment variables.
- Database relationships and constraints help maintain data integrity.
- Sensitive configuration files should be excluded from version control.
- Database access should be restricted according to the application's requirements.

## 🎯 Project Objectives

- Design and implement a relational database for an academic platform.
- Establish relationships between multiple database entities.
- Apply primary keys, foreign keys, constraints, and indexes.
- Integrate a Node.js backend with MySQL.
- Manage structured data for users, tutoring, sessions, and communication.
- Practice database initialization and seeding.
- Develop a foundation for a practical academic peer tutoring system.

## 🔮 Future Improvements

Potential enhancements include:

- Advanced search and filtering for tutors and tutoring posts.
- Improved session scheduling and booking workflows.
- Enhanced notifications and messaging.
- More comprehensive administrative reporting.
- Additional database performance monitoring.
- Automated testing and stronger access-control validation.

These are potential improvements rather than claims about existing functionality.

## 👨‍💻 Development Team

**Project:** MicroTeach  
**Course:** Database Management Systems (DBMS)

Add the names of the project contributors and their respective roles here.

## 📄 License

No specific open-source license is declared in this README. Add a license file if the project is intended to be distributed under particular licensing terms.

---

<p align="center">
  <b>MicroTeach — Connecting Learners Through Peer Tutoring 🎓</b>
</p>
