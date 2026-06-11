# Field360

**Internal Spatial Farm Management Platform**

Field360 is a mobile-first, offline-first farm management platform built to support my own agricultural operations in Kerala. It was created to solve a practical problem: managing thousands of plants where timing, visibility, and consistency directly impact yield.

The platform is actively used to manage Co3 fodder cultivation and tapioca plots, providing a digital representation of the farm, operational task tracking, and financial management in a single application.

---

## The Problem

Managing a large fodder operation is not just about recording data.

With 2,500+ plants under cultivation, important activities such as fertilization, irrigation, maintenance, and harvesting must happen at the right time and in the right location.

Traditional record-keeping methods make it difficult to:

* Track individual plant groups across the farm
* Identify what actions are required today
* Maintain consistent crop management cycles
* Monitor production across recurring harvest periods
* Connect farm operations with financial records

Field360 was built to address these challenges through a spatial, mobile-first approach.

---

## Core Modules

### Dashboard

A centralized overview of farm operations.

Features include:

* Farm activity summaries
* Upcoming operational tasks
* Production insights
* Financial snapshots
* Operational status tracking

---

### Plots

Digital management of farm plots and cultivation zones.

Features include:

* Plot organization
* Crop assignment
* Zone management
* Spatial farm structure

---

### Tasks

Operational task management designed around farm workflows.

Features include:

* Task generation
* Status tracking
* Priority management
* Action visibility across the farm

---

### Finance

Farm-focused financial tracking.

Features include:

* Expense recording
* Income tracking
* Financial summaries
* Farm operation cost visibility

---

## FieldView

FieldView is the primary operational interface of Field360.

Instead of presenting information only as lists or tables, FieldView provides a spatial representation of the farm.

The system highlights areas requiring attention and allows operational activities to be viewed directly within the context of the field layout.

FieldView includes:

### Management Tools

Used to build and manage the farm's digital representation.

Examples include:

* Plot creation
* Layout management
* Spatial organization
* Field structure updates

### Crop Action Tools

Used to surface operational activities that require attention.

When an action is selected, FieldView highlights the relevant areas within the farm layout, helping identify where work needs to be performed.

The farmer performs the work; the application provides visibility into what needs attention and where.

---

## Technology Stack

### Flutter

Cross-platform mobile application framework used to build the entire application.

### Riverpod

Used for application state management.

Riverpod integrates closely with the database layer, allowing the UI to stay synchronized with live data streams without requiring manual refresh logic.

### Drift (SQLite)

Used as the primary persistence layer.

Reasons for choosing Drift:

* Type-safe database access
* Structured relational data modeling
* Code generation
* Strong integration with Flutter
* Cleaner maintenance compared to raw SQLite

### Repository Pattern

Repositories act as a boundary between persistence and presentation layers.

Responsibilities include:

* Consuming DAO results
* Transforming database models
* Exposing UI-friendly models
* Isolating data source implementation details

### Feature-First Architecture

The application is organized around features rather than technical layers.

Each feature owns its:

* Models
* Providers
* Widgets
* Helpers
* Data access logic

This structure improves maintainability as the project grows.

### Offline-First Design

Field360 was designed as an offline-first application from the beginning.

Benefits include:

* Fast local access
* No dependency on network connectivity
* Reduced operational cost
* Local-first reliability

Remote synchronization can be introduced later without restructuring the application.

---

## Project Statistics

As of June 2026:

* 184 Dart files
* 21,000+ lines of code
* 4 major FieldView design iterations
* 2,500+ tracked fodder plants
* Active daily usage

---

## Design Evolution

FieldView evolved through multiple iterations:

1. Initial grid-based prototype
2. Clustered spatial layout
3. Row-based interaction model
4. Current production design

Each iteration was driven by real farm usage and operational feedback.

---

## Screenshots

### Dashboard

*Add screenshot*

### FieldView

*Add screenshot*

### Plot Management

*Add screenshot*

### Finance

*Add screenshot*

---

## Development Status

Field360 is an actively maintained internal platform and continues to evolve as farm requirements grow.

Current areas of development include:

* Rendering system improvements
* Task workflow enhancements
* Additional operational tooling

---

## About

Field360 began on February 26, 2026 as an internal tool built for real agricultural operations.

It continues to serve as both a production system for farm management and a long-term software engineering project focused on building practical, domain-driven solutions using Flutter.
