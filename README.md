# EventHub - Event Management Platform

A modern, beautiful event management web application built with Next.js 15, TypeScript, and Tailwind CSS.

## 🚀 Features

### ✅ Completed UI Components

- **Modern Dashboard Layout** with responsive sidebar navigation
- **Beautiful Landing Page** with smooth animations
- **Events Listing Page** with filtering, search, and card-based layout
- **Event Creation Form** with comprehensive validation
- **Analytics Dashboard** with charts and performance metrics
- **Dark/Light Theme Support** with system preference detection
- **Responsive Design** optimized for mobile, tablet, and desktop

### 🎨 Design System

- **Shadcn/ui Components** - Modern, accessible component library
- **Custom Animations** - Smooth fade-in, slide-up, and scale animations
- **Glass Effect Styling** - Modern backdrop blur effects
- **Custom Scrollbars** - Styled scrollbars for better UX
- **Gradient Backgrounds** - Beautiful gradient overlays

### 📱 Pages Implemented

1. **Landing Page** (`/`) - Welcome screen with auto-redirect to dashboard
2. **Dashboard** (`/dashboard`) - Overview with stats, recent events, and quick actions
3. **Events Listing** (`/events`) - Comprehensive event management with filters
4. **Create Event** (`/events/create`) - Beautiful form with validation
5. **Analytics** (`/analytics`) - Performance metrics and insights

## 🛠️ Tech Stack

- **Framework**: Next.js 15 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **UI Components**: Shadcn/ui + Radix UI
- **Icons**: Lucide React
- **Form Handling**: React Hook Form + Zod validation
- **Animations**: Framer Motion + Custom CSS animations
- **Theme**: Next-themes for dark/light mode
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ and npm
- A Supabase account (free tier available)

### 1. Clone and Install

```bash
git clone https://github.com/Shaharyar417/eventhub-webinar-app.git
cd eventhub-webinar-app
npm install
```

### 2. Set Up Supabase

1. Create a new project at [supabase.com](https://supabase.com)
2. Go to Settings → API and copy your credentials
3. Create `.env.local` file:
   ```bash
   NEXT_PUBLIC_SUPABASE_URL=https://your-project-id.supabase.co
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key-here
   SUPABASE_SERVICE_ROLE_KEY=your-service-role-key-here
   ```

### 3. Set Up Database

1. Go to your Supabase SQL Editor
2. Copy and run the contents of `src/lib/supabase/schema.sql`
3. Copy and run the contents of `src/lib/supabase/functions.sql`

### 4. Configure Authentication

1. In Supabase Dashboard → Authentication → Settings
2. Set Site URL to `http://localhost:3000`
3. Add redirect URL: `http://localhost:3000/auth/callback`

### 5. Start Development Server

```bash
npm run dev
```

### 6. Open in Browser

Navigate to [http://localhost:3000](http://localhost:3000)

📖 **Detailed Setup Guide**: See `SUPABASE_SETUP.md` for complete instructions.

## 📁 Project Structure

```
src/
├── app/                    # Next.js App Router pages
│   ├── dashboard/         # Dashboard page
│   ├── events/           # Events listing and creation
│   ├── analytics/        # Analytics dashboard
│   ├── globals.css       # Global styles and animations
│   └── layout.tsx        # Root layout with theme provider
├── components/
│   ├── ui/               # Shadcn/ui components
│   ├── layout/           # Layout components (header, sidebar)
│   └── theme-provider.tsx # Theme switching logic
└── lib/
    └── utils.ts          # Utility functions
```

## ✅ Complete Features

### Backend Integration

- **Supabase Integration** ✅ - Database and authentication fully configured
- **User Authentication** ✅ - Login/register functionality with JWT tokens
- **Database Schema** ✅ - Complete schema with RLS policies
- **Event Management** ✅ - Full CRUD operations with database
- **User Profiles** ✅ - Profile management with avatar upload
- **Real-time Updates** ✅ - Live updates using Supabase subscriptions
- **Analytics** ✅ - Event statistics and performance metrics

### Security Features

- **Row Level Security (RLS)** - Database-level security policies
- **JWT Authentication** - Secure token-based authentication
- **Protected Routes** - Middleware-based route protection
- **Input Validation** - Form validation with Zod schemas
- **CSRF Protection** - Built-in Next.js security features

---

**Built with ❤️ using modern web technologies for the best user experience.**