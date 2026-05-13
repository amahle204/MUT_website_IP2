# MUT ICT Department Website

> Internet Programming 2 Assessment  
> Submission Date: 13 May 2026

---

# Table of Contents

- [Group Members](#group-members)
- [Project Overview](#project-overview)
- [System Features](#system-features)
- [Technologies Used](#technologies-used)
- [System Architecture](#system-architecture)
- [API Routes](#api-routes)
- [Middleware Implementation](#middleware-implementation)
- [UXD Improvements](#uxd-improvements)
- [Frontend Interactivity](#frontend-interactivity)
- [Database Design](#database-design)
- [CRUD Operations](#crud-operations)
- [AI / Smart Functionality](#ai--smart-functionality)
- [Setup Instructions](#setup-instructions)
- [Admin Dashboard Access](#admin-dashboard-access)
- [Conclusion](#conclusion)

---

# Group Members

| Name | Student Number |
|------|----------------|
| AN Khomo | 22407383 |
| N Masinga | 22426770 |
| KA Manzini | 22416153 |
| ZT Khanyile | 22320153 |
| J Macuacua | 22329264 |

---

# Project Overview

The MUT ICT Department Website is a modern full-stack web application developed to redesign and improve the ICT Department website at Mangosuthu University of Technology.

This project was developed as part of the Internet Programming 2 assessment and demonstrates the practical implementation of:

- Frontend web development
- Backend integration
- Middleware implementation
- CRUD operations
- Database connectivity
- AI-powered smart functionality

Traditional departmental websites often provide static information with limited interaction and poor user engagement. This project transforms the ICT Department website into a responsive, intelligent, and interactive platform that improves communication between students, staff, and prospective students.

The system focuses on usability, accessibility, responsive design, and smart automation to create a modern digital experience.

---

# System Features

The system contains several features designed for public users, students, and administrators.

## Public Features

| Feature | Description |
|---------|-------------|
| Responsive Homepage | Mobile-friendly homepage with modern layout |
| About ICT Department | Information about the department |
| Staff Directory | Displays department staff members |
| Programme Information | Interactive programme and module details |
| Announcements & Events | Dynamic news loaded from Firebase |
| FAQ Section | AI-powered FAQ support |
| Contact Page | Interactive contact forms and accordions |

---

## Student Features

| Feature | Description |
|---------|-------------|
| Enquiry Submission | Students can submit enquiries |
| Appointment Booking | Students can request appointments |
| Resource Access | Access departmental resources |
| AI Chatbot Support | Instant AI-powered responses |

---

## Admin Dashboard Features

| Feature | Description |
|---------|-------------|
| News Management | Add, edit, and delete announcements |
| FAQ Management | Update FAQ content |
| Enquiry Monitoring | View submitted student enquiries |
| Department Updates | Modify website information |

---

## Smart Features

| Feature | Description |
|---------|-------------|
| Gemini AI Chatbot | AI-powered assistance using Gemini API |
| Smart Search | Dynamic search functionality |
| Automated Support | Automated responses to enquiries |
| Context-Aware Responses | AI limited to MUT ICT information |

---

# Technologies Used

The project combines multiple frontend, backend, database, and AI technologies.

## Frontend Technologies

| Technology | Purpose |
|------------|---------|
| HTML5 | Structure and semantic markup |
| CSS3 | Styling and responsive design |
| JavaScript (ES6) | Interactivity and API integration |
| Bootstrap | Responsive UI components |
| marked.js | Markdown rendering |

---

## Backend Technologies

| Technology | Purpose |
|------------|---------|
| Node.js | JavaScript runtime environment |
| Express.js | Backend routing and API handling |
| CORS | Cross-origin request handling |
| dotenv | Environment variable management |

---

## Database Technologies

| Technology | Purpose |
|------------|---------|
| Firebase Firestore | NoSQL cloud database |
| Firebase Admin SDK | Secure server-side database access |

---

## AI Integration

| Technology | Purpose |
|------------|---------|
| Google Gemini 2.5 Flash API | AI-powered chatbot assistant |

---

## Development & Deployment Tools

| Tool | Purpose |
|------|---------|
| GitHub | Version control |
| Visual Studio Code | Code editor |
| Postman | API testing |
| Netlify | Frontend deployment |

---

# System Architecture

The following diagram demonstrates how the system components communicate with each other.

```text
User Browser (Mobile/Desktop)
            ↓
      HTML / CSS / JS
   (Frontend on Netlify)
            ↓
         Fetch API
            ↓
   Node.js + Express Server
 (Routes + Middleware Layer)
            ↓
     Firebase Firestore
    (News & Event Storage)
            ↓
      Google Gemini API
      (AI Chatbot System)
```

---

# API Routes

| Method | Endpoint | Purpose |
|--------|----------|---------|
| GET | `/api/news` | Retrieve all news articles |
| POST | `/api/news` | Create a news article |
| PUT | `/api/news/:id` | Update a news article |
| DELETE | `/api/news/:id` | Delete a news article |
| POST | `/api/chat` | Send question to AI chatbot |

---

# Middleware Implementation

| Middleware | Purpose |
|------------|---------|
| Request Logger | Logs incoming requests with timestamps |
| Input Validator | Validates news article input |
| Error Handler | Handles server-side errors |
| CORS Middleware | Allows frontend-backend communication |

---

# UXD Improvements

The original ICT Department website was redesigned using modern User Experience Design (UXD) principles.

## Key UX Improvements

- Simplified mobile navigation using a hamburger menu
- Progressive disclosure through accordion sections
- Mobile-first responsive layouts
- Horizontal swipe programme carousel
- Interactive modals for course information
- Consistent colour palette and typography
- Improved readability and accessibility
- Real-time feedback notifications

These improvements create a smoother and more user-friendly browsing experience across desktop and mobile devices.

---

# Frontend Interactivity

JavaScript was used extensively to create dynamic and interactive user experiences.

| Feature | Description |
|---------|-------------|
| Form Validation | Real-time validation with error messages |
| Search Filtering | Dynamic announcement filtering |
| Programme Carousel | Swipeable mobile carousel |
| Modal Popups | Interactive course information windows |
| Accordion Menus | Expandable contact sections |
| Toast Notifications | User feedback messages |
| AI Chatbot | Intelligent FAQ assistant |

---

# Database Design

The system uses Firebase Firestore as its cloud-based NoSQL database.

## Firestore Collection Structure

### Collection: `news_events`

| Field | Type | Description |
|------|------|-------------|
| title | string | News/article title |
| date | string | Publication date |
| description | string | Article summary/content |
| imageUrl | string | Optional image |
| createdAt | timestamp | Record creation time |

---

# CRUD Operations

All CRUD operations are fully integrated between the frontend, backend, and Firebase database.

| Operation | Method | Endpoint |
|-----------|--------|----------|
| Create | POST | `/api/news` |
| Read | GET | `/api/news` |
| Update | PUT | `/api/news/:id` |
| Delete | DELETE | `/api/news/:id` |

The system allows administrators to manage announcements dynamically without modifying source code manually.

---

# AI / Smart Functionality

The project integrates the Google Gemini 2.5 Flash API to provide intelligent chatbot support.

## How the AI Chatbot Works

1. User enters a question in the chatbot interface
2. Frontend sends request to `/api/chat`
3. Backend communicates with Gemini API
4. Gemini processes the request using predefined instructions
5. AI returns a contextual response
6. Response is displayed in the chat interface

---

## AI System Instructions

```text
"You are an admissions assistant for MUT ICT Department.
Only answer questions about ICT programs,
CAO applications, admission requirements,
and departmental contact information.
If asked anything else, politely say
you cannot answer that question."
```

---

## Benefits of AI Integration

- Provides 24/7 student support
- Reduces repetitive staff enquiries
- Improves website engagement
- Enhances accessibility to information
- Creates a smarter digital platform

---

# Setup Instructions

The following steps explain how to install and run the project locally.

## Prerequisites

Before installation, ensure the following are available:

- Node.js (v20 or higher)
- npm (v10 or higher)
- Firebase account
- Google AI Studio account

---

## Installation Process

### 1. Clone the Repository

```bash
git clone [your-repository-link]
cd ict-department-website
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Create Environment Variables

Create a `.env` file in the root directory.

```env
PORT=3000
GEMINI_API_KEY=your_gemini_api_key_here
FIREBASE_PROJECT_ID=your_firebase_project_id
FIREBASE_PRIVATE_KEY=your_private_key_here
FIREBASE_CLIENT_EMAIL=your_client_email_here
ADMIN_PASSWORD=your_admin_password_here
```

---

# Firebase Setup

1. Create a Firebase project
2. Enable Firestore Database
3. Generate a Firebase service account key
4. Copy Firebase credentials into the `.env` file

---

# Google Gemini API Setup

1. Open Google AI Studio
2. Generate a Gemini API key
3. Add the API key to the `.env` file

---

# Running the Application

## Start the Server

```bash
npm start
```

## Development Mode

```bash
npm run dev
```

## Open in Browser

```text
http://localhost:3000
```

---

# Admin Dashboard Access

Administrators can manage website content through the admin dashboard.

## Steps to Access

1. Navigate to:

```text
/admin.html
```

2. Enter the admin password configured in the `.env` file

3. Access dashboard functionality:
   - Add announcements
   - Edit news
   - Delete content
   - Manage FAQs

---

# Conclusion

The MUT ICT Department Website successfully demonstrates the integration of modern web technologies into a single intelligent full-stack application.

The project combines:

- Responsive frontend design
- Backend API development
- Middleware processing
- Firebase database integration
- CRUD functionality
- AI-powered chatbot support

The redesigned system improves usability, accessibility, interaction, and efficiency while providing students and staff with a smarter and more engaging digital platform.
