# 🍽️ Swipes Admin

An admin dashboard for managing the **Swipes** platform — a food discovery and recipe-swiping mobile app.

## Overview

Swipes Admin provides a web-based control panel for managing all aspects of the Swipes platform, including:

- 📋 **Restaurant & Recipe Management** — Add, edit, and remove food listings
- 👥 **User Management** — View, moderate, and manage user accounts
- 📊 **Analytics Dashboard** — Monitor swipes, likes, and engagement metrics
- 🏷️ **Category & Tag Management** — Organise content with categories and dietary tags
- 🔔 **Push Notification Control** — Send targeted notifications to users
- ⚙️ **App Settings** — Configure global platform settings

## Tech Stack

| Layer      | Technology              |
|------------|-------------------------|
| Framework  | Next.js (App Router)    |
| Styling    | Tailwind CSS            |
| Auth       | Firebase Authentication |
| Database   | Firebase Firestore      |
| Hosting    | Firebase App Hosting    |
| Language   | TypeScript              |

## Project Structure

```
tastyswipe-admin/
├── app/                    # Next.js App Router pages
│   ├── (auth)/             # Auth routes (login, etc.)
│   ├── dashboard/          # Main dashboard
│   ├── restaurants/        # Restaurant/recipe management
│   ├── users/              # User management
│   ├── analytics/          # Analytics & reporting
│   ├── categories/         # Categories & tags
│   ├── notifications/      # Push notifications
│   └── settings/           # Platform settings
├── components/             # Reusable UI components
│   ├── ui/                 # Base UI primitives
│   ├── charts/             # Analytics chart components
│   ├── tables/             # Data table components
│   └── layout/             # Layout components (sidebar, navbar)
├── lib/                    # Utility functions & configs
│   ├── firebase.ts         # Firebase client config
│   └── utils.ts            # General utilities
├── hooks/                  # Custom React hooks
├── types/                  # TypeScript type definitions
└── public/                 # Static assets
```

## Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn
- A Firebase project linked to TastySwipe

### Installation

```bash
# Clone the repo
git clone https://github.com/sadeeqahli/Swipes-Admin.git
cd Swipes-Admin

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Fill in your Firebase config in .env.local

# Run the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Environment Variables

Create a `.env.local` file in the root with the following:

```env
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
```

## Related

- 📱 [Swipes Mobile App](https://github.com/sadeeqahli/Swipes) — The React Native / Expo client app

## License

MIT
