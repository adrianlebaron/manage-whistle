#  Release Notes Whistle Drywall App
This page is intended for internal development and QA reference of **Whistle Drywall App**.

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

## August/September  2025 Release Notes – Whistle Drywall App (Internal)

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

## July 2025 Release Notes – Whistle Drywall App (Internal)

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