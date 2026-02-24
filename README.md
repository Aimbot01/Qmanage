# Qmanage • Full-Stack Food Ordering Platform

Qmanage is a full-stack **food ordering and management platform** built with **Node.js, Express, EJS, and MongoDB**.  
It has evolved from a static frontend into a server-rendered, data-driven web application with a modular backend and rich frontend interactivity.

The project demonstrates real-world full-stack concepts including MVC architecture, RESTful APIs, server-side rendering, and dynamic frontend behavior.

---

## 🍽️ Highlights

- Server-rendered **EJS views** with reusable layouts and partials  
- **Node.js + Express + MongoDB** backend using clean MVC architecture  
  (`/routes · /controllers · /models`)
- Full **CRUD APIs** for:
  - Outlets
  - Menu Items
  - Orders
- Admin console (EJS + vanilla JS) for managing outlets, menus, and live orders
- Dynamic pages powered by **JSON & REST APIs**
- Rich frontend **OOP architecture**:
  - `Cart`, `FoodItem`, `Outlet` classes
  - Filters, modals, animations, and state syncing
- Developer-friendly workflow with **Nodemon**
- Environment-based MongoDB configuration

---

## 🚀 Getting Started

### 1️⃣ Prerequisites
- **Node.js** 18+
- **MongoDB** (local or cloud-hosted)

---
Qmanage/
├── server.js
├── config/
│   └── database.js
├── controllers/
│   ├── menuController.js
│   ├── orderController.js
│   ├── outletController.js
│   └── pageController.js
├── models/
│   ├── MenuItem.js
│   ├── Order.js
│   └── Outlet.js
├── routes/
│   ├── webRoutes.js
│   └── api/
│       ├── index.js
│       ├── menuRoutes.js
│       ├── orderRoutes.js
│       └── outletRoutes.js
├── views/
│   ├── layout.ejs
│   ├── partials/
│   ├── admin/
│   └── *.ejs
├── public/
│   ├── css/
│   ├── js/
│   ├── json/
│   └── img/
└── README.md

| Method | Endpoint                 | Description                         |
| ------ | ------------------------ | ----------------------------------- |
| GET    | `/api/outlets`           | List outlets                        |
| POST   | `/api/outlets`           | Create outlet                       |
| PUT    | `/api/outlets/:id`       | Update outlet                       |
| DELETE | `/api/outlets/:id`       | Remove outlet (cascades menu)       |
| GET    | `/api/menu-items`        | List menu items (filters supported) |
| POST   | `/api/menu-items`        | Create menu item                    |
| PUT    | `/api/menu-items/:id`    | Update menu item                    |
| DELETE | `/api/menu-items/:id`    | Delete menu item                    |
| GET    | `/api/orders`            | List orders                         |
| POST   | `/api/orders`            | Create order                        |
| PUT    | `/api/orders/:id`        | Update order                        |
| PATCH  | `/api/orders/:id/status` | Update order status                 |
| DELETE | `/api/orders/:id`        | Delete order                        |

🧠 Frontend Architecture

public/js/main.js — Cart class (localStorage sync, custom events)

public/js/home.js — FoodItem, OutletCategory, sliders

public/js/menu.js — Menu model, filters, rendering

public/js/outlets.js — Outlet model, modal controllers

public/js/order.js — Outlet-aware menu browsing

public/js/cart.js — Cart page syncing

public/js/admin/*.js — Fetch-based admin CRUD dashboards

public/js/data-loader.js — API-first loader with JSON fallback

public/js/utils.js — UI helpers, animations, validators


🤝 Contributing

Issues, ideas, and pull requests are welcome.
Please raise an issue before making large changes so we can collaborate on the project direction.

📄 License

MIT © Rohan Yadav


