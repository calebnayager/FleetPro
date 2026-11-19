# FleetPro Logistics

# Functional Requirements

## 1. Purpose

The purpose of this document is to define the functional requirements for the proposed FleetPro Logistics Vehicle Maintenance Management System.

The functional requirements describe the specific functions and behaviours that the system must provide to satisfy the system requirements identified during the Systems Analysis phase.

These requirements are derived from the system requirements and business requirements established during the previous analysis stages.

The functional requirements will provide a foundation for the development of user stories, use cases, system design, development and testing activities.

## 2. Functional Requirement Structure

Each functional requirement identifies a specific function or behaviour that the system must provide.

The requirements are linked to their corresponding system requirements to maintain traceability throughout the project.

### 2.1 Centralised Maintenance Information

#### FR-001 — Create Maintenance Record

**Requirement:**  

The system shall allow authorised users to create a maintenance record for a vehicle.

**Reason:**  

Users require a structured method of recording completed maintenance information within the centralised system.

**Source:**  

SR-001 — Centralised Maintenance Information.

---

#### FR-002 — View Maintenance Records

**Requirement:**  

The system shall allow authorised users to view maintenance records stored within the system.

**Reason:**  

Users need to access recorded maintenance information without relying on disconnected physical records, spreadsheets or communication channels.

**Source:**  

SR-001 — Centralised Maintenance Information.

---

#### FR-003 — Update Maintenance Record

**Requirement:**  

The system shall allow authorised users to update maintenance records when corrections or additional information are required.

**Reason:**  

Maintenance information may require correction or additional details after a record has been created.

**Source:**  

SR-001 — Centralised Maintenance Information.

---

#### FR-004 — Associate Maintenance Record with Vehicle

**Requirement:**  

The system shall associate each maintenance record with the relevant vehicle.

**Reason:**  

Maintenance information must be linked to a specific vehicle so that users can maintain and retrieve the correct maintenance history.

**Source:**  

SR-001 — Centralised Maintenance Information.

### 2.2 Accurate Maintenance History

#### FR-005 — View Vehicle Maintenance History

**Requirement:**  

The system shall allow authorised users to view the maintenance history of a selected vehicle.

**Reason:**  

Users need to review previous maintenance performed on a vehicle to understand its maintenance history and support informed maintenance decisions.

**Source:**  

SR-002 — Accurate Maintenance History.

---

#### FR-006 — Record Maintenance Date

**Requirement:**  

The system shall allow authorised users to record the date on which maintenance was performed.

**Reason:**  

The maintenance date is required to establish when maintenance occurred and maintain an accurate chronological maintenance history.

**Source:**  

SR-002 — Accurate Maintenance History.

---

#### FR-007 — Record Maintenance Details

**Requirement:**  

The system shall allow authorised users to record details of the maintenance or repair performed on a vehicle.

**Reason:**  

Maintenance details are required to provide a clear record of the work performed on each vehicle.

**Source:**  

SR-002 — Accurate Maintenance History.

---

#### FR-008 — Display Maintenance History Chronologically

**Requirement:**  

The system shall display maintenance records for a vehicle in chronological order.

**Reason:**  

A chronological maintenance history will allow users to understand the sequence of maintenance activities performed on a vehicle.

**Source:**  

SR-002 — Accurate Maintenance History.

---

### 2.3 Maintenance Record Management

#### FR-009 — Validate Required Maintenance Information

**Requirement:**  

The system shall require specified maintenance information to be provided before a maintenance record can be saved.

**Reason:**  

Required information helps ensure that maintenance records are complete and consistently captured.

**Source:**  

SR-003 — Maintenance Record Management.

---

#### FR-010 — Save Maintenance Record

**Requirement:**  

The system shall save completed maintenance records so that they can be accessed after they have been recorded.

**Reason:**  

Maintenance information must be retained so that it becomes part of the vehicle's maintenance history and can be retrieved when required.

**Source:**  

SR-003 — Maintenance Record Management.

---

#### FR-011 — Identify Maintenance Record

**Requirement:**  

The system shall assign a unique identifier to each maintenance record.

**Reason:**  

A unique identifier will allow individual maintenance records to be distinguished and referenced within the system.

**Source:**  

SR-003 — Maintenance Record Management.

---

### 2.4 Maintenance Cost Tracking

#### FR-012 — Record Maintenance Cost

**Requirement:**  

The system shall allow authorised users to record the cost associated with a maintenance activity.

**Reason:**  

Maintenance costs need to be associated with the relevant maintenance activity and vehicle to support accurate cost tracking.

**Source:**  

SR-004 — Maintenance Cost Tracking.

---

#### FR-013 — Calculate Maintenance Costs

**Requirement:**  

The system shall calculate maintenance costs for selected vehicles and defined reporting periods.

**Reason:**  

The system should reduce reliance on manual spreadsheet calculations and provide a consistent method of calculating maintenance expenditure.

**Source:**  

SR-004 — Maintenance Cost Tracking.

---

#### FR-014 — View Maintenance Cost Information

**Requirement:**  

The system shall allow authorised users to view maintenance cost information associated with vehicles and maintenance activities.

**Reason:**  

Users require access to maintenance cost information to monitor expenditure and support maintenance and financial decision-making.

**Source:**  

SR-004 — Maintenance Cost Tracking.

---

### 2.5 Vehicle Maintenance Status Visibility

#### FR-015 — View Vehicle Maintenance Status

**Requirement:**  

The system shall allow authorised users to view the current maintenance status of a vehicle.

**Reason:**  

Users need visibility of vehicle maintenance status to understand whether a vehicle has outstanding or completed maintenance activity.

**Source:**  

SR-005 — Vehicle Maintenance Status Visibility.

---

#### FR-016 — Update Maintenance Status

**Requirement:**  

The system shall allow authorised users to update the maintenance status of a vehicle or maintenance activity.

**Reason:**  

Maintenance status needs to reflect changes as maintenance requests are reviewed, performed or completed.

**Source:**  

SR-005 — Vehicle Maintenance Status Visibility.

---

### 2.6 Maintenance Information Retrieval

#### FR-017 — Search Maintenance Records

**Requirement:**  

The system shall allow authorised users to search for maintenance records using vehicle information.

**Reason:**  

Users need an efficient method of locating maintenance information without searching through multiple physical and digital sources.

**Source:**  

SR-006 — Maintenance Information Retrieval.

---

#### FR-018 — Filter Maintenance Information

**Requirement:**  

The system shall allow authorised users to filter maintenance information using relevant criteria such as vehicle and maintenance date.

**Reason:**  

Filtering will allow users to narrow maintenance information and locate relevant records more efficiently.

**Source:**  

SR-006 — Maintenance Information Retrieval.

---

### 2.7 Scalability

The scalability requirement is primarily addressed through non-functional requirements rather than additional functional requirements.

SR-007 describes the system's ability to support the current fleet and future growth. This will therefore be addressed through requirements relating to system capacity, performance, maintainability and scalability in the **Non-Functional Requirements** document.

---

### 2.8 Maintenance Reporting

#### FR-019 — Generate Maintenance Report

**Requirement:**  

The system shall allow authorised users to generate maintenance reports based on recorded maintenance information.

**Reason:**  

Structured reports will allow management and relevant users to review maintenance activity and support operational decision-making.

**Source:**  

SR-008 — Maintenance Reporting.

---

#### FR-020 — Generate Maintenance Cost Summary

**Requirement:**  

The system shall allow authorised users to generate summaries of maintenance costs for selected vehicles and reporting periods.

**Reason:**  

Cost summaries will provide structured financial information for monitoring maintenance expenditure and supporting management decisions.

**Source:**  

SR-008 — Maintenance Reporting.

---

#### FR-021 — Filter Maintenance Reports

**Requirement:**  

The system shall allow authorised users to filter maintenance reports using relevant criteria such as vehicle and reporting period.

**Reason:**  

Filtering reports will allow users to obtain information relevant to specific vehicles or periods without reviewing unrelated maintenance information.

**Source:**  

SR-008 — Maintenance Reporting.

---

## 3. Functional Requirements Traceability

The functional requirements provide a detailed representation of the system behaviour required to support the system requirements.

| Functional Requirement | System Requirement | Business Requirement |
|---|---|---|
| FR-001 — Create Maintenance Record | SR-001 — Centralised Maintenance Information | BR-001 — Centralised Maintenance Information |
| FR-002 — View Maintenance Records | SR-001 — Centralised Maintenance Information | BR-001 — Centralised Maintenance Information |
| FR-003 — Update Maintenance Record | SR-001 — Centralised Maintenance Information | BR-001 — Centralised Maintenance Information |
| FR-004 — Associate Maintenance Record with Vehicle | SR-001 — Centralised Maintenance Information | BR-001 — Centralised Maintenance Information |
| FR-005 — View Vehicle Maintenance History | SR-002 — Accurate Maintenance History | BR-002 — Accurate Maintenance History |
| FR-006 — Record Maintenance Date | SR-002 — Accurate Maintenance History | BR-002 — Accurate Maintenance History |
| FR-007 — Record Maintenance Details | SR-002 — Accurate Maintenance History | BR-002 — Accurate Maintenance History |
| FR-008 — Display Maintenance History Chronologically | SR-002 — Accurate Maintenance History | BR-002 — Accurate Maintenance History |
| FR-009 — Validate Required Maintenance Information | SR-003 — Maintenance Record Management | BR-003 — Maintenance Record Management |
| FR-010 — Save Maintenance Record | SR-003 — Maintenance Record Management | BR-003 — Maintenance Record Management |
| FR-011 — Identify Maintenance Record | SR-003 — Maintenance Record Management | BR-003 — Maintenance Record Management |
| FR-012 — Record Maintenance Cost | SR-004 — Maintenance Cost Tracking | BR-004 — Maintenance Cost Tracking |
| FR-013 — Calculate Maintenance Costs | SR-004 — Maintenance Cost Tracking | BR-004 — Maintenance Cost Tracking |
| FR-014 — View Maintenance Cost Information | SR-004 — Maintenance Cost Tracking | BR-004 — Maintenance Cost Tracking |
| FR-015 — View Vehicle Maintenance Status | SR-005 — Vehicle Maintenance Status Visibility | BR-005 — Vehicle Maintenance Status Visibility |
| FR-016 — Update Maintenance Status | SR-005 — Vehicle Maintenance Status Visibility | BR-005 — Vehicle Maintenance Status Visibility |
| FR-017 — Search Maintenance Records | SR-006 — Maintenance Information Retrieval | BR-006 — Maintenance Information Retrieval |
| FR-018 — Filter Maintenance Information | SR-006 — Maintenance Information Retrieval | BR-006 — Maintenance Information Retrieval |
| FR-019 — Generate Maintenance Report | SR-008 — Maintenance Reporting | BR-008 — Maintenance Reporting |
| FR-020 — Generate Maintenance Cost Summary | SR-008 — Maintenance Reporting | BR-008 — Maintenance Reporting |
| FR-021 — Filter Maintenance Reports | SR-008 — Maintenance Reporting | BR-008 — Maintenance Reporting |

## 4. Functional Requirements Conclusion

The functional requirements define the specific functions that the proposed FleetPro Vehicle Maintenance Management System must provide.

The requirements cover the creation, management, retrieval and reporting of vehicle maintenance information, including maintenance history, maintenance costs and vehicle maintenance status.

The functional requirements are traceable to the system requirements and the original business requirements established during the Business Analysis phase.

These requirements provide the foundation for the next Systems Analysis activities, including non-functional requirements, business rules, user stories and use cases.