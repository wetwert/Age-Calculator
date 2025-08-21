# Age Calculator Application

## Overview

This is a comprehensive age calculator web application that provides detailed age calculations, life statistics, zodiac signs, and historical comparisons. The application allows users to input their birth date and receive extensive information about their age, including exact years/months/days, countdown to next birthday, life statistics (heartbeats, breaths, etc.), zodiac signs (Western and Chinese), historical events from their birth year, and celebrity age comparisons.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture

**Framework**: React with TypeScript using Vite as the build tool
- Component-based architecture with reusable UI components
- Client-side routing using Wouter for single-page application navigation
- State management through React hooks (useState, useEffect)
- Form handling and validation using React Hook Form with Zod schemas
- Date manipulation library (date-fns) for all age calculations and date operations

**UI Library**: shadcn/ui components built on Radix UI primitives
- Comprehensive component library including cards, buttons, inputs, dialogs, and more
- Consistent design system with Tailwind CSS for styling
- Dark mode support through CSS variables
- Custom component variants using class-variance-authority

**Styling**: Tailwind CSS with custom design tokens
- CSS custom properties for theme management
- Responsive design with mobile-first approach
- Custom animations and transitions
- Inter font family for typography

**Data Management**:
- TanStack Query for server state management and caching
- Static data files for historical events and celebrity information
- Client-side calculation utilities for age computations, zodiac signs, and life statistics

### Backend Architecture

**Server Framework**: Express.js with TypeScript
- RESTful API design patterns
- Middleware for request logging and error handling
- Health check endpoints for monitoring
- Development and production environment configurations

**Development Setup**:
- Vite integration for hot module replacement in development
- Custom middleware for serving static assets and handling SPA routing
- Development-specific error overlay and debugging tools

**Authentication Ready**: Basic user schema and storage interface defined
- User model with username/password fields
- In-memory storage implementation for development
- Database-ready with Drizzle ORM schema definitions

### Data Storage Solutions

**Database ORM**: Drizzle ORM with PostgreSQL support
- Type-safe database operations
- Schema migration support with drizzle-kit
- Connection to Neon Database (serverless PostgreSQL)
- Prepared for user authentication and data persistence

**Static Data Storage**:
- Historical events data organized by years
- Celebrity database with birth dates and professions
- Zodiac sign definitions and characteristics
- All calculations performed client-side for optimal performance

### External Dependencies

**Core Libraries**:
- React ecosystem (React 18, React DOM, React Router via Wouter)
- TypeScript for type safety across frontend and backend
- Express.js for server framework
- Vite for build tooling and development server

**UI and Styling**:
- Radix UI primitives for accessible components
- Tailwind CSS for utility-first styling
- Lucide React for consistent iconography
- Inter and custom fonts via Google Fonts

**Development Tools**:
- ESBuild for production bundling
- PostCSS with Autoprefixer for CSS processing
- Replit-specific plugins for development environment integration

**Date and Utility Libraries**:
- date-fns for comprehensive date manipulation and calculations
- clsx and tailwind-merge for conditional CSS class management
- Zod for runtime type validation and schema definition

**Database and ORM**:
- Drizzle ORM for type-safe database operations
- @neondatabase/serverless for PostgreSQL connection
- drizzle-zod for schema validation integration

The application is designed as a primarily client-side application where all age calculations, zodiac determinations, and data presentations are handled in the browser for optimal performance. The backend serves as a foundation for future user authentication and data persistence features.