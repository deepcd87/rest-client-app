# 🚀 REST Client
### Final Team Project (RS React Course)

This project is the final team assignment of the **RS School React Course**.  
It is a simplified Postman-like REST client built with **Next.js**, featuring secure authentication, a full backend, internationalization, a request history system, and generated code snippets.

The project simulates real-world web development teamwork:

- students collaborate in a shared repository
- participate in code reviews
- follow Git flow
- build production-ready features
- work with a mentor who reviews the codebase
- complete a full 4-week sprint using Agile principles

---

## ⚡ Technology Stack

### **Core**

- **Next.js 15 (App Router, Turbopack)**
- **React 19**
- **TypeScript 5**

### **Backend & Auth**

- **NextAuth.js v5**
- **Prisma ORM**
- **bcrypt / bcryptjs**

### **UI**

- **Tailwind CSS v4**
- **Heroicons**
- **next-intl** (internationalization)

### **Validation**

- **Zod**

### **Testing**

- **Vitest**
- **Testing Library**
- **JSDOM**

### **Code Quality**

- **ESLint**
- **Prettier**
- **Husky**

---

## 🏁 Sprints Overview

<details>
  <summary><strong>🟦 Sprint 1 – Project Setup & Authentication</strong></summary>

- Initialize Next.js project (App Router + Turbopack)
- Configure Prisma and the database connection
- Implement authentication via **NextAuth.js (Credentials provider)**
- Create Sign In / Sign Up pages
- Integrate **next-intl** for multi-language support
- Setup Tailwind CSS and global layout
- Add protected routes and session logic
- Configure ESLint, Prettier, Husky, Git Hooks
</details>

<details>
  <summary><strong>🟨 Sprint 2 – REST Client Core</strong></summary>

- Implement method selector (GET, POST, PUT, PATCH, DELETE)
- Build URL input with Base64-encoded parameter handling
- Add headers and body editors
- Create a fetch proxy on the server to bypass CORS
- Add formatted response viewer (JSON highlight)
- Handle request errors gracefully
- Add custom 404 and error components
</details>

<details>
  <summary><strong>🟩 Sprint 3 – Variables & Code Generation</strong></summary>

- Add variable editor with LocalStorage persistence
- Implement variable substitution (`{{varName}}`) for requests
- Generate request code snippets for:
  - curl
  - JavaScript fetch
  - Node.js
  - Python
  - Go
  - Java
  - C#
- Improve layout, mobile responsiveness, and accessibility
</details>

<details>
  <summary><strong>🟥 Sprint 4 – History & Analytics</strong></summary>

- Store request history in the database via Prisma
- Save:
  - URL
  - method
  - status
  - duration
  - response size
  - request size
  - timestamp
- Implement history page UI
- Allow reopening requests from history
- Add “Empty history” state
</details>

---

## 🚀 Get Started

> ⚠️ **Important:**  
> The application will NOT run without **environment variables** for **NextAuth** and **Prisma**.  
> Make sure to configure your `.env` file before starting the project.

Follow these steps to set up the project locally:

### 1. Clone the repository

```bash
git clone https://github.com/deepcd87/rest-client-app.git
cd rest-client-app
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Rename the `example.env` to `.env`:

- Linux / MacOS:

```bash
mv example.env .env
```

- Windows (CMD)::

```bash
rename example.env .env
```

### 4. Set up the database

```bash
npx prisma generate
npx prisma db push
```

### 5. Run the development server

```bash
npm run dev
```

## 📜 Available Scripts

| Command                 | Description                             |
| ----------------------- | --------------------------------------- |
| `npm run dev`           | Start Next.js dev server with Turbopack |
| `npm run build`         | Build the project for production        |
| `npm start`             | Run production server                   |
| `npm run lint`          | Run ESLint                              |
| `npm run lint:fix`      | Fix ESLint warnings                     |
| `npm run format:fix`    | Format code with Prettier               |
| `npm test`              | Run unit tests via Vitest               |
| `npm run test:watch`    | Watch mode for tests                    |
| `npm run test:coverage` | Generate coverage report                |
