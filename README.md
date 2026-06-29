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

# Healthcare Connector API Endpoints

## Authentication APIs

POST /api/v1/auth/login

---

## Provider APIs

POST /api/v1/providers

GET /api/v1/providers

GET /api/v1/providers/{id}

---

## Payer APIs

POST /api/v1/payers

GET /api/v1/payers

GET /api/v1/payers/{id}

---

## Patient APIs

POST /api/v1/patients

GET /api/v1/patients

GET /api/v1/patients/{id}

---

## Authorization APIs

POST /api/v1/authorizations

GET /api/v1/authorizations

GET /api/v1/authorizations/{id}

PUT /api/v1/authorizations/{id}/review

PUT /api/v1/authorizations/{id}/approve

PUT /api/v1/authorizations/{id}/reject

PUT /api/v1/authorizations/{id}/clarification-request

PUT /api/v1/authorizations/{id}/clarification-response

---

## Communication APIs

POST /api/v1/communications

GET /api/v1/communications/{authorizationId}

---

## Notification APIs

GET /api/v1/notifications

---

# Authorization Workflow

Provider Creates Authorization Request

↓

SUBMITTED

↓

UNDER_REVIEW

↓

APPROVED / REJECTED

---

# Security

JWT Authentication

Role-Based Access Control

Roles:

ROLE_ADMIN

ROLE_PROVIDER

ROLE_PAYER

---

# Database Tables

users

roles

user_roles

providers

payers

patients

authorization_requests

communications

notifications


## Author

Sourabh

Healthcare Connector UI developed using Angular and Spring Boot following enterprise application architecture and healthcare authorization workflows.
