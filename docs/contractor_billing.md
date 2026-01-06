# Contractor Billing Module - User Guide

**Date:** 31-12-2025  
**Contact:** support@factri.ai

---
### What is the Contractor Billing Module?

The Contractor Billing Module helps you track payments to external contractors who perform work on the production lines. When production work is completed and confirmed, the system automatically calculates how much to pay each contractor based on your pre-configured rates.

---

### How Does Billing Work?

Automatic Billing

You don't need to manually create billing entries. The system does it automatically when:

1. An operator confirms that work is complete on a production line
2. The system checks which contractors are assigned to that line
3. Billing entries are created based on your configured rates

### How is the Billing Amount Decided?

The billing amount comes directly from the Work Code you set up. Each Work Code has a fixed price, and this price is used whenever that type of work is confirmed.

*Example: If "Casting Inspection" Work Code has a price of ₹1,250, every time casting inspection work is confirmed, the contractor receives ₹1,250.*

## Key Terms Explained

### Part Family

**What it is:** A category that groups similar types of materials together for billing purposes.

**Why it matters:**
- Helps organize which billing rates apply to which materials
- Materials in the same Part Family use the same set of Work Codes

*Examples: Casting Parts, Machined Components, Assembly Items*

**Important Rule:** Each material can only belong to ONE Part Family.

---
### Material Family Assignment

**What it is:** The link between a specific material and its Part Family.

**Why it matters:**
- Tells the system which Part Family a material belongs to
- Without this assignment, no billing will be generated for that material

**How to use:** Go to Material Family Assignment and select which Part Family each material belongs to.

---
### Work Code

**What it is:** A specific type of billable work with a set price.

Key Information in a Work Code:

| Field           | What it means                                            |
|-----------------|----------------------------------------------------------|
| Work Code       | A unique code to identify this work type                 |
| Job Description | A clear name for the work being done                     |
| Weight (KG)     | The standard weight for this work (for reference)        |
| Man Hours       | How many hours this work typically takes (for reference) |
| Price           | The amount that will be billed                           |
| Part Family     | Which category of materials this applies to              |

**Why it matters:** The Price in the Work Code is what gets charged to the contractor's account.

**Important Rule:** Each Work Code must have a unique code name.

---
### Contractor

**What it is:** An external company or individual who performs work and receives payment.

Key Information for a Contractor:

| Field         | What it means                                   |
|---------------|-------------------------------------------------|
| Code          | A unique identifier for the contractor          |
| Name          | The contractor's full name or company name      |
| Contact Phone | Phone number (optional)                         |
| Contact Email | Email address (optional)                        |
| Plant         | Which plant this contractor works at (optional) |

**Important Rule:** Each contractor must have a unique code.

---
### Production Line

**What it is:** A physical location in your facility where work is performed.

**Why it matters:** Billing is based on which line the work was done on. Different lines can have different contractors assigned.

---
### Line-Work Code-Contractor Mapping

**What it is:** The main configuration that connects everything together. It answers: "Which contractor gets paid for which type of work on which line?"

**How it works:**

| You set up... | To define...                          |
|---------------|---------------------------------------|
| Line          | Where the work happens                |
| Work Code     | What type of work (and at what price) |
| Contractor    | Who gets paid                         |

Example:
- Line: "Assembly Line 1"
- Work Code: "Final Inspection" (₹500)
- Contractor: "ABC Quality Services"

*This means: When final inspection is confirmed on Assembly Line 1, ABC Quality Services gets billed ₹500.*

**Important Rules:**
- You cannot have duplicate mappings (same line + same work code + same contractor)
- One contractor can be assigned to multiple lines
- One line can have multiple contractors (for different types of work)

---
### Billing Entry

**What it is:** A record of money owed to a contractor for completed work.

What it contains:

| Field          | What it means               |
|----------------|-----------------------------|
| Contractor     | Who is being paid           |
| Work Code      | What work was done          |
| Billing Amount | How much is owed            |
| Billing Date   | When the work was completed |

**Important:** Billing entries are created automatically. You do not create them manually.

---
### How Everything Connects

Step 1: SET UP (Do this once)
````
Create Part Families
        ↓
Assign Materials to Part Families
        ↓
Create Work Codes with Prices
        ↓
Create Contractors
        ↓
Create Mappings (Line + Work Code + Contractor)
````


Step 2: DAILY OPERATIONS (Happens automatically)
````
Operator confirms work on a line
        ↓
System finds the material's Part Family
        ↓
System finds matching mappings
        ↓
Billing entries are created automatically
````

---
## Reports Available

| Report             | What it shows                                       |
|--------------------|-----------------------------------------------------|
| Contractor Summary | Total billing for each contractor over a date range |
| Monthly Summary    | Month-by-month breakdown of all billing             |
| Audit Log          | History of all changes made to billing records      |

### Exporting Data

You can download billing data in two formats:
- Excel (.xlsx) - Opens in Microsoft Excel or Google Sheets
- CSV (.csv) - Opens in any spreadsheet application

Exports include all related information: contractor details, work performed, materials, and production line.

---
## Change Tracking

The system keeps a complete record of all changes:
- Who made the change
- When it was made
- What was changed (old value and new value)

This applies to:
- Work Code prices
- Contractor assignments
- Billing entries

---
## Quick Reference: Important Rules

| Rule                                                     | Why it matters                                  |
|----------------------------------------------------------|-------------------------------------------------|
| Each material can only be in ONE Part Family             | Ensures clear billing categorization            |
| Each Work Code must be unique                            | Prevents confusion in billing                   |
| Each Contractor Code must be unique                      | Ensures accurate payment tracking               |
| Line + Work Code + Contractor combination must be unique | Prevents duplicate billing                      |
| Changing a Work Code price only affects future billing   | Past billing entries keep their original amount |

---