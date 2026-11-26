# Actors and Use Cases: Smart Clinic Appointment and Patient Scheduling System

Actors are people or external systems that interact with the Smart Clinic Appointment and Patient Scheduling System.

## **Patient**

**Who:** A person who wants to receive medical services and book an appointment with a doctor.

**Note:** Patients can register, log in, and manage their appointments through the system.

**Use cases:** Register, Log In, Update Profile, View Doctors, Search Doctor by Specialty, Check Doctor Availability, Request Appointment, View Appointment Status, Reschedule Appointment, Cancel Appointment, View Appointment History, View Notifications.

## **Receptionist**

**Who:** A clinic employee who handles patient registration, appointment booking, and daily scheduling activities.

**Use cases:** Log In, Register Patient, Search Patient, View Patient Information, Update Patient Information, Book Appointment, Confirm Appointment, Reschedule Appointment, Cancel Appointment, Manage Walk-in Patients, View Doctor Schedule, Update Appointment Status, View Notifications.

## **Doctor**

**Who:** A medical professional who provides consultations and manages their appointment schedule and availability.

**Use cases:** Log In, View My Schedule, View Appointments, View Relevant Patient Information, View Patient Appointment History, Manage Availability, Request Schedule Change, Request Time Off, Mark Appointment Completed, Mark Patient as Missed, View Notifications.

## **Administrator**

**Who:** The person responsible for managing system accounts, roles, doctors, staff, and overall system configuration.

**Use cases:** Log In, Manage Users, Create User Accounts, Assign Roles, Activate/Deactivate Accounts, Reset Password, Manage Doctors, Manage Staff, Manage Specialties, Manage System Settings, Configure Appointment Rules, Manage Access Permissions.

## **Clinic Manager**

**Who:** The person who oversees clinic operations, doctor schedules, appointment activities, and clinic workflow.

**Use cases:** Log In, View Clinic Schedule, Monitor Doctor Availability, Monitor Appointments, View Pending Appointments, Review Appointment Status, Monitor Patient Flow, View Reports, Monitor Staff Schedules, Request Schedule Adjustments, View Scheduling Conflicts, View Notifications.

## **External Actors**

### **Notification Service**

**Who:** An external service that delivers appointment reminders and notifications to patients, doctors, and clinic staff.

**Note:** Sending notifications is initiated by the clinic system. The notification service delivers messages and returns the delivery result where supported.

**Use cases:** Send Appointment Confirmation, Send Appointment Reminder, Send Cancellation Notification, Send Rescheduling Notification, Send Schedule Update Notification.

---

The full functional requirements are documented in `functional_requirements.md`.
