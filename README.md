#  Orders App

A Flutter-based cross-platform application to manage and display open stock orders.
This project demonstrates a clean, modern UI with interactive components (search, filters, dialogs, bottom sheets) and a modular approach for future scalability.
<img width="200" height="423.5" alt="Screenshot_20250904_130125" src="https://github.com/user-attachments/assets/542bb04b-f2fc-4c95-9d7a-813ad7be3145" />

---

 My Approach

The app is built with a UI-first approach, focusing on a professional orders dashboard:

1. Core Layout
   - `Scaffold` + `AppBar` for top navigation and structure.
   - A subtle divider under the AppBar for visual separation.

2. **Search & Filters**
   - A custom search bar (`TextField`) placeholder to filter orders.
   - Reusable filter chips for quick symbol filters.
   - A **"Cancel all"** action with a confirmation dialog.

3. **Orders List**
   - `ListView.builder` for performance with growing lists.
   - Each order is shown as a card containing:
     - Side badge (Buy/Sell) with semantic colors.
     - Client, ticker, product, and time.
     - Price and quantity shown as `executed/total`.
     - A progress bar visualizing execution percentage.

4. **User Interactions**
   - Bottom sheet for per-order actions (Modify, Cancel, Details).
   - Global options bottom sheet (Download, Refresh, Filter options).
   - Confirmation dialogs for destructive actions.

5. **Reusable Components**
   - Extracted helpers: `_buildOrderCard`, `_buildFilterChip`, `_buildBottomSheetOption`.
   - An `Order` data model structures the order fields.

---

## 📂 Project Structure

```
orders_app/
│
├── lib/
│   └── main.dart        # Entry point, UI widgets, interactions, and Order model
│
├── android/             # Android native project files
├── ios/                 # iOS native project files
├── web/                 # Web build files
├── windows/             # Windows desktop support
├── pubspec.yaml         # App metadata & dependencies
└── README.md            # This documentation
```



- **Framework:** Flutter (Dart, Material Design)


