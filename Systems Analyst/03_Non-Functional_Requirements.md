# FleetPro Logistics

# Non-Functional Requirements

## 1. Purpose

The purpose of this document is to define the non-functional requirements for the proposed FleetPro Logistics Vehicle Maintenance Management System.

Non-functional requirements describe the quality attributes, constraints and operational characteristics that the system must satisfy.

Unlike functional requirements, which describe what the system must do, non-functional requirements describe how well the system should perform and the characteristics it should maintain while providing its functions.

These requirements will guide the System Design, Development, Testing and Deployment stages of the FleetPro project.

## 2. Non-Functional Requirement Categories

The following non-functional requirement categories have been identified for the FleetPro system:

- Performance
- Security
- Usability
- Availability
- Reliability
- Scalability
- Maintainability
- Data Integrity

## 3. Non-Functional Requirements

### 3.1 Performance

#### NFR-001 — System Response Time

**Requirement:**

The system should provide an acceptable response time for normal operations under expected operating conditions.

**Reason:**

Users need to work with maintenance information efficiently without unnecessary delays when using the system.

**Source:**

SR-006 — Maintenance Information Retrieval.

---

#### NFR-002 — Performance Under Normal Load

**Requirement:**

The system should maintain acceptable performance while handling the expected number of vehicles, maintenance records and concurrent users during normal business operations.

**Reason:**

The system must remain responsive as FleetPro users access and manage increasing amounts of maintenance information.

**Source:**

SR-007 — Scalable Maintenance-Recording Process.

---

### 3.2 Security

#### NFR-003 — Protection of Maintenance Information

**Requirement:**

The system shall protect stored maintenance information against unauthorised access, modification and disclosure.

**Reason:**

Vehicle maintenance information is business information and should only be accessed or modified by appropriately authorised users.

**Source:**

SR-001 — Centralised Maintenance Information.

---

#### NFR-004 — Secure Data Transmission

**Requirement:**

Maintenance information transmitted between system components should be protected against unauthorised interception or modification.

**Reason:**

Protecting information during transmission reduces the risk of sensitive business information being exposed or altered.

**Source:**

SR-001 — Centralised Maintenance Information.

---

### 3.3 Usability

#### NFR-005 — User Interface Usability

**Requirement:**

The system should provide a clear and understandable interface that allows intended users to complete common maintenance-related tasks without unnecessary complexity.

**Reason:**

FleetPro users may have different levels of technical experience, so the system should be straightforward to understand and use.

**Source:**

SR-003 — Maintenance Record Management.

---

#### NFR-006 — Interface Consistency

**Requirement:**

The system should maintain consistent navigation, terminology, layout and interaction patterns throughout the application.

**Reason:**

Consistent interface behaviour reduces confusion and helps users understand how different parts of the system operate.

**Source:**

SR-003 — Maintenance Record Management.

---

### 3.4 Availability

#### NFR-007 — System Availability

**Requirement:**

The system should be available during the normal operating periods in which FleetPro users require access to vehicle maintenance information.

**Reason:**

Maintenance information may be required during normal fleet operations, and extended periods of unavailability could interfere with maintenance activities.

**Source:**

SR-005 — Vehicle Maintenance Status Visibility.

---

### 3.5 Reliability

#### NFR-008 — Reliable Operation

**Requirement:**

The system should operate consistently under normal operating conditions and minimise unexpected failures during normal use.

**Reason:**

Users depend on the system to remain available and dependable when recording, accessing and reviewing maintenance information.

**Source:**

SR-003 — Maintenance Record Management.

---

#### NFR-009 — Data Recovery

**Requirement:**

The system should provide an appropriate mechanism for recovering maintenance information following a system failure or data-loss event.

**Reason:**

Maintenance history is important operational information and should not be permanently lost because of a system failure.

**Source:**

SR-002 — Accurate Maintenance History.

---

### 3.6 Scalability

#### NFR-010 — Fleet Capacity

**Requirement:**

The system should support the storage and management of maintenance information for FleetPro's current fleet of more than 300 vehicles without significant degradation of normal system performance.

**Reason:**

The existing process became increasingly difficult to manage as the fleet grew. The proposed system must therefore be capable of supporting the current fleet size.

**Source:**

SR-007 — Scalable Maintenance-Recording Process.

---

#### NFR-011 — Future Growth

**Requirement:**

The system should allow the number of vehicles and maintenance records to increase without requiring a complete redesign of the system.

**Reason:**

FleetPro may continue to grow, and the system should remain suitable as the volume of vehicles and maintenance information increases.

**Source:**

SR-007 — Scalable Maintenance-Recording Process.

---

### 3.7 Maintainability

#### NFR-012 — Maintainable Architecture

**Requirement:**

The system should use a structured and maintainable architecture that allows individual system components to be modified, corrected or improved without unnecessary changes to unrelated components.

**Reason:**

The system will require maintenance and improvements as technical requirements and business needs change.

**Source:**

SR-007 — Scalable Maintenance-Recording Process.

---

### 3.8 Data Integrity

#### NFR-013 — Data Consistency

**Requirement:**

The system should maintain consistent relationships between vehicles, maintenance records and associated maintenance information.

**Reason:**

Inconsistent relationships between records could result in inaccurate maintenance histories, cost information and reporting.

**Source:**

SR-002 — Accurate Maintenance History.

---

#### NFR-014 — Data Persistence

**Requirement:**

The system should preserve successfully stored maintenance information so that it remains available for authorised retrieval after the original record has been created.

**Reason:**

Maintenance records form part of the vehicle's historical information and need to remain available for future reference.

**Source:**

SR-002 — Accurate Maintenance History.

---

## 4. Non-Functional Requirements Traceability

The following traceability matrix shows how the non-functional requirements relate to the system requirements and the original business requirements.

| Non-Functional Requirement | System Requirement | Business Requirement |
|---|---|---|
| NFR-001 — System Response Time | SR-006 — Maintenance Information Retrieval | BR-006 — Maintenance Information Retrieval |
| NFR-002 — Performance Under Normal Load | SR-007 — Scalable Maintenance-Recording Process | BR-007 — Scalable Maintenance-Recording Process |
| NFR-003 — Protection of Maintenance Information | SR-001 — Centralised Maintenance Information | BR-001 — Centralised Maintenance Information |
| NFR-004 — Secure Data Transmission | SR-001 — Centralised Maintenance Information | BR-001 — Centralised Maintenance Information |
| NFR-005 — User Interface Usability | SR-003 — Maintenance Record Management | BR-003 — Maintenance Record Management |
| NFR-006 — Interface Consistency | SR-003 — Maintenance Record Management | BR-003 — Maintenance Record Management |
| NFR-007 — System Availability | SR-005 — Vehicle Maintenance Status Visibility | BR-005 — Vehicle Maintenance Status Visibility |
| NFR-008 — Reliable Operation | SR-003 — Maintenance Record Management | BR-003 — Maintenance Record Management |
| NFR-009 — Data Recovery | SR-002 — Accurate Maintenance History | BR-002 — Accurate Maintenance History |
| NFR-010 — Fleet Capacity | SR-007 — Scalable Maintenance-Recording Process | BR-007 — Scalable Maintenance-Recording Process |
| NFR-011 — Future Growth | SR-007 — Scalable Maintenance-Recording Process | BR-007 — Scalable Maintenance-Recording Process |
| NFR-012 — Maintainable Architecture | SR-007 — Scalable Maintenance-Recording Process | BR-007 — Scalable Maintenance-Recording Process |
| NFR-013 — Data Consistency | SR-002 — Accurate Maintenance History | BR-002 — Accurate Maintenance History |
| NFR-014 — Data Persistence | SR-002 — Accurate Maintenance History | BR-002 — Accurate Maintenance History |

## 5. Requirements Considerations

The non-functional requirements describe the expected characteristics of the proposed FleetPro system.

Some requirements will require specific technical measurements during System Design, Development and Testing.

For example, response time and system capacity should be measured during testing using defined test conditions rather than being assumed to meet the requirements.

The final technical implementation used to satisfy these requirements will be determined during the System Design and Development stages.

## 6. Conclusion

The non-functional requirements define the expected quality and operational characteristics of the FleetPro Vehicle Maintenance Management System.

The requirements address performance, security, usability, availability, reliability, scalability, maintainability and data integrity.

Together with the functional requirements, these requirements provide a more complete definition of the expected system.

The non-functional requirements will be used to guide the subsequent Business Rules, User Stories, Use Cases, Data Requirements, System Design, Development and Testing activities.