# University Enrollment System

A TypeScript application that models university course enrollment. Used for educational purposes during the 2025-2026 school year

**Course:** Advanced JavaScript @ EPITA
**Module:** Domain-Driven Design, Branded Types & Observer Pattern

---

## Overview

This project models the core business logic of a university enrollment system. It manages students, courses, and enrollments while enforcing rules around course capacity, duplicate registrations, student status, withdrawals, and grade completion.

The application runs as a command-line demonstration backed by in-memory repositories.

My task: Build a University Enrollment System from scratch, applying **Domain-Driven Design (DDD)** principles, **TypeScript Branded Types**, and the **Observer Pattern**.

---

## Key Features

- Student and course management
- Enrollment creation and validation
- Course capacity and duplicate-enrollment checks
- Enrollment withdrawal and completion
- Typed domain models and result-based error handling
- Event-driven observers for audit, notifications, and capacity monitoring
- Separation of domain logic, application services, and repositories

## Architecture

The project separates responsibilities into distinct components:

- Domain: Student, Course, and Enrollment models, including business rules and validation.
- Application service: Coordinates enrollment, withdrawal, and completion workflows.
- Repositories: in-memory storage and lookup operations.
- Events and observers: Allow components to react to relevant domain events.
- CLI: Demonstrates normal operations and rejected actions.

## Tech Stack

- TypeScript
- Node.js
- npm
- UUID generation

## Getting Started

**1. Prerequisites** 

- Node.js (use a version supported by the project)
- npm

**2. Installation**

git clone https://github.com/namkhanh-le/university-enrollment-system.git
cd university-enrollment-system
npm install

**3. Run the application**

npm run dev

The CLI demonstrates student and course registration, enrollment attempts, invalid operations, withdrawals, grade completion, and a final summary.

## Design Principles

Domain-driven design: Organizes the application around the business domain.
Type safety: Uses TypeScript to distinguish domain concepts and constrain valid operations.
Encapsulation: Keeps business rules close to the entities and services responsible for enforcing them.
Separation of concerns: Separates application workflows, storage, and event handling.
Observer pattern: Supports reactions to events without coupling every observer directly to the business workflow.

## Limitations

This is a learning project focused on domain modeling and application logic. It currently uses in-memory repositories and a CLI rather than a persistent database or HTTP API.

## Future Improvements

Automated unit and integration tests
Stronger type-checking and validation coverage
Persistent storage
An HTTP API for enrollment operations
Continuous integration to run checks automatically

