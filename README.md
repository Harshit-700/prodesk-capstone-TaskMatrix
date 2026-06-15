# TaskMatrix

## Enterprise Agile Project Management Platform

### Project OvervieW

TaskMatrix is a modern Agile Project Management platform inspired by industry-leading solutions such as Jira and Asana. The platform is designed to help software development teams efficiently manage projects, organize sprints, assign tasks, monitor deadlines, and collaborate in real time.

The primary objective of TaskMatrix is to provide a centralized workspace where project managers, developers, and administrators can streamline their workflow using Agile methodologies. The system focuses on task visibility, sprint planning, team collaboration, and project tracking while maintaining a scalable and maintainable architecture.

---

# Track

**Fullstack Development**

[Screenshot](https://github.com/Harshit-700/prodesk-capstone-TaskMatrix/blob/8cad65df3219a614c2d149e64f2d4875cf549a71/erd.png).
---

# Problem Statement

Software teams often struggle with fragmented project tracking systems, communication gaps, and inefficient task management processes. Existing enterprise tools can be overly complex or costly for small and medium-sized teams.

TaskMatrix aims to solve these challenges by providing:

* Centralized project management
* Sprint planning and execution
* Task lifecycle tracking
* Team collaboration workflows
* Real-time activity monitoring
* Role-based access management

---

# Technology Stack

## Frontend

* React.js
* Zustand
* Tailwind CSS
* React Router
* Socket.io Client

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT Authentication
* Socket.io

## Deployment

* Vercel (Frontend)
* Render (Backend)
* MongoDB Atlas (Database)

---

# Core Features (Priority Order)

## P0 - Core MVP

### Authentication & Authorization

* User Registration
* User Login
* JWT Authentication
* Protected Routes
* Role-Based Access Control

### Project Management

* Create Projects
* Update Projects
* Archive Projects
* Team Member Assignment

### Task Management

* Create Tasks
* Update Tasks
* Delete Tasks
* Assign Tasks
* Priority Management
* Due Date Tracking

---

## P1 - Agile Workflow

### Sprint Management

* Create Sprint
* Start Sprint
* Complete Sprint
* Sprint Goal Tracking

### Kanban Board

* Backlog
* Todo
* In Progress
* Review
* Done

### Drag-and-Drop Functionality

* Task Reordering
* Status Updates
* Optimistic UI Updates

---

## P2 - Advanced Features

### Real-Time Activity Feed

* Live Task Updates
* Sprint Events
* Team Activity Tracking

### Analytics Dashboard

* Sprint Progress
* Task Completion Metrics
* Productivity Overview

---

# User Roles

## Administrator

Responsible for platform governance and user management.

### Permissions

* Manage Users
* Manage Projects
* View Analytics
* Configure Roles

---

## Project Manager

Responsible for project planning and sprint execution.

### Permissions

* Create Projects
* Manage Sprints
* Assign Tasks
* Monitor Progress

---

## Developer

Responsible for task execution and collaboration.

### Permissions

* View Assigned Tasks
* Update Task Status
* Participate in Sprint Workflows

---

# Database Architecture

The platform follows a collection-based MongoDB architecture.

## Collections

### Users

Stores user information, authentication data, and role assignments.

### Projects

Stores project metadata, ownership details, and team members.

### Tasks

Stores task information, status, priority, assignments, and deadlines.

### Sprints

Stores sprint schedules, goals, and execution data.

### ActivityLogs

Stores project history and user activity records.

---

# System Architecture

## Entity Relationship Diagram (ERD)

The ERD illustrates the relationships between Users, Projects, Tasks, Sprints, and Activity Logs.

![ERD Diagram](https://github.com/Harshit-700/prodesk-capstone-TaskMatrix/blob/2c3d33e9342ec3c1406c87a4156ee5a00857d3e4/Screenshot%20(445).png)

---

## Frontend State Architecture (Zustand)

The application uses Zustand for centralized state management.

### Stores

#### authStore

* User Session
* Access Token
* Authentication State

#### projectStore

* Projects
* Active Project
* Team Members

#### taskStore

* Tasks
* Kanban Columns
* Drag-and-Drop State

#### sprintStore

* Active Sprint
* Sprint Metrics

#### activityStore

* Activity Feed
* Real-Time Events

#### uiStore

* Sidebar State
* Modal State
* Filters
* Notifications

![State Tree Diagram]![Screenshot](https://github.com/Harshit-700/prodesk-capstone-TaskMatrix/blob/75c2141d55e9d6104b6e93d023a655bd231f78f2/Screenshot%20(446).png)

---

# API Architecture

## Authentication

POST /api/auth/register

POST /api/auth/login

POST /api/auth/refresh

POST /api/auth/logout

---

## Projects

GET /api/projects

POST /api/projects

PUT /api/projects/:id

DELETE /api/projects/:id

---

## Tasks

GET /api/projects/:id/tasks

POST /api/projects/:id/tasks

PUT /api/tasks/:id

PATCH /api/tasks/:id/status

DELETE /api/tasks/:id

---

## Sprints

GET /api/projects/:id/sprints

POST /api/projects/:id/sprints

PATCH /api/sprints/:id/start

PATCH /api/sprints/:id/complete

---

## Activity Logs

GET /api/projects/:id/activity-logs

GET /api/activity-logs

---

# UI / UX Wireframes

The application UI has been designed and prototyped before implementation.

## Core Screens

### Authentication Screen

* Login
* Registration

### Main Dashboard

* Project Overview
* Sprint Metrics
* Activity Feed

### Kanban Board

* Drag-and-Drop Tasks
* Status Management
* Filters

### Task Details View

* Task Information
* Assignee Details
* Activity Timeline

### Figma Design File

[https://www.figma.com/design/FxZOiski44thaAPVrnQlvY/Untitled?node-id=0-1&p=f&t=pZQChwt74evSxZ4G-0001]

---

# Development Roadmap

## Sprint 13

Planning & Architecture Design

## Sprint 14

Authentication & Project Management MVP

## Sprint 15

Task Management & Sprint Workflow

## Sprint 16

Real-Time Features & UX Enhancements

## Sprint 17

Deployment, Testing & Final Presentation

---

# Future Enhancements

* Team Chat
* Comments & Mentions
* File Attachments
* Email Notifications
* AI Sprint Planning
* AI Task Prioritization
* Team Analytics Dashboard

---

# Author

Harshit
Capstone Project
