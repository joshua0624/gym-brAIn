# Gym Brain - AI Workout Tracker

A full-stack workout tracking application with AI-powered workout planning and real-time progress analytics.

**🔗 Live Demo:** [gym-brain-omega-pearl.vercel.app](https://gym-brain-omega-pearl.vercel.app/login)

## Features

- **AI Workout Planning** - Conversational AI generates personalized workout plans based on user goals and fitness level
- **Real-Time Tracking** - Log sets, reps, and weight with immediate feedback and mid-workout coaching
- **Progress Analytics** - Visual charts tracking strength gains, volume, and workout consistency over time
- **Custom Exercises** - Create and save custom exercises with form notes and target muscle groups
- **Smart Summaries** - AI-generated workout summaries analyzing performance and suggesting adjustments

## Tech Stack

**Frontend:** React 18, TypeScript, Tailwind CSS, shadcn/ui  
**Backend:** Supabase (PostgreSQL, Auth, Real-time subscriptions)  
**AI:** OpenAI API for workout generation and coaching  
**Deployment:** Vercel

## Architecture Highlights

- Type-safe API layer with TypeScript interfaces for all database operations
- Row-level security policies ensuring users only access their own data
- React Query for optimistic updates and cache management
- Mobile-first responsive design with progressive enhancement
- Error boundaries and loading states for improved UX

## Project Structure

```
src/
├── components/     # UI components organized by feature
├── lib/           # API clients (Supabase, OpenAI) and utilities
├── hooks/         # Custom React hooks for data fetching
├── pages/         # Route components
└── types/         # TypeScript definitions
```

## Key Implementation Details

**Data Persistence:** Supabase PostgreSQL with automatic profile creation via database triggers

**State Management:** TanStack Query for server state, React Context for auth state

**AI Integration:** Streaming responses from OpenAI API with error handling and fallback strategies

**Authentication:** Supabase Auth with email/password, automatic session management

## Local Development

```bash
# Clone and install
git clone <repo-url>
npm install

# Set up environment variables (see env.example)
cp env.example .env

# Run database setup in Supabase SQL Editor
# (see complete-database-setup.sql)

# Start dev server
npm run dev
```

Requires Node.js 18+, Supabase account, and OpenAI API key.

## Screenshots

Dashboard:
<img width="1902" height="909" alt="image" src="https://github.com/user-attachments/assets/073ee6c7-eeb9-4e97-b176-7c7932997901" />

Workout History:
<img width="1904" height="905" alt="image" src="https://github.com/user-attachments/assets/5a3ce563-d81f-405f-b87d-dc42f4715d9c" />

Mid-workout:
<img width="1903" height="909" alt="image" src="https://github.com/user-attachments/assets/2aa3db61-0326-42e0-9798-ff45dc23512d" />





---

**Built by Joshua Stratton** | [LinkedIn](https://linkedin.com/in/joshua-stratton-b2ab07354) | joshua@robotics.net
