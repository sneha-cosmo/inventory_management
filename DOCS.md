# InvPredict: Inventory Management System - User Handbook

Welcome to **InvPredict**, your all-in-one solution for warehouse management, production tracking, and automated billing. This document provides a comprehensive overview of the application's features and how to use them.

---

## 🚀 Getting Started

InvPredict is designed to be mobile-first and technically robust, featuring a sleek, industrial-grade UI. The primary navigation is located on the **Left Sidebar** (Desktop) or the **Bottom Bar** (Mobile).

### Core Layout:
- **Sidebar**: Switch between Dashboard, Inventory, Orders (Production), Sales, Billing, and Audit logs.
- **Header**: Contains the **Finder (Smart Scanner)**, settings, and user profile.

---

## 🔍 The Finder (Smart Scanner)
The Finder is the most powerful tool for quickly managing your stock.
1. Click the **Scan (Square)** icon in the top header.
2. **Scan**: Aim your physical scanner at a barcode (or click a simulated item in the demo).
3. **Manual Entry**: Type the SKU, Barcode number, or Item Name into the input field.
4. **Action**: Press Enter to instantly jump to that item's stock adjustment or details.

---

## 📦 Inventory Management
### Adding New Items
1. Go to the **Inventory** tab.
2. Click **Add New Item**.
3. Fill in the **Logistics Parameters**:
   - **Daily Consumption**: Average amount used per day.
   - **Lead Time**: How many days it takes for new stock to arrive.
   - **Safety Stock**: Buffer stock to prevent stockouts.
4. **Barcode Generation**: Use the "Barcode" icon next to the barcode field to generate a random EAN-13 code if you don't have one.

### Stock Levels
- **Adjust Stock**: Use this for manual corrections (damaged goods, returns, physical audit corrections).
- **Health Indicators**: Stock levels are automatically color-coded:
  - <span style="color:red">**Critical**</span>: Stock is below the Minimum Level.
  - <span style="color:orange">**Low**</span>: Approaching reorder point.
  - <span style="color:green">**Optimal**</span>: Levels are healthy.

---

## ⚙️ Production & Work Orders
Track the raw materials as they turn into finished goods.
- **Workflow**: Items move from **Awaiting** -> **Active** -> **Completed**.
- **Efficiency tracking**: Each order tracks the planned vs. actual output.
- **Integration**: Completing an order automatically updates inventory levels.

---

## 💰 Sales & Billing
### Creating Sales Orders
1. Go to the **Sales** tab.
2. Click **New Sales Order** or use **Scan to Sell** to find items via barcode.
3. Select the customer and items. The system will prevent you from overselling stock you don't have.

### Invoicing
- **Automatic Generation**: Every Delivered order generates an invoice.
- **View & Print**: Click the **View** button in the Sales table or **Print** in the Billing tab to open a professional invoice.
- **Professional Layout**: Invoices include your company header, GST details, billing address, and itemized breakdown with tax info.

---

## 🛡️ Security & Audit
### Audit Logs
Every critical change—from a barcode update to a stock adjustment—is recorded in the **Audit** tab. This ensures high accountability in multi-user environments.

### Warehouse Tracking
Manage multiple locations. View stock health per warehouse to optimize local distribution.

---

## 🛠️ Technical Specs
- **Engine**: React 18 + Vite
- **Styling**: Tailwind CSS
- **Animations**: Motion (framer-motion)
- **Data**: Real-time relational syncing with local state (Firestore-ready).
