# Phone Finder

## Table of Contents

- [Phone Finder](#phone-finder)
  - [Table of Contents](#table-of-contents)
  - [📌 Overview](#-overview)
  - [🚀 Features](#-features)
  - [🛠️ Technologies Used](#️-technologies-used)
    - [**Frontend**](#frontend)
    - [**Backend**](#backend)
    - [**Testing \& Dev Tools**](#testing--dev-tools)
  - [🏁 Getting Started](#-getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
    - [Environment Variables](#environment-variables)
  - [📂 Project Structure](#-project-structure)
  - [📌 Low-Level Design](#-low-level-design)
    - [Core Structure](#core-structure)
    - [Main Components](#main-components)
  - [⚙️ Technical Implementation](#️-technical-implementation)
  - [📌 API Reference](#-api-reference)
  - [🧪 Testing](#-testing)
  - [👥 Team Members](#-team-members)
  - [🤝 Contributing](#-contributing)
  - [📝 License](#-license)
  - [🙏 Acknowledgments](#-acknowledgments)

---

## 📌 Overview

**Phone Finder** is a full-stack web application designed to help users **search, compare, discuss, and purchase** smartphones. It consists of three main modules:

1. **Admin Panel** - Manages users, products, orders, and community content.
2. **Community Platform** - Enables discussions, reviews, and social interactions.
3. **E-Commerce Platform** - Facilitates phone searches, comparisons, and purchases.

This project follows a **scalable, modular, and secure architecture**, ensuring a smooth user experience.

---

## 🚀 Features

- **🔍 Phone Catalog** – Browse and explore detailed smartphone specifications.
- **🎯 Advanced Search** – Filter phones based on brand, price, and features.
- **📊 Comparison Tool** – Side-by-side comparison of up to three phones.
- **🔑 User Authentication** – Secure login, registration, and session management.
- **🛒 Shopping Cart** – Add phones to the cart and manage purchases.
- **💬 Community Platform** – Engage in discussions and post product reviews.
- **⚡ Admin Dashboard** – Manage products, users, and orders.
- **🌙 Dark Mode** – Toggle between light and dark themes.
- **🔐 Role-Based Access** – Separate permissions for Admins, Moderators, and Users.

---

## 🛠️ Technologies Used

### **Frontend**

- **Next.js 15** (App Router)
- **React.js 18.2**
- **TypeScript 5.0**
- **Tailwind CSS 3.3**
- **shadcn/ui** (UI Components)
- **Lucide React** (Icons)

### **Backend**

- **Next.js API Routes** (`/api/`)
- **Prisma ORM** (Database Management)
- **PostgreSQL** (Primary Database)
- **Redis** (Caching & Real-time Updates)
- **NextAuth.js** (Authentication)

### **Testing & Dev Tools**

- **Cypress** (E2E Testing)
- **Jest & React Testing Library** (Unit Testing)
- **ESLint & Prettier** (Code Quality)
- **Husky & Lint-staged** (Git Hooks)

---

## 🏁 Getting Started

### Prerequisites

Make sure you have the following installed:

- **Node.js** (`v18+`)
- **npm** (`v9+`) or **pnpm** (`v8+`)

### Installation

1. **Clone the Repository**

   ```sh
   git clone https://github.com/your-username/phone-finder.git
   cd phone-finder
   ```

2. **Install Dependencies**

   ```sh
   npm install
   ```

3. **Set Up the Database**

   ```sh
   npx prisma migrate dev
   ```

4. **Run the Development Server**

   ```sh
   npm run dev
   ```

### Environment Variables

Create a `.env` file in the root directory and configure the following:

```env
DATABASE_URL=postgresql://user:password@localhost:5432/phone_finder
NEXTAUTH_SECRET=your-secret-key
NEXT_PUBLIC_API_URL=http://localhost:3000/api
```

---

## 📂 Project Structure

```txt
phone-finder/
│── public/                # Static assets
│── src/
│   ├── app/               # Next.js App Router
│   │   ├── api/           # API routes
│   │   ├── admin/         # Admin Panel
│   │   ├── community/     # Community Features
│   │   ├── shop/          # E-Commerce Pages
│   │   ├── auth/          # Authentication
│   ├── components/        # UI Components
│   ├── hooks/             # Custom Hooks
│   ├── lib/               # Config & Utilities
│   ├── store/             # State Management
│   ├── styles/            # Tailwind CSS
│   ├── tests/             # Cypress & Unit Tests
│── prisma/                # Database Schema
│── .env                   # Environment Variables
│── next.config.mjs        # Next.js Configuration
│── tsconfig.json          # TypeScript Config
│── package.json           # Dependencies
│── README.md              # Documentation
```

---

## 📌 Low-Level Design

### Core Structure

- **Layout**: A responsive layout with header, main content area, and footer.
- **Theme Support**: Light and dark mode with a theme toggle.
- **Responsive Design**: Mobile-friendly UI that adapts to different screen sizes.

### Main Components

1. **Home Page**

   - Hero section with call-to-action
   - Search functionality
   - Features overview
   - Featured phones display

2. **Phones Browsing**

   - Filtering options (brand, price, specs)
   - Grid/list view options
   - Sorting capabilities
   - Pagination

3. **Phone Comparison**

   - Side-by-side comparison of up to 3 phones
   - Tabbed interface for specs, features, and camera
   - Visual performance comparison
   - Recommendations

4. **Community Platform**

   - Discussion forums
   - User reviews
   - Community stats
   - Guidelines

5. **Admin Dashboard**
   - Overview with key metrics
   - User management
   - Product management
   - Order tracking
   - Community moderation

---

## ⚙️ Technical Implementation

- **Next.js 15 App Router** for optimized routing.
- **TypeScript** for type safety.
- **Tailwind CSS** & **shadcn/ui** for styling and UI components.
- **Responsive Design** with fully adaptive layouts.
- **Dark/Light Mode Support** via context API.
- **Backend API Routes** in Next.js to handle authentication, product retrieval, and order processing.
- **Prisma ORM** with **PostgreSQL** for data persistence.
- **Redis Caching** to improve performance.

---

## 📌 API Reference

- `POST /api/auth/login` – User Login
- `POST /api/auth/register` – User Signup
- `GET /api/products` – Fetch All Products
- `GET /api/products/{id}` – Fetch Single Product
- `POST /api/cart/add` – Add to Cart
- `POST /api/order/checkout` – Checkout Order
- `GET /api/community/posts` – Fetch Community Discussions

---

## 🧪 Testing

**End-to-End Testing (Cypress)**

```sh
npx cypress open
```

**Unit Testing (Jest)**

```sh
npm run test
```

---

## 👥 Team Members

- **Md. Maruf Sarker** - 221002063
- **Md. Sohel** - 221002173
- **Moriam Khatun** - 221002197

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m "Added feature"`)
4. Push to your branch (`git push origin feature-name`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the **MIT License**.

---

## 🙏 Acknowledgments

Special thanks to:

- **Next.js Community** for their powerful framework.
- **shadcn/ui** for UI components.
- **Prisma** for simplifying database management.
