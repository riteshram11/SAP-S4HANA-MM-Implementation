# SAP S/4HANA Materials Management (MM) Implementation Project

This repository documents an end-to-end hands-on project covering enterprise configuration, Procure-to-Pay (P2P) automation, special stock processes, value/quantity contracts, and MRP Live execution in SAP S/4HANA.

📄 **Full Project Document:** [Download SAP Project PDF](./SAP%20PROJECT%20FINAL%20DRAFT%20RITESH%20RAM.pdf)

---

## 🛠️ Tech Stack & Systems
* **ERP System:** SAP S/4HANA
* **Interfaces:** SAP GUI & SAP Fiori (My Inbox, Manage Purchase Orders)
* **Core Modules:** SAP MM (Materials Management), Integration with FI/CO & PP

---

## 📋 Key Scenarios Configured & Executed

### 1. Enterprise Structure & Master Data Configuration
* **Enterprise Structure:** Created Plant `Y015` (copied from `1010`), Storage Locations (`101A`, `101C`), and Purchasing Organization `P015` mapped to Company Code `1010`.
* **Master Data:** Created Product Master `T-RC15`, Business Partner `SP-C15`, Purchasing Info Records with price scales, and Source Lists.

### 2. Procure-to-Pay (P2P) Process & Flexible Workflows
* **Purchase Requisition & Order:** Created stock and cost-center PRs/POs (`ME51N`, `ME21N`).
* **Flexible Workflow:** Configured PO approval thresholds (> €5,000) and approved release via **SAP Fiori My Inbox**.
* **Logistics & Financial Settlement:** Executed Goods Receipt (`MIGO`), Invoice Parking (`MIRO` / `MIR6`), and posted unplanned delivery costs.

### 3. Special Procurement & Stock Types
* **Subcontracting:** Processed Subcontracting PO (`T-FL4A15`), components movement (`541`), direct delivery components, and final assembly receipt (`101`/`543`).
* **GR Blocked & Quality Stock:** Received stock into GR Blocked Stock (`103`), released to Quality Inspection (`105`), and transferred to Unrestricted Use (`321`).

### 4. Contracts & Material Requirements Planning (MRP Live)
* **Contracts:** Set up Value Contract (`ME31K` type `WK`) and Quantity Contract (`MK`).
* **MRP Live (`MD01N`):** Executed automated planning runs using MRP-relevant Source Lists mapped to active contracts for automated purchase requisition generation.

---

## 🎯 Key T-Codes Used
`SPRO` | `BP` | `MM01` | `ME11` | `ME51N` | `ME21N` | `MIGO` | `MIRO` | `MIR6` | `ME31K` | `MD01N`# SAP-S4HANA-MM-Implementation
