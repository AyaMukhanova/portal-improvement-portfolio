# To-Be System Architecture

## Purpose
This document explains the high-level structure of the redesigned student portal with AI assistant. It shows the main parts of the system, how they connect, and where Odoo fits.

This is a conceptual architecture, not a low-level technical design.

## Main Users
The main users of this system are students.

The portal is designed for students to access schedules, services, and support. Internal staff may use the backend workflow side, but they are not the main users of this version.

## Main Components

### 1. Student Portal Interface
This is the front-end portal used by students. It allows them to:

- log in
- access schedules and resources
- find services
- submit requests
- interact with the AI assistant

### 2. AI Assistant
The AI assistant is built into the portal. It helps students:

- find information faster
- answer common questions
- understand where to go
- complete tasks more easily
- move to the right service or request flow

### 3. Odoo
Odoo is used on the backend to support structured workflows. In this system, Odoo can be used for:

- request tracking
- workflow routing
- service management
- status updates
- admin review

### 4. Data Layer
The data layer stores system records such as:

- student requests
- request status
- interaction history
- service records

### 5. Notification Service
This part sends messages such as:

- confirmations
- reminders
- status updates
- resolution notices

### 6. External Systems
The portal may connect to other university systems such as:

- authentication
- academic records
- schedule systems
- other student service systems

## High-Level Flow
1. A student logs into the portal.
2. The student navigates directly or uses the AI assistant.
3. The AI assistant gives guidance or answers a question.
4. If the issue needs formal handling, the request is sent into Odoo.
5. Odoo manages the workflow and status.
6. The data layer stores records.
7. Notifications keep the student updated.

## Where Odoo Is Used
Odoo is used in the backend service layer. It supports structured request handling and internal workflows.

It helps the system:

- receive requests from the portal
- route them correctly
- track progress
- support staff handling

## System Boundary
The system can be viewed in three parts:

### User-facing layer
- student portal
- AI assistant

### Internal processing layer
- Odoo
- data layer
- notification service

### External integration layer
- university systems such as login and records

## Summary
The redesigned portal gives students a simpler front-end experience. The AI assistant helps with guidance and navigation. Odoo supports the backend workflow and service process.
