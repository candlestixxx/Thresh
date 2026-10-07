# DEPLOY

## Current Deployment Instructions

### Prerequisites
*   Node.js (v20+)
*   PostgreSQL (v15+) with PostGIS extension (if location matching requires geospatial queries)
*   pnpm (v9+)

### Local Development Setup
1. Clone the repository.
2. Run `pnpm install` to grab dependencies.
3. Copy `.env.example` to `.env.local` and configure your local Postgres credentials (`DATABASE_URL`).
4. Run `pnpm prisma migrate dev --name init` to initialize your local database.
5. (Optional) Run `pnpm prisma db seed` if seed data is available.
6. Run `pnpm dev` to start the Next.js development server.

### Production Environment Variables Needed
*   `DATABASE_URL`: Connection string for production Postgres.
*   `NEXTAUTH_SECRET`: Secure random string for session tokens.
*   `NEXTAUTH_URL`: Canonical URL for the production app.
*   `STRIPE_SECRET_KEY` / Identity keys: For real user verification webhooks.
