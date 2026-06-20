# ProjectFlow — Project Management System

ProjectFlow is a zero-dependency, highly interactive Single-Page Application (SPA) built for managing projects and tracking tasks. Featuring a premium dark-mode interface, client-side authentication, a comprehensive metrics dashboard, and full CRUD capability, the app serves as a robust prototype for project tracking.

---

## 🚀 Key Features

*   **Simulated Client-Side Authentication**: Registration, login, and secure-state routing guarded by session verification.
*   **Interactive Metrics Dashboard**: Tracks total projects, active statuses, task counts, and completion percentages. Displays recent projects and tasks.
*   **Project Management (CRUD)**: Create, read, update, and delete projects. Dynamic progress bars automatically calculate completion rates based on nested tasks.
*   **Task Management (CRUD)**: Assign status, priority level, and dates to tasks. Toggle task completion instantly using list checkboxes.
*   **Global Search & Advanced Filtering**: Search and narrow down items by status, priority, or ownership.
*   **Dynamic UX**: Built-in toast notifications (success, warning, error), modal forms, page-load transition animations, and a responsive mobile sidebar.
*   **Zero Dependencies**: Written completely in Vanilla HTML5, CSS3, and modern ES6+ JavaScript. No node modules or local server needed.

---

## 🛠️ Tech Stack

*   **Structure**: HTML5 Semantic markup (App Shell)
*   **Styling**: CSS Custom Properties (Variables), Flexbox/Grid, Glassmorphism, animations
*   **Logic**: ES6+ JavaScript modules (Router, Auth Manager, Storage ORM, UI Components)
*   **Database & Session Management**: Browser `localStorage`

---

## 📁 Project Structure

```text
project-management-system/
├── index.html     # Main app skeleton (header, sidebar, modal, toast containers)
├── index.css      # Custom dark-theme styling, transitions, responsive layouts
├── app.js         # Single-Page router, business logic, storage operations
└── README.md      # Documentation (this file)
