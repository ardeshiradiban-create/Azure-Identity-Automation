# Microsoft Entra ID: Dynamic Group Automation & Troubleshooting

## Introduction
As an IT Professional with over 15 years of experience in infrastructure and support, I am currently specializing in Cloud Administration and preparing for the Microsoft Azure Administrator (AZ-104) certification.

This project demonstrates my ability to implement Attribute-Based Access Control (ABAC) within Microsoft Entra ID (formerly Azure AD). By moving away from manual user assignments to Dynamic Membership Groups, I've showcased how to streamline IT operations, reduce human error, and ensure that access is automatically granted based on a user's organizational role and location.

Problem Statement
Manual group management is inefficient and prone to security risks in growing organizations. For instance, in a company like Greenwall Companies, where I manage IT and project coordination, ensuring that only the right staff (e.g., IT personnel in Toronto) have specific access is critical.

Technical Implementation
In this repository, you will find a step-by-step walkthrough of:

Dynamic Group Configuration: Building complex logic using Rule Syntax.

Error Analysis & Troubleshooting: Investigating "Policy Restrictions" when manual overrides are attempted.

Identity Life-cycle Management: Automating the onboarding process by mapping user attributes (Job Title & City) to group memberships.

## Step-by-Step Implementation

### 1. Group Configuration
I created a Security group with a **Dynamic User** membership type to automate onboarding.
![Step 1](step1.png)

### 2. Defining Membership Rules
The rule ensures only users with the title "IT" in "Toronto" are added.
- **Rule Syntax:** `(user.jobTitle -eq "IT") and (user.city -eq "Toronto")`
![Dynamic Rule](step2.png)

### 3. Troubleshooting Manual Assignment Errors
When I tried to manually add a user, I encountered a policy restriction error. This confirms that the Dynamic Rule is governing the group correctly.
![Error Message](error.png)

## Conclusion
This project demonstrates my proficiency in **Azure Administration** and **Identity Governance**, skills I am currently applying in my role at **Greenwall Companies**.
