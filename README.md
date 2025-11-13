# Travel Itinerary Web Application

A responsive, accessible, single‑page **Travel Itinerary Manager** built using **HTML, CSS, JavaScript, and Bootstrap 5**. It allows users to add, edit, delete, search, filter, import, and export itinerary items. All data is saved in the browser via **localStorage**, meaning no backend is required.

---
 Features

 Core Features
- Add, edit, delete itinerary items
- Store items in **localStorage** (data persists locally)
- Search by title, notes, or location
- Filter by date or jump to **today**
- Import and export itinerary as **JSON**
- Automatic trip summary (item count & date range)
- Sample demo data for first‑time users

 UI & Styling
- Modern responsive layout using **Bootstrap 5**
- Custom color palette using CSS variables
- Sticky filter sidebar
- Smooth modal form for item editing
- Accessible controls (ARIA labels, keyboard shortcuts)

 Technical Highlights
- Modular JavaScript with functions for CRUD operations
- Debounced search input for better performance
- Dynamic UI rendering
- Keyboard shortcuts:
  - **Ctrl + N** → Add new item
  - **/** → Focus search


All logic is currently inside **index.html** for simplicity.

---
 How It Works

### 1. Saving Data
Items are stored using:
```
localStorage.setItem('itinerary.v1', JSON.stringify(items));
```

### 2. Loading Data
If no saved data exists, sample items are created automatically.

### 3. Rendering the List
JavaScript dynamically builds the itinerary list using DOM operations.

### 4. Import / Export
- Export → Downloads a `.json` file
- Import → Reads a JSON file and validates fields

---
 Requirements
No external backend or dependencies needed.
Only requires:
- A modern browser
- Internet (for Bootstrap CDN)

---
 How to Use

1. Open the **index.html** file in a browser.
2. Click **Add Item** to insert a new itinerary entry.
3. Use search or filters to find specific items.
4. Export or import your itinerary using JSON buttons.
5. All changes are saved automatically.
