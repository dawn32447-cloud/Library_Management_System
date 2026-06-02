# Library Management System SQL Project


## Project Overview

This project demonstrates the implementation of a Library Management System using SQL. It covers the core aspects of relational database design, including table creation with primary and foreign key constraints, data insertion, data manipulation (updates/deletions), and data analysis using advanced SQL queries. 

The dataset models a real-world library operation, tracking branches, employees, members, books issued, and return statuses.

## Database Architecture

The system consists of 6 interrelated tables:
* branch: Details of library branches and their managers.
* employees: Employee profiles, salaries, and branch assignments.
* members: Registered library patrons and their registration dates.
* books: Comprehensive catalog including category, rental price, and availability status.
* issued_status: Log of books checked out by members, handled by specific employees.
* return_status: Records of returned books mapped back to their original issuance.

## File Structure

* 01_Database_schema.sql: Definitive DDL scripts to set up database structures, data types, and primary/foreign key relationships.
* 02_Data_insertion.sql: DML scripts containing realistic dataset rows for comprehensive testing.
* 03_Analytics_tasks.sql: Solutions to 12 production-level business tasks ranging from simple CRUD operations to analytical aggregations using CTAS and Joins.

---

## Key SQL Analytics & Tasks Accomplished


### 1. Data Modification (CRUD)

* Task 1: Added new book acquisitions into the catalog.
* Task 2: Updated stale member profile addresses dynamically.
* Task 3: Executed isolated record deletions on transaction tables.

### 2. Operational Operational Reporting

* Task 4: Filtered and isolated books issued by specific personnel identifiers.
* Task 5: Grouped transaction histories to isolate high-frequency member checkouts using HAVING filters.
* Task 7: Categorized inventory lookups for targeted genres (e.g., *Classic*).
* Task 9: Dynamic time-series filtering to extract members who registered within a rolling 180-day window.

### 3. Business Analytics & Reporting

* Task 6 (CTAS): Generated aggregated summary tables reporting total lookup frequencies per book title.
* Task 8: Calculated gross revenue yield metrics broken down by book category segments.
* Task 10: Implemented complex self-joins to map organizational hierarchies linking employees directly to their respective branch managers.
* Task 11: Created dedicated, isolated high-tier price segments ($> \$7.00$) tables via automated CTAS routines.
* Task 12: Discovered unreturned inventory bottlenecks using structured LEFT JOIN logic assessing null return states.

---

