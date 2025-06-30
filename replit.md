# Satish Events & Decor - Event Decoration Business Website

## Overview

This is a full-stack web application for Satish Events & Decor, a premium event decoration business based in Ghaziabad. The application showcases the company's portfolio, services, and provides a contact form for customer inquiries. It features a modern design with 3D elements, interactive galleries, and responsive layouts.

## System Architecture

### Technology Stack
- **Frontend**: React 18 with TypeScript, Vite for build tooling
- **Backend**: Express.js with TypeScript (Node.js)
- **Database**: PostgreSQL with Drizzle ORM
- **Styling**: Tailwind CSS with shadcn/ui components
- **3D Graphics**: Three.js with React Three Fiber
- **Animations**: Framer Motion
- **State Management**: TanStack Query for server state
- **Email Service**: Nodemailer for contact form submissions

### Architecture Pattern
The application follows a monorepo structure with clear separation between client and server code:
- **Client**: React SPA with modern component architecture
- **Server**: RESTful API with Express.js
- **Shared**: Common schemas and types using Drizzle and Zod

## Key Components

### Frontend Architecture
- **Component-based architecture** using React functional components
- **Custom hooks** for scroll animations and mobile detection
- **3D scene management** with React Three Fiber for interactive elements
- **Responsive design** using Tailwind CSS breakpoints
- **Type safety** throughout with TypeScript

### Backend Architecture
- **RESTful API** with Express.js middleware
- **Database abstraction** using Drizzle ORM with PostgreSQL
- **Email service integration** for contact form processing
- **Environment-based configuration** for different deployment stages

### Database Design
The application uses three main tables:
- **users**: Basic user authentication (currently using in-memory storage)
- **contacts**: Customer inquiry form submissions
- **portfolio_items**: Dynamic portfolio management

### UI Component System
- **shadcn/ui**: Pre-built accessible components
- **Radix UI**: Unstyled, accessible component primitives
- **Custom components**: Business-specific components for galleries, forms, and sections

## Data Flow

1. **Client-side rendering**: React components fetch data using TanStack Query
2. **API requests**: RESTful endpoints handle contact form submissions
3. **Database operations**: Drizzle ORM manages database interactions
4. **Email notifications**: Nodemailer sends inquiry notifications
5. **3D rendering**: Three.js handles interactive visual elements

The application uses a unidirectional data flow pattern with React's component state and TanStack Query for server state management.

## External Dependencies

### Core Dependencies
- **@neondatabase/serverless**: PostgreSQL database driver
- **drizzle-orm**: Type-safe database ORM
- **@tanstack/react-query**: Server state management
- **@react-three/fiber**: React renderer for Three.js
- **framer-motion**: Animation library
- **nodemailer**: Email service
- **zod**: Runtime type validation

### UI Dependencies
- **@radix-ui/react-***: Collection of accessible UI primitives
- **tailwindcss**: Utility-first CSS framework
- **class-variance-authority**: Type-safe component variants
- **sonner**: Toast notifications

### Development Dependencies
- **vite**: Fast build tool and dev server
- **typescript**: Static type checking
- **tsx**: TypeScript execution for Node.js
- **esbuild**: Fast bundler for production builds

## Deployment Strategy

### Build Process
1. **Frontend build**: Vite compiles React app to static assets
2. **Backend build**: esbuild bundles Express server for production
3. **Database migration**: Drizzle handles schema migrations
4. **Static asset serving**: Express serves built client files

### Environment Configuration
- **Development**: Uses Vite dev server with hot module replacement
- **Production**: Serves built static files from Express server
- **Database**: PostgreSQL with connection via DATABASE_URL environment variable
- **Email**: SMTP configuration via environment variables

### Scaling Considerations
- **Database**: Uses connection pooling for PostgreSQL
- **Static assets**: Can be served via CDN in production
- **Email service**: Uses external SMTP provider for reliability
- **3D assets**: Optimized for web delivery with appropriate formats

## Changelog

```
Changelog:
- June 29, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```