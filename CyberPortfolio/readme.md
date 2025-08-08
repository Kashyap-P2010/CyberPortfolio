# Overview

This is a full-stack web application built with a modern React frontend and Express backend. The project appears to be a cyberpunk-themed developer portfolio website with a futuristic hacker aesthetic. The application uses a monorepo structure with shared TypeScript schemas and a PostgreSQL database managed through Drizzle ORM.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript, built using Vite
- **Styling**: Tailwind CSS with shadcn/ui component library for consistent UI components
- **State Management**: TanStack Query (React Query) for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Theme**: Cyberpunk/hacker aesthetic with matrix rain background effects, custom cursors, and neon color schemes
- **Animations**: GSAP and Three.js for advanced animations and 3D effects
- **Forms**: React Hook Form with Zod validation via @hookform/resolvers

## Backend Architecture
- **Framework**: Express.js with TypeScript
- **Build System**: ESBuild for production bundling, TSX for development
- **Development**: Hot module replacement via Vite integration
- **Storage Interface**: Abstracted storage layer with in-memory implementation for development
- **Session Management**: PostgreSQL-backed sessions using connect-pg-simple

## Data Storage
- **Database**: PostgreSQL with Neon Database serverless driver
- **ORM**: Drizzle ORM for type-safe database operations
- **Schema Management**: Shared TypeScript schema definitions with Zod validation
- **Migrations**: Drizzle Kit for database migrations and schema management

## Authentication & Authorization
- Basic user schema defined with username/password fields
- Session-based authentication infrastructure prepared
- No authentication routes currently implemented

## External Dependencies
- **Database**: Neon Database (@neondatabase/serverless) for serverless PostgreSQL
- **UI Components**: Extensive Radix UI primitive components via shadcn/ui
- **Animation Libraries**: GSAP for animations, Three.js for 3D graphics
- **Development**: Replit-specific plugins for runtime error handling and debugging
- **Styling**: PostCSS with Autoprefixer for CSS processing
- **Type Safety**: Comprehensive TypeScript setup with strict configuration

The application follows a clean separation of concerns with shared types between frontend and backend, modular component architecture, and a flexible storage abstraction that can be easily switched from in-memory to database-backed implementations.