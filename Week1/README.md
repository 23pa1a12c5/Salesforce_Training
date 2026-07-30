# Day 3 Salesforce Training

## Project Title
Placement Management System Automation using Salesforce Flow and Validation Rules

---

## Objective

The objective of this assignment is to automate the Placement Management System using Salesforce declarative tools such as Record-Triggered Flows and Validation Rules.

---

## Tasks Completed

### Flow Automation

#### Flow 1 – Auto Set Application Date
- Type: Record-Triggered Flow
- Trigger: When a new Application record is created.
- Action:
  - Automatically sets the Application Date to the current date.

#### Flow 2 – Send Confirmation Email
- Type: Record-Triggered Flow
- Trigger: When a new Application record is created.
- Action:
  - Sends a confirmation email after the application is submitted.

#### Flow 3 – Auto Create Offer Letter
- Type: Record-Triggered Flow
- Trigger: When the Application Status is "Selected".
- Action:
  - Automatically creates an Offer Letter record.
  - Copies Student, Application, Company Name, Offer Date, and Salary into the Offer Letter.

---

## Validation Rules Implemented

### 1. Validate Student CGPA
Ensures that the student's CGPA is greater than or equal to the minimum CGPA required.

### 2. Validate Application Date
Prevents users from entering an Application Date that is later than the Job Closing Date.

### 3. Mandatory Fields Check
Ensures that mandatory fields such as Student and Company Name are not left blank.

---

# README Questions

## 1. Which requirements did you solve using Flow?

The following requirements were implemented using Salesforce Record-Triggered Flows:

- Automatically set the Application Date.
- Automatically create an Offer Letter when the application status becomes "Selected".
- Send a confirmation email after an application is submitted.

---

## 2. Which requirements required Validation Rules?

Validation Rules were used to enforce business constraints:

- Student CGPA must be greater than or equal to the minimum CGPA.
- Application Date cannot be after the Job Closing Date.
- Mandatory fields cannot be left blank.

---

## 3. Which requirements still needed Apex?

No Apex was required for this assignment because all required business logic was successfully implemented using Salesforce declarative tools such as Flows and Validation Rules.

If future requirements involve complex calculations, integrations, or bulk processing, Apex can be used.

---

## 4. Why did you choose those solutions?

Flows were chosen because they automate business processes without writing code and are recommended for declarative automation in Salesforce.

Validation Rules were used to prevent invalid data from being saved and to ensure data quality.

These solutions improve automation, maintain data integrity, and reduce manual work while following Salesforce best practices.

---
