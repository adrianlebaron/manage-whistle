# 🧑‍💻 Release Notes WDA
 This page is intended for internal development and QA reference of **Whistle Drywall App**.  
*The emphasis at the end its to be able to search for the clickup card on the main searcher 
 Each task ID in parentheses corresponds to a ClickUp card. The “CU-” prefix is omitted to make the ID directly searchable in ClickUp’s global search bar.*

---

## 🧾 October 2025

**🧠 Improvements / Enhancements**

- Enabled searchable filter items within all dropdown filters on:
    - Invoices (**86b5gyvn4**)  
    - Worker Contracts (**86b6v61jm**)  
    - Bills (**86b6v4gbe**)  
    - Payments (**86b6v4gbe**)  
    - Teams (**86b6v4qd3**)  
    - Tasks (**86b6uwpkv**)  
- The sidebar menu items are now sorted alphabetically, making navigation more intuitive and consistent (**86b6q4wtv**).

**🐛 Bug Fixes / Resolved Issues**

- Fixed pagination styling in **Purchase Orders**. Page numbers now display correctly without overflowing (**86b6v7pxy**).  
- Fixed an issue where the printed **Bill PDF** incorrectly labeled the Payee section as “Worker.” Now, both Workers and Vendors are labeled as **Payee** (**86b6e2vqf**).

---

## 🧾 September 2025

**🚀 New Features**

- Added a **warning modal** in the **SML (Service Master List)** workflow when creating a Bill for items already associated with an existing Bill.  
  Lists each service linked to an existing Bill to prevent duplicate charges (**86b3qp0g9**).

**🧠 Improvements / Enhancements**

- **Percent Completed** field now allows decimals for SOV invoices (**86b5r0j0x**).  
- Added a **“Back to Filtered Bills”** link on the Payments subpage (**86b6bpnuu**).  
- Unified **Vendor** and **Worker** into a single **Payee** column (**86b6nv30j**).  
- Standardized **action buttons** across all modules (**86b5gyw5z**).

**🐞 Bug Fixes**

- Fixed metadata on **Bill PDF** pages — browser tab now shows “Bill” (**86b6e4uvg**).  
- Fixed **Teams** module 500 error when pressing Enter after search (**86b6fj963**).  
- Fixed multiple payment errors in **Invoices** module (**86b4nf5yh**).  
- Resolved **payment data alignment** issue (**86b4nf5yh**).

---

## 🧾 July 2025

**🚀 New Features**

- Added a **search bar** to the Invoice module (**86b4ng084**).  
- Enabled **searchable filter items** within dropdowns (**86b4ng084**).  
- Users can return to filtered **Bills** and **Invoices** after editing (**86b4nh11b**, **86b4ngqx8**).  
- Invoice number now displays at the top when editing (**86b4ngqx8**).

**🧠 Improvements / Enhancements**

- **Memo field** shows all text (**86b4ng084**).  
- **Client Contact** shows only company name (**86b4ng084**).  
- **Invoice table** shows full job names (**86b4ng084**).  
- Action buttons now consistent (**86b4ng084**).  
- Numbers display larger and clearer when editing (**86b4ngqx8**).  
- After saving invoice changes, user stays in editing interface (**86b4ngqx8**).  
- **Invoice exports** include all selected invoice data (**86b4ng5xe**).  
- **Payments** page includes Job column and filter (**86b4c8nru**).  
- **Bills** page includes Created By filter (**86b4gbehq**).

**🐛 Bug Fixes**

- **Excel & CSV exports** display correct totals (**86b4ng5xe**).  
- Fixed **Total Amount** issue when creating Bills from Time Entries (**86b4ydj10**).