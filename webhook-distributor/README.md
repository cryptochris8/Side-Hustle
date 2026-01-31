# Webhook Distributor

**Status**: 🚧 Day 1 of 7-day build
**Ship Date**: February 7, 2026
**Current Focus**: Planning & Validation

---

## What It Does

Receives webhooks from forms and forwards them to multiple destinations (email, Slack, Google Sheets, etc.).

**Think**: Simpler, cheaper Zapier for form submissions.

---

## V1 Features (Shipping Feb 7)

1. ✅ Receive webhook at unique URL
2. ✅ Send email notifications
3. ✅ View webhook history

**That's it. Nothing else.**

---

## V2 Ideas (After Launch)

- Slack integration
- Google Sheets sync
- Custom transformations
- Multiple webhook URLs
- Analytics

---

## Tech Stack

- Next.js 14 (App Router)
- Supabase (Database + Auth)
- Tailwind CSS + shadcn/ui
- Resend (Email)
- Vercel (Hosting)
- Stripe (Payments)

---

## Pricing

**Free**: 100 webhooks/month
**Pro ($10/mo)**: 10,000 webhooks/month

---

## Current Progress

See PROJECT.md for detailed build plan and daily progress.

---

## Anti-Perfectionism Reminder

If it's not one of the 3 core features, it's a V2 feature. Ship first, polish later.
