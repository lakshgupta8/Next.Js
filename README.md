# Next.js App Router Dashboard

This project is a full-stack dashboard application built with the Next.js App Router. It serves as a comprehensive implementation of modern Next.js features, including Server Components, Server Actions, routing, authentication, and database integration.

## Features

- **Authentication**: Secure user login and protected routes using NextAuth.js.
- **Database Operations**: Direct database queries using PostgreSQL for fetching and mutating data.
- **Form Handling and Validation**: Robust server-side form validation mechanisms using Zod.
- **Search and Pagination**: URL-based search and pagination implemented with use-debounce to optimize server requests.
- **Styling**: Utility-first styling utilizing Tailwind CSS for a modern and responsive user interface.
- **Data Fetching architecture**: Utilization of React Server Components to fetch data efficiently on the server.

## Technologies Used

- **Framework**: Next.js (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Authentication**: NextAuth.js
- **Database Interface**: PostgreSQL (`postgres` client)
- **Validation Engine**: Zod
- **Password Hashing**: bcrypt

## Getting Started

### Prerequisites

- Node.js (version 18 or higher recommended)
- A PostgreSQL database instance

### Installation

1. Clone the repository and navigate to the project directory:

```bash
git clone <repository-url>
cd <project-directory>
```

2. Install the application dependencies:

```bash
npm install
```

### Configuration

Create a `.env` file at the root of your project and configure the required environment variables.

Example `.env` configuration:

```env
# Database configuration
POSTGRES_URL="postgres://user:password@hostname/database"

# NextAuth configuration
AUTH_SECRET="your-random-auth-secret"
AUTH_URL="http://localhost:3000/api/auth"
```

### Development Server

Start the local development server:

```bash
npm run dev
```

Navigate to `http://localhost:3000` in your browser to access the application.

## Project Structure

- `app/`
  - `dashboard/`: Contains the core dashboard views and nested layouts.
  - `login/`: Contains the user authentication interface.
  - `ui/`: Reusable React components such as buttons, forms, and navigation links.
  - `lib/`: Contains utility functions, database query logic, and TypeScript definitions.
- `public/`: Stores static assets.

## Acknowledgments

This project is built based on the official [Next.js App Router Course](https://nextjs.org/learn) by Vercel.
