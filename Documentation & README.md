# Fin-Aggregate

**Fin-Aggregate** is a Next.js application designed to manage and aggregate financial data. Built for a hackathon, the project leverages modern tools and libraries to deliver a seamless and rich user experience, with features for real-time data management, visualization, and more.

## Table of Contents

- [Overview](#overview)
- [Project Architecture](#project-architecture)
- [Features](#features)
- [Project Setup](#project-setup)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [Scripts](#scripts)
- [Core Dependencies](#core-dependencies)
- [Dev Dependencies](#dev-dependencies)
- [Usage](#usage)
- [Additional Information](#additional-information)
- [License](#license)

## Overview

Fin-Aggregate aggregates data from multiple financial sources, providing a unified view of accounts, transaction history, and spending patterns. The application features real-time updates, secure user authentication, and advanced data visualization.

## Project Architecture

This project follows a full-stack architecture using:

- **Frontend**: Built with Next.js and React for a fast and interactive user experience.
- **Backend**: Utilizes API routes in Next.js for server-side operations and data fetching.
- **Database**: MySQL is used for persistent data storage, managed and queried via Drizzle ORM.
- **Authentication**: User authentication is handled through Clerk, ensuring secure and easy management of user sessions.
- **Data Visualization**: Recharts is used to create interactive and dynamic visualizations for the financial data.

## Features

- **Data Aggregation**: Collects and normalizes financial data from multiple sources.
- **Secure Authentication**: User authentication using Clerk for robust security.
- **Dynamic Visualizations**: Provides users with interactive charts and graphs using Recharts.
- **Real-Time Updates**: Allows for real-time data management and visualization.
- **Responsive Design**: Fully responsive UI built with Tailwind CSS.

## Project Setup

### Prerequisites

- **Node.js**: Version 18 or later is required. [Download Node.js](https://nodejs.org/).
- **MySQL**: Install and configure [MySQL](https://www.mysql.com/).

### Installation

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd fin-aggregate
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

### Configuration

1. **Environment Variables**: Create a `.env.local` file in the root directory and add the following environment variables:

   ```bash
   NEXT_PUBLIC_CLERK_FRONTEND_API=<your-clerk-frontend-api>
   CLERK_API_KEY=<your-clerk-api-key>
   DATABASE_URL=<your-database-url>
   ```

2. **Database Setup**: Configure your MySQL database and apply schema migrations using Drizzle ORM:

   ```bash
   npm run db:push
   ```

## Scripts

Here are the available npm scripts to help with development and deployment:

- **`dev`**: Starts the development server with hot reloading.

  ```bash
  npm run dev
  ```

- **`build`**: Compiles the project for production.

  ```bash
  npm run build
  ```

- **`start`**: Starts the production server.

  ```bash
  npm run start
  ```

- **`lint`**: Runs linting checks on the codebase.

  ```bash
  npm run lint
  ```

- **`db:push`**: Applies database migrations using Drizzle ORM.

  ```bash
  npm run db:push
  ```

- **`db:studio`**: Opens the Drizzle ORM studio for managing your database.

  ```bash
  npm run db:studio
  ```

## Core Dependencies

- **[@clerk/nextjs](https://clerk.dev/docs/nextjs)**: Provides authentication and user management for Next.js applications.
- **[ag-grid-react](https://www.ag-grid.com/react-data-grid/)**: A powerful data grid component for displaying and manipulating data.
- **[axios](https://axios-http.com/)**: A promise-based HTTP client for making requests to APIs.
- **[drizzle-orm](https://orm.drizzle.team/)**: A modern ORM for TypeScript and JavaScript that integrates with MySQL databases.
- **[next](https://nextjs.org/)**: The React framework for building server-side rendered and static web applications.
- **[react](https://reactjs.org/)**: A JavaScript library for building user interfaces.
- **[recharts](https://recharts.org/)**: A charting library built with React components for data visualization.
- **[tailwindcss](https://tailwindcss.com/)**: A utility-first CSS framework for rapidly building custom designs.
- **[zod](https://zod.dev/)**: A TypeScript-first schema declaration and validation library.

## Dev Dependencies

- **[@types/node](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/node)**: Provides TypeScript type definitions for Node.js.
- **[@types/react](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/react)**: Provides TypeScript type definitions for React.
- **[@types/react-dom](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/react-dom)**: Provides TypeScript type definitions for React DOM.
- **[drizzle-kit](https://github.com/drizzle-team/drizzle-kit)**: CLI for managing Drizzle ORM migrations and database schema.
- **[postcss](https://postcss.org/)**: A tool for transforming CSS with JavaScript plugins.
- **[typescript](https://www.typescriptlang.org/)**: A strongly typed programming language that builds on JavaScript.

## Usage

### Development

Start the development server to see changes in real-time:

```bash
npm run dev
```

### Production

Build and start the application for production:

```bash
npm run build
npm run start
```

## Additional Information

For more detailed information about each dependency, refer to their respective documentation linked in the Core and Dev Dependencies sections.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more information.
```

This version provides more clarity, details, and a polished structure for anyone viewing your GitHub repo.
