# Productivity Tips Hub

## Overview

A full-stack productivity tips application built with React and Express that provides users with curated productivity advice across multiple categories. The application features a modern glassmorphism design, user statistics tracking, favorites management, and social sharing capabilities. Users can browse tips by category, search for specific content, track their reading progress, and manage personalized settings.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript, using Vite for build tooling
- **Routing**: Wouter for client-side routing
- **State Management**: TanStack Query for server state management and caching
- **UI Components**: Radix UI primitives with shadcn/ui component system
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **Design System**: Glassmorphism aesthetic with category-specific color coding

### Backend Architecture
- **Framework**: Express.js with TypeScript
- **Data Storage**: In-memory storage implementation with interface for future database integration
- **API Design**: RESTful endpoints for tips, user stats, favorites, and settings
- **Error Handling**: Centralized error middleware with structured error responses
- **Development**: Hot reload with Vite integration in development mode

### Data Schema Design
- **Users**: Basic user authentication structure (username/password)
- **Tips**: Content with title, description, category, and read time metadata
- **User Stats**: Reading progress tracking (tips read, favorites count, streak tracking)
- **User Favorites**: Many-to-many relationship between users and tips
- **User Settings**: Notification preferences and reading behavior settings

### Key Features
- **Category System**: Tips organized into focus, wellness, time management, organization, and motivation
- **Search Functionality**: Real-time tip searching with query-based filtering
- **User Progress Tracking**: Statistics for reading habits, streaks, and engagement
- **Social Sharing**: Twitter and LinkedIn integration with custom sharing modals
- **Responsive Design**: Mobile-first approach with glassmorphism visual effects
- **Settings Management**: User preferences for notifications and auto-read marking

### Component Architecture
- **Modular Components**: Reusable UI components with clear separation of concerns
- **Custom Hooks**: localStorage management and mobile detection utilities
- **Type Safety**: Full TypeScript integration with shared schema validation using Zod

## External Dependencies

### Database & ORM
- **Drizzle ORM**: Type-safe database toolkit configured for PostgreSQL
- **Neon Database**: Serverless PostgreSQL database provider
- **Database Migrations**: Drizzle Kit for schema management and migrations

### UI & Styling
- **Radix UI**: Comprehensive primitive component library for accessibility
- **Tailwind CSS**: Utility-first CSS framework with custom design tokens
- **Lucide React**: Icon library for consistent iconography
- **Class Variance Authority**: Type-safe component variant management

### State Management
- **TanStack Query**: Server state management with caching and synchronization
- **React Hook Form**: Form state management with validation
- **Hookform Resolvers**: Integration layer for form validation schemas

### Development Tools
- **Vite**: Fast build tool with HMR and plugin ecosystem
- **TypeScript**: Static type checking and enhanced developer experience
- **ESBuild**: Fast JavaScript bundler for production builds
- **Replit Integration**: Development environment optimization and runtime error handling

### Utility Libraries
- **Date-fns**: Date manipulation and formatting utilities
- **CLSX & Tailwind Merge**: Conditional class name management
- **Nanoid**: Unique ID generation for client-side operations
- **Embla Carousel**: Touch-friendly carousel component system