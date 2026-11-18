# Module Specification: Patient Records & Class Mapping

## 1. Module Overview

The Patient Records & Class Mapping module maintains
patients' medical histories and defines the entity classes
used by the Smart Clinic Appointment System.

The module allows authorized medical staff to record,
retrieve, and manage patient medical information securely.

## 2. Data Attributes

The PatientRecord entity contains the following attributes:

| Attribute           | Data Type   | Description                      |
| ------------------- | ----------- | -------------------------------- |
| recordId            | String (PK) | Unique medical record identifier |
| patientId           | String (FK) | Reference to the patient         |
| visitDate           | Timestamp   | Date and time of the visit       |
| diagnosisNotes      | Text        | Clinical diagnosis and notes     |
| prescriptionDetails | Text        | Prescribed medication details    |

PK = Primary Key
FK = Foreign Key

## 3. Use Case: Maintain Medical Records

**Actor:** Doctor / Authorized Medical Staff

**Precondition:**

- The staff member is authenticated.
- The patient has an active clinical encounter.

**Main Flow:**

1. Staff searches for a patient.
2. The system retrieves the patient's profile.
3. Staff enters diagnosis notes.
4. Staff adds prescription details when applicable.
5. The system validates the information.
6. The system saves the medical record.
7. The system confirms successful storage.

**Postcondition:**
The medical record is securely stored and associated
with the correct patient.

## 4. Data Privacy and Security

Medical history records are confidential.

Security requirements:

- Only authenticated users can access the module.
- Access is restricted according to user roles.
- Patients can access their own permitted records.
- Unauthorized access must be rejected.
- Sensitive information must be protected during
  transmission and storage.
- Important record activities should be logged.

## 5. Class Modeling Definitions

### Class: PatientRecord

**Attributes:**

- private String recordId
- private String patientId
- private LocalDateTime visitDate
- private String diagnosisNotes
- private String prescriptionDetails

**Methods:**

- public createRecord()
- public updateRecord()
- public getRecordById()
- public getRecordsByPatientId()
- public getRecordsByDateRange()

### Class: Patient

**Attributes:**

- private String patientId
- private String fullName

**Methods:**

- public getPatientDetails()
- public getMedicalHistory()

## 6. History Retrieval Logic

The system supports chronological retrieval of
medical records using date-range filtering.

Requirements:

- Search records by patient ID.
- Filter records by start date and end date.
- Display records in chronological order.
- Use appropriate database indexes to improve
  search performance as data grows.

## 7. First-Time Visitor Handling

When a patient visits the clinic for the first time:

1. The system checks whether the patient exists.
2. If the patient exists, retrieve the existing history.
3. If the patient has no previous medical records,
   initialize an empty medical history collection.
4. Allow authorized staff to create the first record.
5. Associate the new record with the patient ID.

An empty medical history does not mean that the
patient's profile does not exist.

## 8. Verification Status

The module documentation should be checked against
the system architecture and class diagrams.

Verification checklist:

- [ ] PatientRecord attributes are documented.
- [ ] Primary and foreign keys are identified.
- [ ] Use case requirements are documented.
- [ ] Privacy and security rules are defined.
- [ ] Class attributes and methods are documented.
- [ ] History retrieval requirements are defined.
- [ ] First-time visitor handling is documented.
- [ ] Documentation matches the UML class diagram.

## 9. Conclusion

The Patient Records & Class Mapping module provides
a structured approach to maintaining patient medical
histories. It supports secure record management,
historical retrieval, and consistent class modeling
within the Smart Clinic Appointment System.
