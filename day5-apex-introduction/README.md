# Day 5 – Apex Introduction

## 1. What is Apex?
Apex is a programming language developed by Salesforce. It is used to add custom business logic and automation inside Salesforce applications. Apex is similar to Java and runs on the Salesforce platform.

---

## 2. Difference Between Flow and Apex

| Flow | Apex |
|------|------|
| No-code or low-code tool | Full programming language |
| Easy to create using drag and drop | Requires coding knowledge |
| Best for simple automation | Best for complex logic |
| Faster to develop | More flexible and powerful |
| Used by admins | Used by developers |

### Configuration vs Coding

#### Configuration
Configuration means customizing Salesforce using clicks instead of code.
Examples:
- Creating objects
- Validation rules
- Flows

#### Coding
Coding means writing programs to implement advanced logic.
Examples:
- Apex classes
- Triggers
- Custom integrations

---

## 3. Real Examples Where Apex Is Needed

### Example 1
Automatically calculate scholarship eligibility based on student marks and attendance.

### Example 2
Integrate Salesforce with an external payment gateway or college website.

### Example 3
Send custom notifications and generate reports when fee payments are delayed.

---

## 4. Integrated System Design – College Management System

### CRM
Salesforce CRM helps manage students, faculty, courses, attendance, and fee details in one system.

### Objects
Custom objects used:
- Student
- Faculty
- Course
- Attendance
- Fee

### Relationships
- One student can enroll in many courses.
- One faculty member can teach multiple courses.
- Attendance records are linked to students.

### Validation
Validation rules ensure proper data entry.
Examples:
- Phone number must contain 10 digits.
- Attendance percentage cannot exceed 100.

### Flow
Flows automate tasks such as:
- Sending fee reminders
- Creating attendance records
- Sending welcome emails to students

### Apex
Apex handles advanced business logic such as:
- Automatic grade calculation
- Scholarship eligibility processing
- External system integrations

---

## 5. Pseudocode Examples

### Example 1 – Attendance Check

IF attendance < 75%
THEN send warning email to student

### Example 2 – Fee Reminder

IF fee status = unpaid
THEN send reminder notification

### Example 3 – Grade Calculation

IF marks >= 90
THEN grade = A
ELSE IF marks >= 75
THEN grade = B
ELSE grade = C

---

## 6. Reflection

Enterprise systems eventually need programming because business requirements become more complex over time. Simple configuration tools may not handle advanced logic, integrations, security, or custom automation. Programming languages like Apex help developers build scalable, flexible, and efficient enterprise applications.
