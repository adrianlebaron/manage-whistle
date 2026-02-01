#  Release Notes Whistle Drywall App
This page is intended for internal development and QA reference of **Whistle Drywall App**.

---

# December 2025 Release Notes – Whistle Drywall App (Internal)

## 🐛 Bugs / Resolved Issues
- **Worker Contracts – Job Dropdown**  
  Fixed an issue where admin users could not change the job from the dropdown when editing a worker contract. Job names containing apostrophes no longer prevent updates from being saved.  
  [CU-86b2j1cdk](https://app.clickup.com/t/86b2j1cdk)

- **Billing – Edit Bill Item with Apostrophes**  
  Fixed an issue where bill items with apostrophes (') in the service name could not be edited after creation. Special characters in bill item names are now handled correctly, allowing items to be modified without errors.  
  [CU-86b5tf4rn](https://app.clickup.com/t/86b5tf4rn)

## 🧠 Improvements / Enhancements
- **Change Order Requests – Bulk Selection Across Pages**  
  Enhanced the Change Order Request module so users can select multiple COR items across different pages. Selected items now persist when navigating between pages, allowing bulk actions to be completed without losing previous selections.  
  [CU-86b7cx1wp](https://app.clickup.com/t/86b7cx1wp)

- **Change Order Requests – Email Attachment Preview (Bulk Send)**  
  Enhanced the COR bulk email preview so that when multiple CORs are selected, all corresponding attachment links are displayed in the Attachments section. Previously, only one attachment link appeared in the preview, even when multiple CORs were included.  
  [CU-86b71gbgw](https://app.clickup.com/t/86b71gbgw)

## 🚀 New Features
- **Jobs Module – UI & Workflow Redesign**  
  Introduced a redesigned Jobs module with a new table-based landing page, replacing the previous card layout. The new view improves scalability and visibility by displaying key job details such as Job Name, City, Start Date, Deadline, and Status, along with global search, pagination, and adjustable page size for easier navigation across large job lists.  
  Each job row now includes a single Actions button that reveals available job actions (View, View SML, View PML, View SOV), keeping the interface clean while maintaining quick access to key job views.  
  The job detail experience was redesigned with improved navigation across **Overview, Timeline, Geofence, Financials, and Documents**. Tags are now more interactive, supporting better organization and filtering across the app.  
  A persistent timeline panel is displayed on the right side of the job view, providing continuous visibility into schedule, progress, key dates, status, and phase. An **Upcoming Items** section at the bottom of the timeline allows users to add and track upcoming milestones or inspections.  
  A new **Financials** interface provides a consolidated view of cost codes, budget summaries, invoices, and supports creating invoices and purchase orders directly within a job.  
  A new **Documents** interface centralizes project files, supporting uploads of PDFs, images, and documents. Files are organized into system folders such as Plans, Permits, Contracts, Photos, RFIs & Submittals, Correspondence, Reports, Inspections, Safety & Compliance, and Meeting Notes, with search and filtering for easier access.  
  [CU-86b4x870x](https://app.clickup.com/t/86b4x870x)

- **Time & Material (T&M) Module – Web App Availability**  
  Introduced the Time & Material (T&M) module to the Web App, making it easier to track and manage items that were previously only available through the Mobile App, which was the sole place to create T&M records.  
  The T&M workflow allows users to create a T&M record, select a project, add descriptions and reasons for work performed, and include labor, materials, equipment, photos, and files. The module supports a signing flow where the Foreman signs first, followed by the Superintendent via a secured link.  
  Once both signatures are completed, users can generate a Change Order Request (COR) directly from the T&M record.  
  [CU-86b29r13y](https://app.clickup.com/t/86b29r13y)

- **Ability to Create a Bill from Purchase Order**  
  Added the ability to create a Bill directly from a selected Purchase Order. When converting a PO to a Bill, each product line item from the purchase order is automatically converted into a corresponding bill item.  
  Pricing for each bill item is populated from the product summary, improving accuracy and providing a clearer record of materials received and paid for based on supplier invoices.  
  [CU-86b2ph7rw](https://app.clickup.com/t/86b2ph7rw)

- **Reporting Module – Performance & Workflow Redesign (Admin Users)**  
  Redesigned the Reporting module for admin users to improve performance, accuracy, and usability. Page load times and filter interactions were significantly optimized, reducing delays when applying filters, approvals, or creating new entries.  
  The hours workflow was simplified by removing the separate Extra Hours approval feature. Extra Hours are now included directly in the total Hours calculation. A new **Paid Hours** column was added, allowing admin users to explicitly define the number of hours to be paid.  
  When creating Bills from selected records, the system now uses **Paid Hours** as the source of truth, even when the value is zero or left blank.  
  The **Generate Report** feature was updated to include the new columns, and calculations were reviewed and corrected to ensure consistency between hours and cost values.  
  [CU-86b5xyax3](https://app.clickup.com/t/86b5xyax3)

- **Ability to Create Tasks from SML**  
  Added the ability to create tasks directly from selected Schedule of Materials and Labor (SML) line items. From the SML view, users can select one or more items and choose **Create Task**, generating a task for each selected line item.  
  Tasks are automatically associated with the corresponding service item. If a matching tag exists, it is applied to the task; otherwise, a new tag is created based on the service item.  
  [CU-86b2ph89m](https://app.clickup.com/t/86b2ph89m)


---
---

# October 2025 Release Notes – Whistle Drywall App (Internal)

## 🚀 New Features

- **Added search functionality** to the **Job** and **Vendor** dropdown fields when creating a **Purchase Order**. 
  This improvement helps users quickly find entries without having to scroll through long lists, especially on mobile and tablet devices.  
  (<a href="https://app.clickup.com/t/86b734e8p" target="_blank" rel="noopener noreferrer">CU-86b734e8p</a>)

- **Added the ability** to create a **Bill** directly from a **Purchase   Order (PO)**. 
  This allows users to convert a selected PO into a Bill, automatically generating Bill items from the PO’s product list, ensuring accurate cost tracking and smoother transition from ordered to billed materials..  
  (<a href="https://app.clickup.com/t/86b2ph7rw" target="_blank" rel="noopener noreferrer">CU-86b2ph7rw</a>)



## 🧠 Improvements / Enhancements

- Enabled **searchable filter items** within all dropdown filters on:  
  **Invoices** ([CU-86b5gyvn4](https://app.clickup.com/t/86b5gyvn4))  
  **Worker Contracts** ([CU-86b6v61jm](https://app.clickup.com/t/86b6v61jm))  
  **Bills** ([CU-86b6v4gbe](https://app.clickup.com/t/9014528152/86b6v4gbe))  
  **Payments** ([CU-86b6v4gbe](https://app.clickup.com/t/9014528152/86b6v4gbe))  
  **Teams** ([CU-86b6v4qd3](https://app.clickup.com/t/9014528152/86b6v4qd3))  
  **Tasks** ([CU-86b6uwpkv](https://app.clickup.com/t/9014528152/86b6uwpkv))


- The **sidebar menu items** are now sorted alphabetically, making navigation more intuitive and consistent.  
  (<a href="https://app.clickup.com/t/9014528152/86b6q4wtv" target="_blank" rel="noopener noreferrer">CU-86b6q4wtv</a>)

- Updated the **User Management** page to include **activity tracking** from the **mobile app** (iOS and Android). Previously, “Last Active” data only registered web sessions, causing mobile usage to appear inactive. 
This improvement ensures admin users can now accurately monitor both web and mobile app activity.  
  (<a href="https://app.clickup.com/t/86b5g8fbg" target="_blank" rel="noopener noreferrer">CU-86b5g8fbg</a>)

- Added **Account Settings** and **Logout buttons** to the **mobile web navigation bar**, ensuring users can easily access account options and sign out when using the app through a mobile browser or tablet.  
  (<a href="https://app.clickup.com/t/86b736mdw" target="_blank" rel="noopener noreferrer">CU-86b736mdw</a>)



## 🐛 Bug Fixes / Resolved Issues

- Fixed **pagination styling** in Purchase Orders. When there are many pages, the page numbers now display correctly without overflowing off-screen.  
  (<a href="https://app.clickup.com/t/9014528152/86b6v7pxy" target="_blank" rel="noopener noreferrer">CU-86b6v7pxy</a>)

- **Fixed** an issue where the printed **Bill PDF** incorrectly labeled the **Payee** section as “Worker.” Now, both Workers and Vendors are consistently labeled as Payee to maintain uniformity across all printed bills.   
  (<a href="https://app.clickup.com/t/9014528152/86b6e2vqf" target="_blank" rel="noopener noreferrer">CU-86b6e2vqf</a>)

- Fixed an issue where Vendor contacts could not be edited if the associated Job name contained an apostrophe (’).   
  (<a href="https://app.clickup.com/t/86b5tfm3y" target="_blank" rel="noopener noreferrer">CU-86b5tfm3y</a>)

---

# August/September  2025 Release Notes – Whistle Drywall App (Internal)

## 🚀 New Features

- **Added** a **warning modal** in the **SML** (Service Master List) workflow when attempting to create a **Bill** for items that are already associated with an **existing** Bill. 
The system now displays a detailed message listing each service linked to an existing Bill, helping prevent duplicate charges and ensuring accurate billing.  
  (<a href="https://app.clickup.com/t/9014528152/86b3qp0g9" target="_blank" rel="noopener noreferrer">CU-86b3qp0g9</a>)

## 🧠 Improvements / Enhancements

- **Action buttons** now consistent **across** all modules.  
  (<a href="https://app.clickup.com/t/86b5gyw5z" target="_blank" rel="noopener noreferrer">CU-86b5gyw5z</a>)

- **Percent Completed** field now **allows** decimal values when **editing invoices** created from an **SOV**, providing more accurate progress tracking.  
  (<a href="https://app.clickup.com/t/9014528152/86b5r0j0x" target="_blank" rel="noopener noreferrer">CU-86b5r0j0x</a>)

- Added a **“Back to Filtered Bills”** link within the Payments subpage of the Bills module. 
  When a user filters bills, selects one to view or edit, and then opens the Payments section inside that bill, they can now easily return to their previously filtered bills list without losing their filter context.  
  (<a href="https://app.clickup.com/t/9014528152/86b6bpnuu" target="_blank" rel="noopener noreferrer">CU-86b6bpnuu</a>)

- **Combine Vendor** and **Worker** columns into a single unified column called **Payee**. 
  This change simplifies data presentation across the app by showing a single payee entity, whether it’s a vendor or a worker.  
  (<a href="https://app.clickup.com/t/9014528152/86b6nv30j" target="_blank" rel="noopener noreferrer">CU-86b6nv30j</a>)

## 🐛 Bug Fixes / Resolved Issues

- **Fixed** incorrect **metadata** on **Bill PDF** pages — the **browser tab** now **correctly** displays “Bill” instead of “Purchase Order.”
  (<a href="https://app.clickup.com/t/9014528152/86b6e4uvg" target="_blank" rel="noopener noreferrer">CU-86b6e4uvg</a>)

- **Fixed** an issue in the **Teams module** where pressing **Enter** after using the search box caused a 500 error. The search action now works correctly without triggering an error.
  (<a href="https://app.clickup.com/t/9014528152/86b6fj963" target="_blank" rel="noopener noreferrer">CU-86b6fj963</a>)

- **Fixed** an issue in the **Invoices** module where **adding** multiple **payments** caused an error — after adding the first payment, additional payments couldn’t be added.
  (<a href="https://app.clickup.com/t/9014528152/86b4nf5yh" target="_blank" rel="noopener noreferrer">CU-86b4nf5yh</a>) 

- **Fixed** a data shift issue that occurred when **editing payments**. The payment details (date, description, created by, and action buttons) now remain **correctly** aligned after saving multiple payments.
  (<a href="https://app.clickup.com/t/9014528152/86b4nf5yh" target="_blank" rel="noopener noreferrer">CU-86b4nf5yh</a>)

---

# July 2025 Release Notes – Whistle Drywall App (Internal)

## 🚀 New Features

- Added a **search bar** to Invoice module to quickly locate invoices.  
  (<a href="https://app.clickup.com/t/9014528152/86b4ng084" target="_blank" rel="noopener noreferrer">CU-86b4ng084</a>)

- Added **searchable filters** items within dropdown filters on invoice module.  
  (<a href="https://app.clickup.com/t/9014528152/86b4ng084" target="_blank" rel="noopener noreferrer">CU-86b4ng084</a>)

- Added **back to previews filtered bills link** when editing one bill.
  (<a href="https://app.clickup.com/t/9014528152/86b4nh11b" target="_blank" rel="noopener noreferrer">CU-86b4nh11b</a>)

- **Excel & CSV exports** show correct totals.  
  (<a href="https://app.clickup.com/t/9014528152/86b4ng5xe" target="_blank" rel="noopener noreferrer">CU-86b4ng5xe</a>)

## 🧠 Improvements / Enhancements

  - Invoice number now shows at top when editing.  
  (<a href="https://app.clickup.com/t/9014528152/86b4ngqx8" target="_blank" rel="noopener noreferrer">CU-86b4ngqx8</a>)

  - The memo field on invoices now showing all available source text.
   (<a href="https://app.clickup.com/t/9014528152/86b4ng084" target="_blank" rel="noopener noreferrer">CU-86b4ng084</a>)

  - On invoices Client Contact field now displays only the Client (Company name). 
    (<a href="https://app.clickup.com/t/9014528152/86b4ng084" target="_blank" rel="noopener noreferrer">CU-86b4ng084</a>)

  - On invoices table now displays the entire job name. 
    (<a href="https://app.clickup.com/t/9014528152/86b4ng084" target="_blank" rel="noopener noreferrer">CU-86b4ng084</a>)

  - When editing an invoice now shows bigger readable numbers.   
    (<a href="https://app.clickup.com/t/9014528152/86b4ngqx8" target="_blank" rel="noopener noreferrer">CU-86b4ngqx8</a>)

  - When saving changes on invoices now the user stays on the editing interface.
    (<a href="https://app.clickup.com/t/9014528152/86b4ngqx8" target="_blank" rel="noopener noreferrer">CU-86b4ngqx8</a>) 

  - On invoices exports for an excel and CVS files are now including all data related to the selected invoices for an export. 
    (<a href="https://app.clickup.com/t/9014528152/86b4ng5xe" target="_blank" rel="noopener noreferrer">CU-86b4ng5xe</a>)   
  
  - The Payments page now includes a Job column and a Job filter, improving tracking and filtering of payments. 
    (<a href="https://app.clickup.com/t/9014528152/86b4c8nru" target="_blank" rel="noopener noreferrer">CU-86b4c8nru</a>) 

  - The Bills page now includes a Created By filter to make locating bills by their creator easier.
    (<a href="https://app.clickup.com/t/9014528152/86b4gbehq" target="_blank" rel="noopener noreferrer">CU-86b4gbehq</a>)   

## 🐛 Bug Fixes / Resolved Issues 

  - Excel and CVS exports are now providing the correct invoice total.
    (<a href="https://app.clickup.com/t/9014528152/86b4ng5xe" target="_blank" rel="noopener noreferrer">CU-86b4ng5xe</a>)

  - Fixed an issue when selecting a bill on the Total Amount was not displaying correctly on the Bill module when creating Bills from Time Entries.
    (<a href="https://app.clickup.com/t/9014528152/86b4ydj10" target="_blank" rel="noopener noreferrer">CU-86b4ydj10</a>) 