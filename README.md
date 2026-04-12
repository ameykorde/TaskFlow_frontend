# TaskFlow

**TaskFlow** is a cloud-ready task management platform designed to help teams organize projects, manage tasks, and track work progress using a Kanban-style workflow.

The system enables collaborative project management where users can create projects, invite team members, assign tasks, and monitor progress through clearly defined workflow stages.

TaskFlow is built as a full-stack application and designed with scalability and modern DevOps practices in mind.

---

# Overview

Modern software teams require efficient ways to organize work, collaborate across members, and track project progress. TaskFlow provides a structured environment where projects and tasks can be managed visually using a Kanban board.

Each project acts as an isolated workspace where invited members collaborate to complete tasks. Tasks move across workflow stages to represent their progress in the development lifecycle.

---

# Key Features

* Project creation and management
* Project-level role-based access control
* Invitation-based project collaboration
* Task creation and assignment
* Kanban-style workflow management
* In-application notification system
* Task lifecycle tracking

---

# Technology Stack

Frontend
React

Backend
Java (Spring Boot)

Database
PostgreSQL

---

# System Architecture

TaskFlow follows a standard three-layer architecture:

**Client Layer**
A React-based web interface that allows users to interact with projects, tasks, and notifications.

**Application Layer**
A Spring Boot backend that manages business logic, authentication, project management, and task operations through REST APIs.

**Data Layer**
A PostgreSQL database responsible for storing user data, projects, memberships, tasks, and notifications.

---

# Core Concepts

## Users

Users represent individuals who interact with the platform.
Each user is uniquely identified using an email address.

Users may participate in multiple projects.

---

## Projects

A project represents a collaborative workspace where tasks are managed.

Each project contains:

* project members
* tasks
* workflow stages

The user who creates a project automatically becomes the **Project Admin**.

---

## Tasks

Tasks represent individual units of work within a project.

A task typically contains:

* title
* description
* assigned user
* workflow status

Tasks progress through workflow stages during the development lifecycle.

---

# Project Roles

Roles are assigned **per project**, not globally.

This allows a user to have different roles across different projects.

Example

User A
Project Alpha → Admin
Project Beta → Member

Two roles exist within a project.

---

## Project Admin

Project Admins manage the project and control team collaboration.

Responsibilities include:

* creating projects
* editing project details
* renaming projects
* inviting users to join projects
* managing project members
* changing member roles
* creating tasks
* editing tasks
* deleting tasks
* assigning tasks
* managing task workflow

---

## Project Member

Project Members participate in the project and contribute to tasks.

Members can:

* view project boards
* create tasks
* update tasks
* move tasks across workflow stages

Members primarily focus on executing project work.

---

# Invitation-Based Collaboration

Projects use a controlled access model.

Users cannot join projects directly.

Instead, **Project Admins send invitations** to users.

Invitations are delivered through the application's notification system.

Invited users can choose to:

* accept the invitation and join the project
* reject the invitation

Once accepted, the project becomes visible in the user's dashboard.

---

# Kanban Workflow

TaskFlow uses a Kanban-style board to represent task progress.

Tasks move across three workflow stages:

To Do
Task has not started.

In Progress
Task is actively being worked on.

Done
Task has been completed.

This visual workflow provides teams with a clear understanding of project status.

---

# Notification System

The platform includes an in-application notification system that informs users about important project events.

Notifications include:

* project invitations
* task assignments
* role updates

Notifications help maintain awareness of project activity and collaboration events.

---

# Future Enhancements

TaskFlow is designed to support further DevOps integrations and infrastructure automation.

Future enhancements may include:

* containerization using Docker
* CI/CD pipeline integration
* cloud deployment
* infrastructure as code
* monitoring and logging systems

---

# Purpose of the Project

TaskFlow serves as a demonstration platform for building modern cloud-ready applications. The system is structured to showcase collaborative project management, scalable architecture, and readiness for automated deployment environments.

