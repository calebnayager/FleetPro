# FleetPro Logistics

# Business Requirements

## 1. Purpose

The purpose of this document is to define the business requirements for improving FleetPro Logistics' vehicle maintenance-recording process.

The requirements are derived from the findings identified during the stakeholder analysis, investigation and root cause analysis.

These requirements describe the business needs that the proposed solution must address to improve the recording, tracking, retrieval and management of vehicle maintenance information.

The business requirements will provide the foundation for defining the functional and non-functional requirements of the proposed system during the systems analysis phase.


## 2. Business Need

FleetPro needs to improve the way vehicle maintenance information is recorded, stored, accessed and managed.

The current maintenance-recording process relies on physical suspension files, spreadsheets, email and WhatsApp. As the fleet grew to more than 300 trucks, the existing process became increasingly difficult to manage and maintain accurately.

The business therefore needs a more consistent and scalable approach to managing vehicle maintenance information so that previous maintenance can be identified, maintenance records can be maintained accurately, and management can obtain reliable information about vehicle maintenance and associated costs.

## 3. Business Objectives

The proposed improvement should support FleetPro in achieving the following business objectives:

- Improve the accuracy and completeness of vehicle maintenance records.
- Improve the ability to identify previous maintenance performed on each vehicle.
- Improve the visibility of vehicle maintenance information.
- Improve the recording and monitoring of maintenance costs.
- Reduce difficulties associated with retrieving historical maintenance information.
- Establish a maintenance-recording process that can support the size and continued growth of the fleet.
- Provide structured maintenance information to support management reporting and decision-making.


## 4. Business Requirements


### BR-001 — Centralised Maintenance Information

**Requirement:**  

FleetPro requires a centralised method of maintaining and accessing vehicle maintenance information.

**Business Reason:**  

Maintenance information is currently recorded across WhatsApp, spreadsheets and paper documentation, making it difficult to accurately track previous maintenance.

**Source:**  

Investigation — Maintenance Information Across Multiple Channels.

---

### BR-002 — Accurate Maintenance History

**Requirement:**  

FleetPro requires accurate maintenance history to be maintained for each vehicle.

**Business Reason:**  

The business needs to determine what maintenance has previously been performed on a vehicle to reduce the risk of maintenance being performed when the required maintenance has already been completed.

**Source:**  

Investigation — Problem Being Investigated.

---

### BR-003 — Maintenance Record Management

**Requirement:**  

FleetPro requires a standardised method for recording vehicle maintenance information, including the maintenance performed, maintenance date and associated details.

**Business Reason:**  

The investigation found that there was no formal maintenance-recording process initially and that maintenance information was recorded through different methods.

**Source:**  

Investigation — Standardised Maintenance-Recording Process.

---

### BR-004 — Maintenance Cost Tracking

**Requirement:**  

FleetPro requires maintenance costs to be recorded and associated with the relevant vehicle and maintenance activity.

**Business Reason:**  

The spreadsheet process was introduced to record the individual cost of repairs and calculate monthly and yearly maintenance totals for each vehicle. This information supports the monitoring of maintenance expenditure.

**Source:**  

Investigation — Standardised Maintenance-Recording Process.

---

### BR-005 — Vehicle Maintenance Status Visibility

**Requirement:**  

FleetPro requires visibility of the maintenance status and history of each vehicle.

**Business Reason:**  

The investigation found that management visibility became more difficult as the fleet grew and maintenance information became harder to manage. Improved visibility can help the business determine whether maintenance has already been performed on a vehicle.

**Source:**  

Investigation — Growth of Fleet and Physical Records.

---

### BR-006 — Maintenance Information Retrieval

**Requirement:**  

FleetPro requires maintenance information to be easily retrieved for individual vehicles when required.

**Business Reason:**  

Maintenance information is currently distributed across physical suspension files, spreadsheets, email and WhatsApp. This makes it difficult to locate and verify previous maintenance information efficiently.

**Source:**  

Investigation — Maintenance Information Across Multiple Channels.

---

### BR-007 — Scalable Maintenance-Recording Process

**Requirement:**  

FleetPro requires a maintenance-recording process that can accommodate the current size of the fleet and future growth in the volume of maintenance information.

**Business Reason:**  

The fleet grew to more than 300 trucks, while the existing maintenance-recording process was not updated to accommodate the increased volume of vehicles and information. The investigation identified the lack of scalability as the underlying root cause.

**Source:**  

Investigation — Maintenance-Recording Process and Fleet Growth.

---

### BR-008 — Maintenance Reporting

**Requirement:**  

FleetPro requires maintenance information to be available in a structured form that supports maintenance and financial reporting.

**Business Reason:**  

The later spreadsheet process was designed to record repair details, individual maintenance costs and monthly and yearly maintenance totals for each vehicle. These records provide information that can support management monitoring and decision-making.

**Source:**  

Investigation — Standardised Maintenance-Recording Process and Maintenance-Recording Process and Fleet Growth.


## 5. Requirement Prioritisation

The business requirements have been prioritised using the MoSCoW
prioritisation technique.

The prioritisation is based on the relationship between each
requirement and the business problem identified during the
investigation and root cause analysis.

The priorities below represent the proposed scope for the FleetPro
solution.

| Requirement | Description | Priority |
|---|---|---|
| BR-001 | Centralised Maintenance Information | Must Have |
| BR-002 | Accurate Maintenance History | Must Have |
| BR-003 | Maintenance Record Management | Must Have |
| BR-004 | Maintenance Cost Tracking | Should Have |
| BR-005 | Vehicle Maintenance Status Visibility | Should Have |
| BR-006 | Maintenance Information Retrieval | Must Have |
| BR-007 | Scalable Maintenance-Recording Process | Must Have |
| BR-008 | Maintenance Reporting | Should Have |


## 6. Requirements Traceability

Requirements traceability is used to establish a clear relationship
between the findings identified during the investigation, the business
requirements and the business objectives they support.

This ensures that the business requirements are based on identified
business needs and problems rather than being introduced without
supporting evidence.

| Requirement | Investigation Finding | Business Objective |
|---|---|---|
| BR-001 | Maintenance information is recorded across WhatsApp, spreadsheets and paper documentation. | Improve the accuracy and accessibility of vehicle maintenance records. |
| BR-002 | Previous maintenance information can be difficult to track accurately. | Improve the ability to identify previous maintenance performed on each vehicle. |
| BR-003 | There was no formal maintenance-recording process initially. | Establish a consistent method for recording maintenance information. |
| BR-004 | The spreadsheet process recorded individual repair costs and monthly and yearly maintenance totals. | Improve the recording and monitoring of maintenance costs. |
| BR-005 | Management visibility became more difficult as the fleet grew and maintenance information became harder to manage. | Improve visibility of vehicle maintenance information. |
| BR-006 | Maintenance information is distributed across physical files, spreadsheets, email and WhatsApp. | Improve the ability to retrieve historical maintenance information. |
| BR-007 | The maintenance-recording process was not updated as the fleet grew to more than 300 trucks. | Establish a maintenance-recording process that can support fleet growth and increasing information volume. |
| BR-008 | The spreadsheet process provided repair details, individual costs and monthly and yearly totals. | Provide structured maintenance information to support management reporting and decision-making. |


## 7. Assumptions and Constraints

### 7.1 Assumptions

The following assumptions have been made for the purpose of analysing
and designing the proposed FleetPro solution:

- Existing vehicle maintenance information will be used as a source for
  populating the proposed maintenance records.
- Users responsible for vehicle maintenance administration will provide
  the required maintenance information when records are created or
  updated.
- The proposed solution will need to support the maintenance information
  currently required by the business, including maintenance dates,
  maintenance details and associated costs.
- Historical maintenance information may be incomplete because the
  investigation identified gaps in records and incomplete historical
  spreadsheets.

### 7.2 Constraints

The following constraints have been identified from the investigation:

- Historical maintenance information is incomplete for some vehicles.
- More than five years of historical maintenance information may need to
  be reconstructed or captured.
- The fleet contains more than 300 trucks, creating a significant volume
  of maintenance information to manage.
- Existing maintenance information is distributed across physical files,
  spreadsheets, email and WhatsApp.
- Physical suspension files remain the official source of maintenance
  documentation in the existing process.


  ## 8. Requirement Validation

The business requirements were reviewed against the findings from the
investigation and root cause analysis to determine whether they are
relevant, supported by evidence, clearly defined and appropriate at the
business level.

The validation also checks that the requirements do not unnecessarily
duplicate one another and that they describe business needs rather than
specific technical solutions.

| Requirement | Relevant | Supported by Investigation | Clear | Business-Focused | Validation Result |
|---|---|---|---|---|---|
| BR-001 | Yes | Yes | Yes | Yes | Valid |
| BR-002 | Yes | Yes | Yes | Yes | Valid |
| BR-003 | Yes | Yes | Yes | Yes | Valid |
| BR-004 | Yes | Yes | Yes | Yes | Valid |
| BR-005 | Yes | Yes | Yes | Yes | Valid |
| BR-006 | Yes | Yes | Yes | Yes | Valid |
| BR-007 | Yes | Yes | Yes | Yes | Valid |
| BR-008 | Yes | Yes | Yes | Yes | Valid |

### Validation Summary

The validation confirmed that all eight business requirements are
supported by findings identified during the investigation and root
cause analysis.

The requirements address the key business needs identified during the
analysis, including centralised maintenance information, accurate
maintenance history, standardised record management, cost tracking,
maintenance visibility, information retrieval, scalability and
reporting.

The requirements remain technology-independent and therefore provide a
suitable foundation for defining the solution requirements during the
systems analysis and design stages.


