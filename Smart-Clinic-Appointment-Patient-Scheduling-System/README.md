# Smart Clinic Appointment and Patient Scheduling System

## Project Overview

This project involves building a web-based system that helps clinics manage patient registration, doctor schedules, and appointments in one place. Currently, many clinics rely on phone calls, paper records, and manual appointment books to organize patient visits. This can lead to long waiting times, scheduling conflicts, lost patient information, and confusion between patients, receptionists, and doctors.

The Smart Clinic Appointment and Patient Scheduling System addresses these problems by automating appointment scheduling and managing patient information in a centralized system. Patients can register, request appointments, check their appointment status, and cancel or reschedule appointments. Receptionists can register patients, manage walk-in patients, and book appointments on behalf of patients. Doctors can view their schedules and appointments, while administrators manage doctors, staff, users, and system settings. The system checks doctor availability before confirming appointments to prevent scheduling conflicts.

## Problems Solved

**Appointment conflicts:** Prevents multiple patients from being scheduled with the same doctor at overlapping times.

**Poor patient information management:** Centralizes patient registration and information instead of relying on scattered paper records.

**Long waiting times:** Improves appointment scheduling and organization to reduce unnecessary waiting.

**Poor communication:** Provides a centralized system where patients, receptionists, and doctors can access relevant appointment information and status updates.

**Manual scheduling:** Reduces the effort required to manage doctor availability, appointments, cancellations, and rescheduling.

## Main Goals

**Conflict-free scheduling:** Checks doctor availability before creating or confirming appointments.

**Less paperwork:** Digitizes patient registration, appointment requests, scheduling, and management.

**Patient information management:** Maintains organized patient information and appointment history.

**Improved clinic workflow:** Helps receptionists, doctors, and administrators coordinate their daily activities.

**Appointment tracking:** Allows users to track appointment status, including pending, confirmed, cancelled, and completed appointments.

**Better access control:** Protects patient information and ensures users can access only the information permitted by their roles.

## Users (Actors) and Main Features

The system includes five types of users:

**Patient:** Registers in the system, manages personal information, requests appointments, views appointment status, and cancels or reschedules appointments.

**Receptionist:** Registers patients, handles walk-in patients, books appointments, manages appointment requests, and assists patients with scheduling.

**Doctor:** Views appointment schedules, checks patient appointment information, and manages availability and working schedules.

**Administrator:** Manages system users, doctors, staff, user permissions, and system configurations.

**Clinic Manager:** Oversees clinic operations, monitors appointment activities, manages staff schedules, and reviews reports.

*Note: The project focuses on patient registration, appointment scheduling, doctor and staff management, and clinic workflow. Advanced features such as AI-based diagnosis, online payment processing, pharmacy management, and laboratory systems are excluded to keep the project scope manageable.*

## Course Connection and Tools

**Modeling:** Uses Enterprise Architect for Use Case, Activity, Sequence, and Class diagrams, showing association, aggregation, composition, and inheritance where appropriate for classes such as User, Patient, Doctor, Receptionist, Appointment, Schedule, and Clinic.

**Code Generation:** Generates Java code from the system models using Enterprise Architect.

**Version Control:** Uses Git and GitHub with individual branches, meaningful commits, pull requests, collaboration, and code reviews.

**Testing:** Uses JUnit 4 tests for methods such as checking doctor availability, registering patients, booking appointments, and validating appointment conflicts. Testing includes normal, invalid, and boundary cases.

## Group Members

1. **Mohammed Endris** (ID: 3706/17) — Project Manager
2. **Seblewongel G/michael** (ID: 0568/17)
3. **Ahmed Misbah** (ID: 0852/17)
4. **Redwan Seid** (ID: 1797/17)
5. **Mohammed Seid** (ID: 1691/17)
6. **Umeymah Mohammed** (ID: 0659/17)

**Institution:** Wollo University  
**College:** Kombolcha Institute of Technology  
**Department:** Software Engineering  
**Course:** Software Engineering Tools and Practice (SEng5331)
