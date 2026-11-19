# FleetPro Logistics

# User Stories

## 1. Purpose

This document defines the user stories for the proposed FleetPro Logistics Vehicle Maintenance Management System.

User stories describe the capabilities that stakeholders need from the proposed system. Each story explains who needs a capability, what they need to do and why it matters. Acceptance criteria define the expected outcomes and will support future testing.

## 2. User Story Format

Each user story follows this format:

**As a** [user role], **I want** [a capability], **so that** [a business benefit].

Acceptance criteria specify the conditions that must be satisfied for the story to be considered complete.

## 3. User Stories

### US-001 — Create a Maintenance Record

**User Story**

As a Fleet Administrator, I want to create a maintenance record for a vehicle, so that maintenance activities can be recorded centrally.

**Acceptance Criteria**

- An authorised Fleet Administrator can access the maintenance record creation function.
- The user can identify the relevant vehicle.
- The user can enter the required maintenance information.
- The system validates mandatory information before saving.
- A valid record is saved and available for later retrieval.
- Each record receives a unique identifier.

**Related Requirements:** FR-001, FR-004, FR-009, FR-010, FR-011.

### US-002 — View Maintenance Records

**User Story**

As an authorised Fleet Administrator, Mechanic / Maintenance Team member or Fleet Manager, I want to view saved maintenance records, so that I can review previously recorded maintenance activities.

**Acceptance Criteria**

- Authorised users can access saved maintenance records according to their permissions.
- The system displays the information associated with the selected record.
- The displayed record is associated with the correct vehicle.
- Individual records can be distinguished from one another.
- The system prevents unauthorised users from accessing restricted records.

**Related Requirements:** FR-002, FR-004, FR-011.

### US-003 — Update a Maintenance Record

**User Story**

As an authorised Fleet Administrator or Mechanic / Maintenance Team member, I want to update an existing maintenance record, so that corrections and additional information can be recorded.

**Acceptance Criteria**

- An authorised user can select an existing maintenance record.
- The system displays its current information.
- The user can edit permitted fields.
- The system validates required information before saving changes.
- Saved changes remain available when the record is retrieved again.
- The record remains associated with the correct vehicle.
- Users cannot update fields or records outside their permissions.

**Related Requirements:** FR-003, FR-004, FR-009, FR-010.

### US-004 — View Vehicle Maintenance History

**User Story**

As a Driver, Mechanic / Maintenance Team member or Fleet Manager, I want to view the maintenance history of a selected vehicle, so that I can review its previous maintenance activities.

**Acceptance Criteria**

- An authorised user can identify a vehicle.
- The system displays maintenance records associated with that vehicle.
- Records are displayed in chronological order.
- Available maintenance dates and details are displayed.
- Records belonging to unrelated vehicles are excluded.
- The system only displays information the user is authorised to access.

**Related Requirements:** FR-004, FR-005, FR-006, FR-007, FR-008.

### US-005 — Record Maintenance Costs

**User Story**

As a Fleet Administrator, I want to record maintenance costs, so that vehicle maintenance expenditure can be tracked.

**Acceptance Criteria**

- The user can enter a cost for the relevant maintenance activity.
- The cost is associated with the correct maintenance record and vehicle.
- The system validates the cost according to the defined business rules.
- Saved costs remain available for retrieval.
- Negative costs are rejected under the proposed cost-validation rule.

**Related Requirements:** FR-004, FR-012, FR-014.

### US-006 — Calculate Maintenance Costs

**User Story**

As a Fleet Manager, I want to calculate maintenance costs for selected vehicles and reporting periods, so that I can review maintenance expenditure.

**Acceptance Criteria**

- The user can select the relevant vehicle or vehicles, where supported.
- The user can specify a reporting period.
- The system calculates totals from applicable recorded costs.
- The result corresponds to the selected vehicles and period.
- Costs outside the selected criteria are excluded.
- The system does not imply that missing or unrecorded costs are included in the calculation.

**Related Requirements:** FR-013, FR-020.

### US-007 — View Vehicle Maintenance Status

**User Story**

As a Driver or Fleet Manager, I want to view a vehicle's maintenance status, so that I can understand its recorded maintenance position.

**Acceptance Criteria**

- An authorised user can identify a vehicle.
- The system displays the recorded maintenance status.
- The status belongs to the selected vehicle.
- The status is presented clearly.
- The system only displays status information the user is authorised to access.

**Related Requirements:** FR-015.

### US-008 — Update Maintenance Status

**User Story**

As a Mechanic / Maintenance Team member, I want to update the status of a vehicle or maintenance activity, so that the system reflects the latest known status.

**Acceptance Criteria**

- The user can select the relevant vehicle or maintenance activity.
- The system provides approved status options once these have been defined.
- The system saves a valid status update.
- The updated status is displayed when the relevant record is viewed again.
- The update applies to the intended vehicle or maintenance activity.
- Unauthorised users cannot update maintenance status.

**Related Requirements:** FR-015, FR-016.

### US-009 — Search Maintenance Records

**User Story**

As a Fleet Administrator or Fleet Manager, I want to search maintenance records using vehicle information, so that I can locate relevant records efficiently.

**Acceptance Criteria**

- The user can enter supported vehicle search information.
- The system returns records matching the search criteria.
- The results correspond to the entered criteria.
- The system communicates when no matching records are found.
- Search results only include records the user is authorised to access.

**Related Requirements:** FR-017.

### US-010 — Filter Maintenance Information

**User Story**

As a Fleet Manager, I want to filter maintenance information by vehicle and date, so that I can focus on relevant maintenance activities.

**Acceptance Criteria**

- The user can apply supported filters.
- The system displays records matching the selected criteria.
- Records that do not match are excluded.
- The user can change or clear filters.
- Filtering does not change the underlying maintenance records.

**Related Requirements:** FR-018.

### US-011 — Generate Maintenance Reports

**User Story**

As a Fleet Manager, I want to generate maintenance reports, so that I can review maintenance information in a structured format and make it available for management review.

**Acceptance Criteria**

- The Fleet Manager can request a supported maintenance report.
- The report is generated from recorded maintenance information.
- Relevant maintenance details are presented clearly.
- Supported vehicle and reporting-period filters are applied.
- The Fleet Manager can review the generated report.
- The CEO / Senior Management can access generated reports when authorised.
- The system prevents unauthorised access to restricted reports.

**Related Requirements:** FR-019, FR-021.

### US-012 — Generate Maintenance Cost Summaries

**User Story**

As a Fleet Manager, I want to generate maintenance cost summaries for selected vehicles and reporting periods, so that I can review maintenance expenditure and make the information available for management review.

**Acceptance Criteria**

- The Fleet Manager can select the relevant vehicle or vehicles, where supported.
- The Fleet Manager can select a reporting period.
- The system calculates the summary from applicable recorded costs.
- The summary reflects the selected criteria.
- The Fleet Manager can review the generated cost summary.
- The CEO / Senior Management can access generated cost summaries when authorised.
- The system prevents unauthorised access to restricted cost summaries.
- The system does not imply that missing or unrecorded costs are included.

**Related Requirements:** FR-013, FR-020, FR-021.

## 4. User Story Traceability

| User Story | Related Functional Requirements |
|---|---|
| US-001 — Create a Maintenance Record | FR-001, FR-004, FR-009, FR-010, FR-011 |
| US-002 — View Maintenance Records | FR-002, FR-004, FR-011 |
| US-003 — Update a Maintenance Record | FR-003, FR-004, FR-009, FR-010 |
| US-004 — View Vehicle Maintenance History | FR-004, FR-005, FR-006, FR-007, FR-008 |
| US-005 — Record Maintenance Costs | FR-004, FR-012, FR-014 |
| US-006 — Calculate Maintenance Costs | FR-013, FR-020 |
| US-007 — View Vehicle Maintenance Status | FR-015 |
| US-008 — Update Maintenance Status | FR-015, FR-016 |
| US-009 — Search Maintenance Records | FR-017 |
| US-010 — Filter Maintenance Information | FR-018 |
| US-011 — Generate Maintenance Reports | FR-019, FR-021 |
| US-012 — Generate Maintenance Cost Summaries | FR-013, FR-020, FR-021 |

## 5. Outstanding Clarifications

The following details must be clarified before implementation and testing:

- **Mandatory fields:** Which fields are required when creating or updating a maintenance record?
- **User permissions:** Which roles can create, view, update, search and report on maintenance information?
- **Role access:** Should Drivers, Fleet Administrators, Mechanics, Fleet Managers and CEO / Senior Management have separate access permissions?
- **Status values:** Which vehicle and maintenance status values will the system support?
- **Status updates:** Which roles may update statuses, and which status changes are permitted?
- **Cost handling:** How should missing, pending, corrected or unconfirmed maintenance costs appear in the system and reports?
- **Reporting access:** Should CEO / Senior Management have read-only access to generated maintenance reports and cost summaries?
- **Report formats:** Which report formats and export options are required?
- **Search criteria:** Which vehicle and maintenance fields should users be able to search?
- **Reporting periods:** How should reporting-period start and end dates be defined?
- **Audit history:** Should the system record who created or changed a maintenance record and when?

These details should be confirmed with the relevant stakeholders before the requirements are finalised and implemented.

## 6. Conclusion

These user stories translate FleetPro's functional requirements into user-centred goals with acceptance criteria. They describe the expected capabilities for Drivers, Fleet Administrators, Mechanics / Maintenance Teams, Fleet Managers and CEO / Senior Management.

The user stories provide a foundation for use-case analysis, system design, development and testing. Their acceptance criteria will help define how the proposed system's functionality should be verified during future testing.