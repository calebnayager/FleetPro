# FleetPro Logistics

# Business Rules

## 1. Purpose

The purpose of this document is to define the business rules governing maintenance information within the proposed FleetPro Logistics Vehicle Maintenance Management System.

Business rules establish the conditions, constraints and principles that must be followed when maintenance information is recorded, managed, retrieved and reported.

These rules are based on the FleetPro business scenario and the requirements identified during the Business Analysis and Systems Analysis phases. Where a rule represents a proposed system constraint rather than a confirmed existing company policy, it is identified as a proposed rule.

The business rules will support the development of functional requirements, user stories, use cases, data models, system design and testing activities.

## 2. Business Rule Categories

The following categories are used to organise the business rules:

- Vehicle and maintenance record identification
- Maintenance information completeness
- Maintenance history
- Maintenance cost tracking
- Maintenance status
- Data accuracy and consistency
- Historical record preservation

## 3. Business Rules

### 3.1 Vehicle and Maintenance Record Identification

#### BR-001 — Vehicle Association

**Rule:**

Every maintenance record must be associated with the identifiable vehicle to which the maintenance activity relates.

**Rationale:**

Maintenance information must be linked to the correct vehicle so that users can retrieve an accurate maintenance history and avoid confusion between vehicles.

**Related Requirements:**

- FR-004 — Associate Maintenance Record with Vehicle
- FR-005 — View Vehicle Maintenance History

**Status:** Proposed business rule.

---

#### BR-002 — Unique Maintenance Record Identification

**Rule:**

Each maintenance record must have a unique identifier that distinguishes it from all other maintenance records.

**Rationale:**

Unique identification allows individual records to be referenced, retrieved and managed without confusing one maintenance event with another.

**Related Requirements:**

- FR-011 — Identify Maintenance Record

**Status:** Proposed business rule.

### 3.2 Maintenance Information Completeness

#### BR-003 — Required Maintenance Information

**Rule:**

A maintenance record must contain all information designated as mandatory before it can be saved as a complete record.

**Rationale:**

Required information supports consistent recordkeeping and reduces incomplete maintenance records that may be difficult to interpret or use in reporting.

**Related Requirements:**

- FR-006 — Record Maintenance Date
- FR-007 — Record Maintenance Details
- FR-009 — Validate Required Maintenance Information
- FR-010 — Save Maintenance Record

**Status:** Proposed business rule. The exact mandatory fields must be confirmed during detailed requirements and system design.

### 3.3 Maintenance History

#### BR-004 — Maintenance History Association

**Rule:**

Maintenance history for a vehicle must include the maintenance records associated with that vehicle and must not incorrectly include records belonging to another vehicle.

**Rationale:**

Accurate vehicle-specific history allows users to review previous maintenance activities and supports informed maintenance decisions.

**Related Requirements:**

- FR-004 — Associate Maintenance Record with Vehicle
- FR-005 — View Vehicle Maintenance History
- FR-008 — Display Maintenance History Chronologically

**Status:** Proposed business rule.

---

#### BR-005 — Maintenance Date Accuracy

**Rule:**

The maintenance date recorded for a maintenance activity must represent the date on which that activity was performed.

**Rationale:**

Accurate dates are necessary to maintain a meaningful maintenance timeline and allow users to review maintenance events in the correct chronological context.

**Related Requirements:**

- FR-006 — Record Maintenance Date
- FR-008 — Display Maintenance History Chronologically

**Status:** Proposed business rule.

### 3.4 Maintenance Cost Tracking

#### BR-006 — Non-Negative Maintenance Cost

**Rule:**

A maintenance cost recorded for a maintenance activity must not be negative.

**Rationale:**

Negative costs would ordinarily represent invalid maintenance expenditure data and could distort cost calculations and reporting. Any future need to represent credits or adjustments must be handled through an explicitly defined business process.

**Related Requirements:**

- FR-012 — Record Maintenance Cost
- FR-013 — Calculate Maintenance Costs
- FR-014 — View Maintenance Cost Information

**Status:** Proposed business rule.

---

#### BR-007 — Maintenance Cost Association

**Rule:**

Each recorded maintenance cost must be associated with the maintenance activity and vehicle to which the cost relates.

**Rationale:**

Cost information must be traceable to the relevant maintenance activity to support accurate vehicle-level cost tracking and reporting.

**Related Requirements:**

- FR-004 — Associate Maintenance Record with Vehicle
- FR-012 — Record Maintenance Cost
- FR-013 — Calculate Maintenance Costs
- FR-020 — Generate Maintenance Cost Summary

**Status:** Proposed business rule.

### 3.5 Maintenance Status

#### BR-008 — Maintenance Status Accuracy

**Rule:**

The maintenance status recorded in the system must reflect the current known status of the relevant vehicle or maintenance activity.

**Rationale:**

Accurate status information helps users understand maintenance progress and avoid relying on outdated or misleading status information.

**Related Requirements:**

- FR-015 — View Vehicle Maintenance Status
- FR-016 — Update Maintenance Status

**Status:** Proposed business rule. Permitted status values and transition rules must be defined during detailed requirements and system design.

### 3.6 Data Accuracy and Consistency

#### BR-009 — Consistent Maintenance Information

**Rule:**

Maintenance information must remain correctly associated with its relevant vehicle, maintenance activity, date and cost information wherever those details are recorded.

**Rationale:**

Incorrect associations or inconsistent information could result in inaccurate maintenance histories, cost summaries and management reports.

**Related Requirements:**

- FR-004 — Associate Maintenance Record with Vehicle
- FR-006 — Record Maintenance Date
- FR-012 — Record Maintenance Cost
- FR-019 — Generate Maintenance Report
- FR-020 — Generate Maintenance Cost Summary

**Status:** Proposed business rule.

### 3.7 Historical Record Preservation

#### BR-010 — Preservation of Recorded Maintenance History

**Rule:**

Previously recorded maintenance information must remain available for authorised historical reference unless an approved business process permits its correction, archival or removal.

**Rationale:**

FleetPro requires maintenance history for ongoing operational reference and cost tracking. Historical information should not become unavailable through routine record updates.

**Related Requirements:**

- FR-003 — Update Maintenance Record
- FR-005 — View Vehicle Maintenance History
- FR-010 — Save Maintenance Record

**Status:** Proposed business rule. Record-retention periods and deletion permissions must be confirmed with relevant stakeholders.

## 4. Business Rules Traceability

The following matrix links the business rules to the relevant functional requirements.

| Business Rule | Functional Requirement | Purpose of Relationship |
|---|---|---|
| BR-001 — Vehicle Association | FR-004, FR-005 | Ensures maintenance information is linked to the correct vehicle. |
| BR-002 — Unique Maintenance Record Identification | FR-011 | Supports unique identification of maintenance records. |
| BR-003 — Required Maintenance Information | FR-006, FR-007, FR-009, FR-010 | Supports complete and consistent record capture. |
| BR-004 — Maintenance History Association | FR-004, FR-005, FR-008 | Supports accurate vehicle-specific maintenance history. |
| BR-005 — Maintenance Date Accuracy | FR-006, FR-008 | Supports accurate chronological maintenance history. |
| BR-006 — Non-Negative Maintenance Cost | FR-012, FR-013, FR-014 | Protects the validity of maintenance cost information. |
| BR-007 — Maintenance Cost Association | FR-004, FR-012, FR-013, FR-020 | Supports accurate vehicle-level cost tracking and summaries. |
| BR-008 — Maintenance Status Accuracy | FR-015, FR-016 | Supports accurate maintenance status visibility. |
| BR-009 — Consistent Maintenance Information | FR-004, FR-006, FR-012, FR-019, FR-020 | Supports consistent information across records and reports. |
| BR-010 — Preservation of Recorded Maintenance History | FR-003, FR-005, FR-010 | Supports continued access to historical maintenance information. |

## 5. Business Rule Considerations

The business rules establish proposed constraints for the FleetPro system. They do not independently define every technical implementation detail.

Further clarification is required for:

- The mandatory fields required for a maintenance record.
- The permitted maintenance status values and transitions.
- The treatment of corrections, cost adjustments and record deletion.
- The retention period for historical maintenance information.
- The approval or authorisation required for changes to existing records.

These details should be clarified with relevant stakeholders before they are finalised as confirmed business policies.

The rules will be used to inform data validation, database constraints, use-case descriptions, system design and test cases.

## 6. Conclusion

The business rules define the proposed constraints governing vehicle identification, maintenance record completeness, maintenance history, cost tracking, status accuracy, data consistency and historical record preservation.

Together with the functional and non-functional requirements, these rules provide a foundation for designing a system that supports reliable maintenance recordkeeping and retrieval.

The rules will inform the next Systems Analysis activities, including user stories, use cases, data requirements and system design.