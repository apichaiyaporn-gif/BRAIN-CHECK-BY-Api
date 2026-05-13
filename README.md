# BRAIN-CHECK-BY-Api
BRAIN CHECK
# Dementia Care Platform

A production-ready starter for a mobile-first healthcare web app covering:

- AD8 → Mini-Cog → MoCA → MMSE/TMSE → ADL → IADL
- patient registry
- risk scoring
- care plan workflow
- alerts and notifications
- auth + RBAC
- deployable on Vercel + PostgreSQL

## Quick start

1. Copy `.env.example` to `.env`
2. Set `DATABASE_URL` and `JWT_SECRET`
3. Install deps:
   ```bash
   npm install
   ```
4. Push schema:
   ```bash
   npm run db:push
   ```
5. Seed demo data:
   ```bash
   npm run seed
   ```
6. Run locally:
   ```bash
   npm run dev
   ```

## Deployment

### Vercel
- Deploy the Next.js app to Vercel
- Set environment variables:
  - `DATABASE_URL`
  - `JWT_SECRET`
  - `NEXT_PUBLIC_BASE_URL`
- Use a managed PostgreSQL database

### Domain
- Point your domain to Vercel
- Add the domain in Vercel project settings
- Update `NEXT_PUBLIC_BASE_URL`

### Important
- MoCA / MMSE / TMSE full instruments may be licensed in some contexts. This scaffold keeps the scoring and workflow architecture configurable so your clinical team can plug in the approved version.
