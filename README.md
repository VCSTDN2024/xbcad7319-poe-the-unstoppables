 # We deployed our web app for you! Access it at:
 # https://XBCADMVCWebApp.azurewebsites.net
 
 # Documentation:

# Comprehensive Documentation for University Query System

## Overview
This is a comprehensive Cross-Platform University Query System, accessible on both Web and Android platforms. The application streamlines the process of student queries, facilitating seamless communication between students and staff while ensuring query resolution in a user-friendly manner.

---

## How to Use the Application

### Web Application

#### Registration
Upon landing on the home page, users can choose either the **Student Registration** or **Staff Registration** option to create an account. This initial step allows users to gain access to features relevant to their role within the system.

#### Login
After completing the registration process, users can proceed by clicking on the **Login** button. Here, they will enter their credentials to access the system. The application dynamically routes them to their appropriate dashboard:
- **Student Dashboard**: Tailored to student-specific functionalities.
- **Staff Dashboard**: Includes tools and features specific to staff operations.

---

### Student Dashboard Features

#### Knowledge Base and FAQ
Students can access a rich **Knowledge Base** and browse through an extensive list of **Frequently Asked Questions (FAQ)**. This feature enables them to find solutions to common queries or learn more about university policies, procedures, and services.

#### Knowledge Base Search Functionality
A powerful **Search Bar** is integrated at the top of the Knowledge Base and FAQ section. This search tool allows students to quickly locate specific information by entering keywords or phrases, providing instant and accurate results.

#### Query Submission
Students have the ability to submit detailed queries directly through the **Query Submission** feature. This involves:
- Selecting the **Query Type**.
- Providing a **Title** and a comprehensive **Description** of their issue.
- Optionally attaching documents to support their query.
- Clicking the **Submit Query** button to forward their concern to the relevant department or lecturer.

#### Query Status Tracking
The **Query Status Tracking** page provides students with an organized view of all their submitted queries, including:
- **Query Type**
- **Title**
- **Description**
- **Submission Date**
- **Status** (e.g., Pending, In Progress, Resolved)

This feature ensures students can monitor the progress of their concerns effortlessly.

---

### Staff Dashboard Features

#### Routed Department Queries
The **Department Queries** section enables staff members to view all queries routed to their department. For each query, staff can see:
- **Query ID**
- **Title**
- **Description**
- **Attached Documents**
- **Status**

Additionally, they have tools to update the query status to either **In Progress** or **Resolved**, streamlining resolution efforts.

#### Analytics and Reporting
The **Analytics and Reporting** page allows staff to analyze trends and performance, such as:
- The most common **Query Titles**.
- A breakdown of **Query Types**.
- The **Departments** submitting the most queries.
- A detailed view of **Submission Dates** and **Resolved Dates** to assess the resolution rate.

#### Service Compliance Status
Staff can monitor **Service Compliance** directly from the Analytics and Reporting section. This includes:
- The number of queries resolved within the compliance target of **48 hours**.
- Identification of **non-compliant queries** to improve service quality.

---

### Android Application

#### Registration and Login
On the Android application, users can register by clicking the **Sign Up** button. Once registered, they can log in using their credentials to access their personalized dashboard.

#### Student Dashboard Features
The Android app mirrors the key features of the web application for students:
- **Knowledge Base and FAQ**: Providing easy access to critical information.
- **Query Submission**: Allowing students to submit detailed queries and attach supporting documents.
- **Status Tracking**: Offering real-time updates on query statuses.

---

## Documented Data Structures and Algorithms

### FAQ and Knowledge Base Search

#### Algorithm
- Loops through the FAQ and Knowledge Base lists.
- Compares the search query with list items using string matching.
- **Time Complexity**: O(n), where n is the number of items.

#### Data Structures
- **Lists**: Used for storing FAQ and Knowledge Base items.
- **Strings**: Utilized for comparing search inputs with stored data.

---

## Documented Classes for Data Transfer
The application uses specific controllers for managing data transfer, including:
- **StudentController**: Handles all student-related operations.
- **StaffController**: Manages staff-related functionality.
- **DashboardController**: Deals with dashboard data such as user-specific details.

---

## Architectural and Design Patterns
The system implements the **Model-View-Controller (MVC)** architecture, a widely recognized design standard in software development. This structure ensures a clear separation of concerns:
- **Model**: Manages data and business logic.
- **View**: Handles the user interface.
- **Controller**: Connects the model and view to facilitate interaction.

---

## Communication Between Frontend and Backend
The application uses **Service Classes** to establish secure and efficient communication between the frontend interface and the backend Firebase database. These services:
- Ensure seamless data exchange.
- Provide synchronization between the web and mobile apps.

---

## Data Storage
The application utilizes **Firebase Realtime Database**, a cloud-based storage solution that supports real-time data synchronization across platforms. This enables users to access the latest information regardless of the device they use.

---

## Security Considerations and Mitigations

### Potential Threats:
1. Potential threat actors include students creating accounts as lecturers when they are not. To mitigate this, staff registration is disabled on the application. This mitigation has already been successfully implemented on the Android app. For the purpose of the demo, staff registration remains available on the web app so users can create a staff account and log in to easily view its functionality.

2. Another potential threat is the use of easily crackable passwords. To combat this, password requirements have been implemented to ensure stronger and more secure passwords.


---

## Demonstration of Running Costs
With Firebase as the backend, the Spark plan allows free database access. Given the application's current low data needs, it is unlikely that an upgrade to a paid account will be necessary in the foreseeable future, even when accounting for potential growth.

---

## Change Management
Universities should adopt this application because it streamlines the process of handling student queries, consolidating it into one platform. The system is accessible via web or mobile, enabling organizations to offer more ways for students to seek help, ultimately fostering a more supportive and accessible environment for students.

---

## Adoption Strategy
1. **Email Campaigns:** We will gather email addresses of principals or relevant stakeholders from organizational websites and send emails about this opportunity to revolutionize query management. The emails will include a demo video and a link to book a call if interested.

2. **Phone Outreach:** We will call these organizations directly to ensure we speak to someone who can provide information on how to move forward or direct us to the right contact person.

3. **On-Site Demonstrations:** We will visit the receptions of organizations to showcase the product and demonstrate its value in person, ensuring it gets into the hands of their students.

---

## Installation Instructions
1. Download the repository zip files.
2. Unzip the files to access the project folders.
3. Open:
   - **XBCAD Application** folder in Android Studio for the Android app.
   - **XBCAD_MVC_WebApplication** folder in Visual Studio for the web application.
