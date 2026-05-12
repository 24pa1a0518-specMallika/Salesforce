# Formula Fields vs Validation Rules

## Overview

In Salesforce, Formula Fields and Validation Rules are powerful features used to automate calculations and enforce business logic.

- Formula Fields are used for automatic calculations and displaying derived values.
- Validation Rules are used to prevent users from entering invalid data.

---

# Formula Fields

## What is a Formula Field?

A Formula Field is a read-only field that automatically calculates its value based on other fields using formulas similar to Excel formulas.

Users cannot manually edit formula fields because Salesforce updates them automatically.

---

## Purpose of Formula Fields

- Perform automatic calculations
- Display dynamic values
- Reduce manual work
- Automate business calculations

---

## Examples of Formula Fields

### Total Amount Calculation

```text
Total Amount = Quantity * Price
```

### Full Name Formula

```text
FirstName & " " & LastName
```

### Discount Calculation

```text
Amount * 0.10
```

### IF Condition Example

```text
IF(Salary > 50000, "High", "Low")
```

---

## Characteristics of Formula Fields

- Read-only field
- Automatically calculated
- Cannot be edited manually
- Used for calculations and display purposes
- Updates automatically when related fields change

---

## When to Use Formula Fields

Use Formula Fields when:

- Automatic calculations are needed
- Values depend on other fields
- Users should not edit the value
- Dynamic information must be displayed

---

## Real-World Examples

### Banking Application

```text
Interest = Principal * Rate
```

### School Management System

```text
Percentage = Obtained Marks / Total Marks
```

---

# Validation Rules

## What is a Validation Rule?

A Validation Rule in Salesforce is used to prevent users from saving invalid or incorrect data.

If the validation condition evaluates to TRUE, Salesforce displays an error message and stops the record from being saved.

---

## Purpose of Validation Rules

- Restrict invalid data
- Enforce business rules
- Improve data quality
- Validate user input

---

## Examples of Validation Rules

### Prevent Negative Salary

```text
Salary__c < 0
```

Error Message:

```text
Salary cannot be negative
```

---

### Discount Limit Validation

```text
Discount__c > 20
```

Error Message:

```text
Discount cannot exceed 20%
```

---

### Age Restriction Validation

```text
Age__c < 18
```

Error Message:

```text
Must be 18 or older
```

---

## Characteristics of Validation Rules

- Prevents invalid records from being saved
- Displays custom error messages
- Used for enforcing restrictions
- Maintains data accuracy and consistency

---

## When to Use Validation Rules

Use Validation Rules when:

- Invalid data must be prevented
- Business restrictions should be enforced
- Certain conditions must be validated
- Mandatory checks are required

---

## Real-World Examples

### Banking System

```text
Loan Amount cannot exceed ₹10 Lakhs
```

### School Management System

```text
Attendance must be above 75%
```

---

# Difference Between Formula Fields and Validation Rules

| Formula Fields | Validation Rules |
|---|---|
| Used for calculations | Used for restrictions |
| Automatically generates values | Prevents invalid data |
| Read-only | Displays error messages |
| Does not stop record save | Stops record save |
| Used for automation | Used for validation |

---

# Key Point

- Use **Formula Fields** to calculate values automatically.
- Use **Validation Rules** to prevent users from entering incorrect data.

---

# Conclusion

Formula Fields and Validation Rules are essential Salesforce features used to automate calculations and maintain high-quality data.

- Formula Fields help generate dynamic values automatically.
- Validation Rules help enforce business logic and prevent incorrect data entry.
