# Example PRD - Full App Spin-Up

## Overview

Build a complete, production-ready web app with authentication, a public marketing site, and a signed-in dashboard. Use a modern stack, ship a clean UI, and include tests and deployment docs.

## Decisions

- Framework: Next.js (App Router)
- Language: TypeScript
- Styling: Tailwind CSS
- Database: Postgres (Prisma)
- Auth: NextAuth
- Deployment: Vercel

## Requirements

- App should run locally with `pnpm dev` and `pnpm test`.
- All routes should have basic loading and error states.
- Use environment variables stored in `.env.local`.

## Tasks

### 1) Project Scaffold
- [ ] Initialize Next.js app with TypeScript, Tailwind, and ESLint
- [ ] Add Prisma setup with Postgres config
- [ ] Add environment template and example values
- [ ] Add base app layout with global styles

### 2) Public Marketing Site
- [ ] Create landing page with hero, feature grid, and CTA
- [ ] Add pricing section with 3 tiers
- [ ] Add FAQ section
- [ ] Add footer with navigation and social links

### 3) Auth + User Model
- [ ] Add NextAuth with GitHub provider
- [ ] Create Prisma User model and migrate
- [ ] Add sign-in/sign-out UI states
- [ ] Protect dashboard routes with middleware

### 4) Dashboard MVP
- [ ] Create `/app/dashboard` with summary cards
- [ ] Add recent activity list with mock data
- [ ] Add settings page with profile form
- [ ] Add empty states for missing data

### 5) Data Layer
- [ ] Add Prisma client with singleton pattern
- [ ] Add seed script for development data
- [ ] Add basic CRUD for a `Project` model

### 6) Testing
- [ ] Add unit testing with Vitest
- [ ] Add integration tests for auth flow
- [ ] Add linting + formatting scripts

### 7) Deployment + Docs
- [ ] Add Vercel deployment instructions
- [ ] Add required env var list to README
- [ ] Add production build script

## Acceptance Criteria

- `pnpm dev` starts the app without errors
- Landing page renders and CTA navigates to sign-in
- Authenticated users can access the dashboard
- Database migrations run successfully
- Tests pass with `pnpm test`

## Notes

- Keep UI clean and modern; avoid placeholder lorem ipsum.
- Prefer server components where possible, and keep client components minimal.
- Use accessible markup and semantic HTML.
