# 🧑‍💻 Release Notes WDA
 This page is intended for internal development and QA reference of **Whistle Drywall App**.  
*The emphasis at the end its to be able to search for the clickup card on the main searcher 
 Each task ID in parentheses corresponds to a ClickUp card. The “CU-” prefix is omitted to make the ID directly searchable in ClickUp’s global search bar.*

---

# 🧾 October 2025 Release Notes – Whistle Drywall App (Internal)

## 🚀 New Features

- Added search functionality to the **Job** and **Vendor** dropdown fields when creating a **Purchase Order**.  
  This improvement helps users quickly find entries without having to scroll through long lists, especially on mobile and tablet devices.  
  A clickable search icon (🔎) has been added, and the feature supports instant search that updates results as users type or delete characters.  
  ([CU-86b734e8p](https://app.clickup.com/t/86b734e8p "View ClickUp Task"))

- Added the ability to **create a Bill directly from a Purchase Order (PO)**.  
  This allows users to convert a selected PO into a Bill, automatically generating Bill items from the PO’s product list — ensuring accurate cost tracking and a smoother transition from ordered to billed materials.  
  ([CU-86b2ph7rw](https://app.clickup.com/t/86b2ph7rw "View ClickUp Task"))

---

## 🧠 Improvements / Enhancements

- Enabled searchable filter items within all dropdown filters on:
  - Invoices ([CU-86b5gyvn4](https://app.clickup.com/t/86b5gyvn4 "View ClickUp Task"))
  - Worker Contracts ([CU-86b6v61jm](https://app.clickup.com/t/86b6v61jm "View ClickUp Task"))
  - Bills ([CU-86b6v4gbe](https://app.clickup.com/t/9014528152/86b6v4gbe "View ClickUp Task"))
  - Payments ([CU-86b6v4gbe](https://app.clickup.com/t/9014528152/86b6v4gbe "View ClickUp Task"))
  - Teams ([CU-86b6v4qd3](https://app.clickup.com/t/9014528152/86b6v4qd3 "View ClickUp Task"))
  - Tasks ([CU-86b6uwpkv](https://app.clickup.com/t/9014528152/86b6uwpkv "View ClickUp Task"))

- The **sidebar menu items** are now sorted alphabetically, making navigation more intuitive and consistent.  
  ([CU-86b6q4wtv](https://app.clickup.com/t/9014528152/86b6q4wtv "View ClickUp Task"))

- Updated the **User Management** page to include activity tracking from the mobile app (iOS and Android).  
  Previously, “Last Active” data only registered web sessions, causing mobile usage to appear inactive.  
  This improvement ensures admin users can now accurately monitor both web and mobile app activity.  
  ([CU-86b5g8fbg](https://app.clickup.com/t/86b5g8fbg "View ClickUp Task"))

- Added **Account Settings** and **Logout** buttons to the **mobile web navigation bar**, ensuring users can easily access account options and sign out when using the app through a mobile browser or tablet.  
  ([CU-86b736mdw](https://app.clickup.com/t/86b736mdw "View ClickUp Task"))

---

## 🐛 Bug Fixes / Resolved Issues

- Fixed **pagination styling** in Purchase Orders.  
  When there are many pages, the page numbers now display correctly without overflowing off-screen.  
  ([CU-86b6v7pxy](https://app.clickup.com/t/9014528152/86b6v7pxy "View ClickUp Task"))

- Fixed an issue where the printed **Bill PDF** incorrectly labeled the Payee section as “Worker.”  
  Now, both Workers and Vendors are consistently labeled as **Payee** to maintain uniformity across all printed bills.  
  ([CU-86b6e2vqf](https://app.clickup.com/t/9014528152/86b6e2vqf "View ClickUp Task"))

- Fixed an issue where **Vendor contacts** could not be edited if the associated Job name contained an apostrophe (’).  
  This resolves similar errors previously seen in other modules (**Bills, Worker Contracts, Time > Clock In, and Email Invoices**) when handling special characters in Job names.  
  ([CU-86b5tfm3y](https://app.clickup.com/t/86b5tfm3y "View ClickUp Task"))

---

## 🧾 September/August 2025

**🚀 New Features**

- Added a **warning modal** in the **SML (Service Master List)** workflow when creating a Bill for items already associated with an existing Bill.  
  Lists each service linked to an existing Bill to prevent duplicate charges ([CU-86b3qp0g9](https://app.clickup.com/t/9014528152/86b3qp0g9 "View ClickUp Task")).

**🧠 Improvements / Enhancements**

- Action buttons now consistent across all modules ([CU-86b5gyw5z](https://app.clickup.com/t/86b5gyw5z "View ClickUp Task")).
- **Percent Completed** field now allows decimals for SOV invoices ([CU-86b5r0j0x](https://app.clickup.com/t/9014528152/86b5r0j0x "View ClickUp Task")).  
- Added a **“Back to Filtered Bills”** link on the Payments subpage ([CU-86b6bpnuu](https://app.clickup.com/t/9014528152/86b6bpnuu "View ClickUp Task")).  
- Unified **Vendor** and **Worker** into a single **Payee** column ([CU-86b6nv30j](https://app.clickup.com/t/9014528152/86b6nv30j "View ClickUp Task")).  
- Standardized **action buttons** across all modules ([CU-86b5gyw5z](https://app.clickup.com/t/9014528152/86b5gyw5z "View ClickUp Task")).

**🐞 Bug Fixes**

- Fixed metadata on **Bill PDF** pages — browser tab now shows “Bill” ([CU-86b6e4uvg](https://app.clickup.com/t/9014528152/86b6e4uvg "View ClickUp Task")).  
- Fixed **Teams** module 500 error when pressing Enter after search ([CU-86b6fj963](https://app.clickup.com/t/9014528152/86b6fj963 "View ClickUp Task")).  
- Fixed multiple payment errors in **Invoices** module ([CU-86b4nf5yh](https://app.clickup.com/t/9014528152/86b4nf5yh "View ClickUp Task")).  
- Resolved **payment data alignment** issue ([CU-86b4nf5yh](https://app.clickup.com/t/9014528152/86b4nf5yh "View ClickUp Task")).

---

## 🧾 July 2025

**🚀 New Features**

- Added a **search bar** to the Invoice module ([CU-86b4ng084](https://app.clickup.com/t/9014528152/86b4ng084 "View ClickUp Task")).  
- Enabled **searchable filter items** within dropdowns on Invoice module ([CU-86b4ng084](https://app.clickup.com/t/9014528152/86b4ng084 "View ClickUp Task")).  
- Users can return to filtered **Bills** and **Invoices** after editing ([CU-86b4nh11b]( https://app.clickup.com/t/9014528152/86b4nh11b "View Clickup"), ([CU-86b4ngqx8](https://app.clickup.com/t/9014528152/86b4ngqx8 "View ClickUp Task"))).  
- Invoice number now displays at the top when editing ([CU-86b4ngqx8](https://app.clickup.com/t/9014528152/86b4ngqx8 "View ClickUp")).

**🧠 Improvements / Enhancements**

- **Memo field** shows all text ([CU-86b4ng084](https://app.clickup.com/t/9014528152/86b4ng084 "View ClickUp Task")).  
- **Client Contact** shows only company name ([CU-86b4ng084](https://app.clickup.com/t/9014528152/86b4ng084 "View ClickUp Task")).  
- **Invoice table** shows full job names ([CU-86b4ng084](https://app.clickup.com/t/9014528152/86b4ng084 "View ClickUp Task")).  
- Numbers display larger and clearer when editing ([CU-86b4ngqx8](https://app.clickup.com/t/9014528152/86b4ngqx8 "View ClickUp Task")).  
- After saving invoice changes, user stays in editing interface ([CU-86b4ngqx8](https://app.clickup.com/t/9014528152/86b4ngqx8 "View ClickUp Task")).  
- **Invoice exports** include all selected invoice data ([CU-86b4ng5xe](https://app.clickup.com/t/9014528152/86b4ng5xe "View ClickUp Task")).  
- **Payments** page includes Job column and filter ([CU-86b4c8nru](https://app.clickup.com/t/9014528152/86b4c8nru "View ClickUp Task")).  
- **Bills** page includes Created By filter ([CU-86b4gbehq](https://app.clickup.com/t/9014528152/86b4gbehq "View ClickUp Task")).

**🐛 Bug Fixes**

- **Excel & CSV exports** display correct totals ([CU-86b4ng5xe](https://app.clickup.com/t/9014528152/86b4ng5xe "View ClickUp Task")).  
- Fixed **Total Amount** issue when creating Bills from Time Entries ([CU-86b4ydj10](https://app.clickup.com/t/9014528152/86b4ydj10 "View ClickUp Task")).