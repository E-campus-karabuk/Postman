# Student Automation System - Postman

## Overview

This repository contains the Postman documentation for the Student Automation System. This system is a senior project developed by a team of four Computer Engineering students at Karabuk University. The Postman collection provides a comprehensive set of API endpoints used by the web and mobile applications, offering a detailed guide for developers to interact with the backend services.

## Team Members

- **Mohamad ZUBI** - [GitHub](https://github.com/MOHAMAD-ZUBI)
- **Muhannad SALKINI** - [GitHub](https://github.com/muhannadsalkini)
- **Nisreen BOUTA** - [GitHub](https://github.com/nisreenbouta)
- **Roula KOURANI** - [GitHub](https://github.com/R-Kourani)

## Features

### API Documentation

The Postman collection includes detailed documentation for all the API endpoints, categorized by their respective modules. This includes request methods, parameters, request bodies, and example responses. The following modules are covered:

- **Authentication**
- **Students**
- **Lecturers**
- **Admins**
- **Chatbot**
- **Courses**
- **Departments**
- **Faculties**
- **Reports**
- **Requests**
- **Senior Groups**

### Usage

This Postman collection is designed to facilitate testing and development by providing pre-configured requests for each endpoint. Developers can easily import the collection into Postman and begin interacting with the APIs immediately.

## Getting Started

### Prerequisites

- [Postman](https://www.postman.com/downloads/) installed on your machine.

### Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/E-campus-karabuk/Postman.git
   cd Postman
   ```

2. **Import the Collection:**
   - Open Postman.
   - Click on `Import` in the top-left corner.
   - Select the file from the cloned repository.
   - The collection will be imported into your Postman workspace.

3. **Environment Setup:**


### Running Requests

1. **Select the Environment:**
   - Ensure the imported environment is selected in the environment dropdown in the top-right corner of Postman.

2. **Navigate the Collection:**
   - The collection is organized by modules, each containing relevant API endpoints.
   - Expand the collection to view and select individual requests.

3. **Send Requests:**
   - Select a request and click `Send` to execute it.
   - Review the response details returned by the API.

## API Endpoints

The Postman collection covers the following API endpoints, categorized by modules:

- **Authentication:**
  - `GET /api/auth` - Get all users (Admin only)
  - `GET /api/auth/current` - Get current user
  - `POST /api/auth/register` - Register a new user
  - `POST /api/auth/login` - Login a user
  - `GET /api/auth/delete/:id` - Delete a user (Admin only)
  - `PATCH /api/auth/addRole/:id` - Add role to a user (Admin only)
  - `PATCH /api/auth/deleteRole/:id` - Remove role from a user (Admin only)

- **Students:**
  - `GET /api/student/current` - Get current student information
  - `POST /api/student/create` - Create a new student

- **Lecturers:**
  - `GET /api/academician/current` - Get current academician information
  - `POST /api/academician/create` - Create a new academician
  - `GET /api/academician/:id` - Get academician by ID

- **Admins:**
  - `GET /api/admin/getAdmin` - Get admin information
  - `POST /api/admin/create` - Create a new admin

- **Chatbot:**
  - `POST /api/bot/test` - Test chatbot
  - `POST /api/bot/newChat` - Send a new chat message

- **Courses:**
  - `GET /api/course/list` - Get all courses
  - `POST /api/course/uploadNote` - Upload a course note
  - `GET /api/course/:id` - Get course by ID
  - `GET /api/course/notes/:id` - Get course notes by course ID
  - `DELETE /api/course/notes/remove/:id` - Delete a course note by ID
  - `GET /api/course/list/mine` - Get my courses
  - `POST /api/course/create` - Create a new course
  - `PUT /api/course/update/:id` - Update course by ID
  - `DELETE /api/course/delete/:id` - Delete course by ID

- **Departments:**
  - `GET /api/department/list` - Get all departments
  - `GET /api/department/userDepartment` - Get department by user (Authenticated)
  - `GET /api/department/:id` - Get department by ID
  - `POST /api/department/addWorker/:id` - Add worker to department by ID
  - `DELETE /api/department/deleteWorker/:id` - Delete worker from department by ID
  - `POST /api/department/addCorse/:id` - Add course to department by ID
  - `DELETE /api/department/deleteCorse/:id` - Delete course from department by ID
  - `POST /api/department/create` - Create a new department
  - `PUT /api/department/update/:id` - Update department by ID
  - `DELETE /api/department/delete/:id` - Delete department by ID

- **Faculties:**
  - `GET /api/faculty/list` - Get all faculties
  - `GET /api/faculty/:id` - Get faculty by ID
  - `POST /api/faculty/create` - Create a new faculty
  - `PUT /api/faculty/update/:id` - Update faculty by ID
  - `DELETE /api/faculty/delete/:id` - Delete faculty by ID

- **Reports:**
  - `POST /api/report/create` - Create a new report
  - `DELETE /api/report/remove/:id` - Delete a report by ID

- **Requests:**
  - `POST /api/request/create` - Create a new student request
  - `GET /api/request` - Get all student requests
  - `GET /api/request/:id` - Get student request by ID
  - `PUT /api/request/:id` - Update student request by ID
  - `DELETE /api/request/:id` - Delete student request by ID
  - `GET /api/request/single/lecturer/:id` - Get single request for lecturer by ID (Authenticated)
  - `GET /api/request/lecturer` - Get requests for lecturer (Authenticated)
  - `PUT /api/request/reply/:id` - Reply to request (Authenticated)
  - `GET /api/request/student` - Get requests for student (Authenticated)
  - `GET /api/request/single/student/:id` - Get single request for student by ID (Authenticated)
  - `GET /api/request/student/lecturers` - Get lecturers for department (Authenticated)

- **Senior Groups:**
  - `GET /api/senior/lecturer/list` - Get senior groups for lecturer (Authenticated)
  - `GET /api/senior/studentGroup` - Get senior group for student (Authenticated)
  - `GET /api/senior/lecturer/students` - Get lecturer's students (Authenticated)
  - `GET /api/senior/files/:id` - Get group reports by ID
  - `POST /api/senior/addStudent/:groupId` - Add student to group by group ID
  - `DELETE /api/senior/removeStudent/:groupId` - Remove student from group by group ID
  - `GET /api/senior/:id` - Get senior group by ID
  - `POST /api/senior/create` - Create a new senior group
  - `PUT /api/senior/update/:id` - Update senior group by ID
  - `DELETE /api/senior/:id` - Delete senior group by ID

## Contributing

If you would like to contribute to this project, please reach out to us via GitHub.

## License

This project is licensed under the Tubitak License.

## Acknowledgments

We appreciate all the guidance and support provided by our professors and peers throughout the development of this project. Feel free to contact the project maintainers with any questions or feedback.
