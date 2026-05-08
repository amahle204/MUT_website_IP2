| Name | Student Number |
|---|---|
| AN Khomo | 22407383 |
| N Masinga | 22426770 |
| KA Manzini | 22416153 |
| ZT Khanyile | 22320153 |
| J Macuacua | 22329264 |


# MUT ICT DEPARTMENT WEBSITE

This is modern full-stack web application designed to improve the ICT Department website by making it interactive, user-centred, database-driven and intelligent. The system was developed as part of the Internet Programming 2 assessment and demonstrates frontend development, backend integration, middleware implementation, CRUD operations and smart functionality.

## Project Overview
Traditional departmental websites often provide static information with limited interaction and poor user engagement. This project redesigns the ICT Department website into a smart and responsive web application that allows students, staff and prospective students to interact with the system more effectively.
The application includes:
- Responsive modern user interface
- Dynamic departmental content
- Student enquiry system
- Appointment booking
- Announcements and events management
- FAQ support
- AI-powered smart assistant/chatbot
- Backend API integration
- Database connectivity
- Middleware validation and error handling

## Objectives
The main objectives of the project are to:

- Improve user experience and navigation
- Create an interactive departmental platform
- Integrate frontend and backend technologies
- Store and retrieve data dynamically
- Demonstrate CRUD operations
- Implement middleware in Express.js
- Introduce smart/AI functionality
- Build a scalable and maintainable web application

## Technologies Used


### Frontend

- HTML5
- CSS3
- JavaScript
- Bootstrap

### Backend:

- Node.js
- Express.js
- Database
- MySQL
  
### Other Tools:

- GitHub
- Visual Studio Code
- Postman
- XAMPP / MySQL Workbench

## System Features

### Public Features

- Homepage
- About ICT Department page
- Staff directory
- Course and module information
- Announcements and events
- FAQ section
- Contact page

### Student Features

- Submit enquiries
- Book appointments
- Access resources
- Receive feedback notifications
  
### Admin Features

- Add/edit/delete announcements
- Manage FAQs
- View enquiries
- Manage events and departmental information
  
### Smart Features

- AI-powered FAQ chatbot
- Smart search functionality
- Automated enquiry assistance

## User Experience (UXD) Improvements

We analysed and redesigned the existing ICT Department website using UXD principles.

These improvements include:

- Responsive layout for mobile and desktop
- Improved navigation structure
- Consistent colour palette and typography
- Better content organization
- Faster access to important information
- Interactive feedback and validation
- Improved accessibility and readability

## Frontend Interactivity

We used JavaScript to improve interaction and usability.

The Interactive features are as follows:

- Form validation
- Search filtering
- Dynamic content updates
- Dropdown menus
- Modal popups
- Feedback messages
- FAQ accordion
- Chatbot interaction

## Backend Development

The backend server was developed using Node.js and Express.js.

Backend responsibilities:

- Handle client requests
- Process form submissions
- Connect to database
- Perform CRUD operations
- Manage routes and middleware
- Return server responses

These features improve user engagement and reduce usability issues.

### Example Routes

These are the GET routes

GET /announcements
GET /staff
GET /faq

These are the POST routes:

POST /enquiries
POST /appointments

These are the PUT routes:

PUT /announcements/:id

These are the DELETE routes:

DELETE /announcements/:id


## Database Design

The system uses a MySQL relational database.

### Main Tables

- announcements
- staff
- faq
- enquiries
- appointments
- events

### Database Functionality

- Store enquiries
- Retrieve announcements
- Manage appointments
- Update departmental information
- Support chatbot FAQ responses

CRUD operations are fully implemented between the frontend, backend and database.

## Middleware Implementation

Middleware was implemented to improve security, validation and error handling.

Middleware used:

- Request logging middleware
- Validation middleware
- Error handling middleware
- Route protection middleware

Purpose of Middleware:

- Validate user input
- Prevent invalid requests
- Log incoming requests
- Handle server errors properly
- Improve application structure

## AI / Smart Functionality

The system includes an AI-powered FAQ chatbot.

This is how it works:

- User enters a question
- System checks keywords/questions
- Matching response is retrieved from database
- User receives automated assistance
  
Benefits of this function are:

- Provides instant support
- Reduces repetitive enquiries
- Improves user experience
- Makes the website more interactive and intelligent
