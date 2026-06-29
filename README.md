# Healthcare Connector UI

## Project Overview

Healthcare Connector is a healthcare authorization management platform that enables Providers, Payers, and Administrators to manage patient authorization requests efficiently.

The application is built using Angular 22 and integrates with Spring Boot REST APIs secured using JWT Authentication.

---

## Technology Stack

### Frontend

* Angular 22
* TypeScript
* Bootstrap 5
* Bootstrap Icons
* Angular Router
* HttpClient

### Backend

* Spring Boot
* Spring Security
* JWT Authentication
* REST APIs
* MySQL

---

## Features Implemented

### Authentication Module

* User Login
* JWT Token Authentication
* Route Protection using Auth Guard
* Logout Functionality

---

### Dashboard Module

* Dashboard Landing Page
* Statistics Overview
* Navigation to all modules

---

### Provider Management

* Create Provider
* View Provider List
* Provider Details Display

---

### Payer Management

* Create Payer
* View Payer List
* Payer Information Management

---

### Patient Management

* Create Patient
* View Patient List
* Patient Information Management

---

### Authorization Management

#### Create Authorization Request

* Select Provider
* Select Payer
* Select Patient
* Enter Diagnosis
* Enter Procedure Code
* Enter Requested Amount

#### Authorization Workflow

* Submit Authorization
* Review Authorization
* Approve Authorization
* Reject Authorization

#### Authorization Tracking

* Request Number Generation
* Status Tracking
* Rejection Reason Handling

---

### Communication Module

* Add Comments
* View Authorization Communications
* Provider and Payer Interaction

---

### Notification Module

* View Notifications
* Notification Status Tracking
* Authorization Event Notifications

---

## Authorization Workflow

Provider creates Authorization Request

```text
SUBMITTED
      ↓
UNDER_REVIEW
      ↓
 ┌─────────────┬─────────────┐
 ↓             ↓
APPROVED    REJECTED
```

---

## Application Modules

```text
Login
   ↓
Dashboard
   ↓
Provider Management
   ↓
Payer Management
   ↓
Patient Management
   ↓
Authorization Management
   ↓
Communication Center
   ↓
Notifications
```

---

## Security Features

* JWT Based Authentication
* Protected Routes
* Role Based Access Control
* Secure API Communication

---

## Future Enhancements

* Authorization Analytics Dashboard
* AI Assisted Authorization Review
* Advanced Search and Filters
* Audit Logging
* Report Generation
* Email Notifications

---

## Author

Sourabh

Healthcare Connector UI developed using Angular and Spring Boot following enterprise application architecture and healthcare authorization workflows.
