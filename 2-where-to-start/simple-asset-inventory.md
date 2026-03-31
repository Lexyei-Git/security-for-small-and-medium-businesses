# Simple asset inventory

A basic asset inventory is a **single, clear list of what you have**: devices, systems, applications and data that matter to your business.

You do not need a complex database or tool to start. A simple spreadsheet or table is enough and will make all other security work (including risk assessment, patching and access control) much easier.

---

## 1. What an asset inventory is (plain language)

In this guide, an **asset** is anything that:

- Stores, processes or transmits important business information, or  
- Is necessary for your day‑to‑day operations.

An **asset inventory** is just a structured list of these items with a few key details:

- What the asset is (name, type).  
- Where it is (location, cloud provider).  
- Who owns or is responsible for it.  
- How important it is to your business.

You can create and maintain this inventory in:

- A spreadsheet (for example, Excel, Google Sheets).  
- A simple asset management or IT documentation tool, if you already use one.

---

## 2. Types of assets to include

Start with the most important categories:

- **Devices (hardware)**
  - Laptops and desktops.  
  - Servers (on‑premises or hosted).  
  - Network equipment (routers, switches, firewalls, Wi‑Fi access points).  
  - Company‑managed mobile devices (phones, tablets).  
  - Other devices that store or process business data (for example, NAS, backup devices).

- **Systems and applications**
  - Email and collaboration platforms.  
  - File storage and sharing solutions (cloud and on‑premises).  
  - Line‑of‑business systems (ERP, CRM, accounting, HR).  
  - Customer‑facing systems (websites, e‑commerce, portals).  
  - Remote access and VPN solutions.

- **Data sets**
  - Customer databases.  
  - Financial and accounting records.  
  - HR and payroll data.  
  - Core operational data (orders, inventory, production, service delivery).

You do not need to capture every single file or device immediately. Focus first on assets that:

- Are **critical for operations**, or  
- Contain **sensitive data** (customer, financial, employee).

---

## 3. Suggested columns for a simple inventory

Below is a suggested set of columns for a starter spreadsheet:

| Column name          | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| Asset ID             | Simple unique identifier (for example, A001, S001)                         |
| Asset name           | Short, clear name (for example, “Finance laptop – Maria”, “CRM system”)    |
| Asset type           | Device, application, data set, network equipment, etc.                     |
| Location / hosting   | Office, data centre, cloud provider (for example, “Office – Vancouver”, “Microsoft 365”) |
| Owner / contact      | Person or role responsible for the asset                                   |
| Business function    | What part of the business it supports (for example, Finance, Sales, HR)    |
| Criticality          | Critical / Important / Nice‑to‑have                                        |
| Contains sensitive data? | Yes / No / Unknown                                                   |
| Internet‑facing?     | Yes / No                                                                   |
| Notes                | Any additional details (for example, model, key integrations)              |

You can add more columns over time (for example, software version, last patch date), but do not start with too many fields or the inventory will be hard to maintain.

---

## 4. How to build the first version

You can usually build a first version in a few short sessions:

1. **Start with what you know**
   - Ask IT or your service provider for:
     - A list of known devices and servers.  
     - A list of systems and cloud services in use.

2. **Talk to key departments**
   - Ask finance, sales, HR, operations:
     - “What systems do you use every day?”  
     - “Where do you store important files and data?”  
     - “Which tools would stop your work if they were down for a day or more?”

3. **Review subscriptions and invoices**
   - Look at financial records for:
     - Software subscriptions (SaaS, licenses).  
     - Hardware purchases and leases.  
     - IT and telecom contracts.

4. **Capture the top 20–50 assets first**
   - It is better to have a **short, accurate list** of key assets than a long, incomplete one.  
   - You can always expand later.

5. **Validate with stakeholders**
   - Review the list with relevant managers and IT to check for missing critical items or mistakes.

---

## 5. Keeping the inventory up to date

An inventory is only useful if it is reasonably current.

Simple practices:

- **Assign an owner**
  - Make one person or role responsible for maintaining the inventory (for example, IT lead, operations manager).

- **Link to onboarding and offboarding**
  - When new devices or systems are introduced, they must be added to the inventory.  
  - When assets are retired or decommissioned, they must be marked as such or removed.

- **Regular reviews**
  - Schedule a review at least **annually**, and ideally **quarterly**, to:
    - Add new assets.  
    - Update ownership and criticality.  
    - Remove or archive obsolete entries.

- **Use change triggers**
  - Update the inventory when:
    - You add a major new system or move to a new cloud service.  
    - You open or close an office.  
    - You go through a merger, acquisition or major restructuring.

---

## 6. How the asset inventory supports other activities

A simple, accurate asset inventory helps with:

- **Risk assessment**
  - Provides the list of assets you assess in `basic-risk-assessment.md`.

- **Patching and updates**
  - Tells you which systems and devices need regular updates and where they are.

- **Access control and account management**
  - Clarifies who owns each system and who should approve access.

- **Backup and recovery**
  - Identifies which data and systems must be backed up and restored first during incidents.

- **Vendor and third‑party risk**
  - Reveals which assets are provided or hosted by vendors and where additional controls or contracts are needed.

- **Incident response**
  - Helps you quickly understand which assets may be affected and who to involve.

In short, the inventory is a **foundation** for almost every other control in this repository.

---

## 7. Minimal checklist for a simple asset inventory

Use this checklist to see if you have a usable starter inventory:

- [ ] We maintain a written list (for example, spreadsheet) of our key devices, systems and data sets.  
- [ ] Each asset has a clear name, type and owner/contact.  
- [ ] We have identified which assets are critical, important or nice‑to‑have.  
- [ ] We have indicated which assets contain sensitive data and which are internet‑facing.  
- [ ] Someone is responsible for keeping the inventory up to date.  
- [ ] The inventory is reviewed and updated at least annually, and when major changes occur.  
- [ ] The inventory is used as an input for risk assessment, patching, backup planning and other security activities.

If several boxes are unchecked, start by building a short list of your top assets and expand over time, rather than waiting for a “perfect” inventory.
