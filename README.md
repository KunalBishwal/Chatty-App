Chatty Application

A premium, full-stack real-time chat application built with Next.js, Convex, and Clerk.

## 🚀 Features

### Core Functionality
- **Authentication**: Secure sign-up/login via Clerk (Email & Social).
- **Real-time Messaging**: Instant message delivery using Convex subscriptions.
- **Presence System**: Real-time online/offline indicators with a green-dot system.
- **Typing Indicators**: Pulsing "Alex is typing..." animations that fade after 2 seconds.
- **Unread Tracking**: Real-time badges for unread messages that clear automatically.

### Enterprise-Grade Optimizations
- **High-Performance Search**: convex **Search Indexes** for O(log N) user discovery.
- **Instant Sidebar Rendering**: Denormalized `lastMessage` data for O(1) conversation listing (N+1 Refactor).
- **Real Media Sharing**: Real-time photo sharing powered by **Convex File Storage**.
- **Interactive Links**: Automated URL detection and clickable link rendering.

## 🛠 Tech Stack

- **Frontend**: Next.js (App Router), Tailwind CSS, Framer Motion, Lucide Icons.
- **Backend/Database**: Convex (Serverless functions & Real-time DB).
- **Authentication**: Clerk.

## 🏁 Getting Started

### 1. Variables Setup
Create a `.env.local` file with the following variables:
```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=...
CLERK_SECRET_KEY=...
NEXT_PUBLIC_CONVEX_URL=...
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Run Development Server
```bash
npm run dev
```

### 4. Setup Convex
```bash
npx convex dev
```

## 📜 License

This project is licensed under the [MIT License](LICENSE).
