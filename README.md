# Brev.ly - Link Shortener Monorepo

A fast, clean, and production-ready Link Shortener application built using a Monorepo architecture with **pnpm Workspaces**. It features a Fastify back-end leveraging Drizzle ORM and a modern React front-end.

## 🏗️ Project Architecture

This repository is split into two independent domains managed under a single workspace:
- **`server/`**: The backend HTTP API powered by Node.js, Fastify, Zod, and Drizzle ORM (PostgreSQL).
- **`web/`**: The frontend Single Page Application (SPA) built with React, Vite, TailwindCSS, and Zustand.

## 🛠️ Prerequisites

Before getting started, make sure you have the following installed on your machine:
- [Node.js](https://nodejs.org/) (v18 or higher)
- [pnpm](https://pnpm.io/) (v8 or higher recommended)
- [PostgreSQL](https://www.postgresql.org/) database instance running

## 🚀 Getting Started

### 1. Install Dependencies
Run the following command in the root folder to install all dependencies for both the server and web applications concurrently using shared linking:
```bash
pnpm install
```

### 2. Environment Configuration
You need to set up the environment variables for both projects. Follow the instructions inside the `server/.env.example` and `web/.env.example` files to create your respective `.env` files.

### 3. Running the Project Locally
To start both the back-end server and the front-end application simultaneously in development mode, run:
```bash
pnpm dev
```

The application will be available at:
- **Frontend Dashboard:** `http://localhost:5173`
- **Backend API:** `http://localhost:3333`
