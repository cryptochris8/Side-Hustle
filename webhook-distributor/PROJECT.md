# Form Webhook Distributor - Project Definition

## SHIPPING DEADLINE: February 7, 2026 (7 DAYS FROM START)

**Start Date**: January 31, 2026
**Ship Date**: February 7, 2026
**Status**: DAY 1 - Planning

---

## The Problem

Small businesses and marketers use form builders (Typeform, Google Forms, Webflow, etc.) but need form submissions sent to multiple places (email, Slack, Google Sheets, CRM).

**Current solutions:**
- Zapier: $20-50/mo for simple workflows
- Manual copy/paste: Time consuming
- Custom code: Too technical

**Our solution:** Simple webhook receiver that forwards form data to multiple destinations for $10-15/mo.

---

## Target Users

1. **Small business owners** (service businesses, consultants)
2. **Marketers** (managing lead forms)
3. **Freelancers** (contact forms on websites)
4. **Side hustlers** (people like you!)

**Validation needed**: Talk to 3 people who use forms and ask if they'd pay $10/mo for this.

---

## V1 Features (MAX 3 - NON-NEGOTIABLE)

### Feature 1: Receive Webhook
**What it does**: Generate unique webhook URL, accept POST requests with form data
**Why it matters**: Core functionality - without this, nothing works
**Acceptance criteria**:
- User creates account → gets unique webhook URL
- Webhook accepts any POST request with JSON or form data
- Data is stored in database

### Feature 2: Email Notifications
**What it does**: Send email when webhook receives data
**Why it matters**: Most common use case - people want email alerts
**Acceptance criteria**:
- User sets notification email address
- Email sent within 1 minute of webhook receiving data
- Email contains all form fields in plain text

### Feature 3: Webhook History
**What it does**: Simple dashboard showing received webhooks
**Why it matters**: Users need to see what was received and when
**Acceptance criteria**:
- List of webhooks (timestamp, data preview)
- Click to see full webhook payload
- Basic search/filter by date

**THAT'S IT. NOTHING ELSE IN V1.**

---

## V2 Ideas (DO NOT BUILD THESE IN V1)

- Slack integration
- Google Sheets integration
- Custom data transformations
- Webhook filtering/routing rules
- Multiple webhook URLs per account
- Team collaboration
- Analytics dashboard
- Webhook retry logic
- Data validation rules
- Export to CSV
- API access
- Zapier/Make.com integration
- Custom email templates
- SMS notifications
- CRM integrations (HubSpot, Salesforce, etc.)

---

## Tech Stack (Keeping it SIMPLE)

**Framework**: Next.js 14 (App Router)
**Database**: Supabase (Postgres + Auth included)
**Styling**: Tailwind CSS + shadcn/ui
**Email**: Resend (simple API, generous free tier)
**Hosting**: Vercel (one-click deploy from Git)
**Payments**: Stripe (just a payment link for V1)

**Why this stack:**
- One framework for frontend + backend (Next.js API routes)
- Supabase gives us database + auth out of the box
- Vercel deploys automatically from Git
- Everything has excellent docs

---

## Pricing (V1)

**Free Tier:**
- 100 webhooks/month
- 1 webhook URL
- Email notifications only

**Pro Tier: $10/month**
- 10,000 webhooks/month
- 5 webhook URLs
- Email notifications
- 30-day webhook history

**V2 can add higher tiers with more integrations**

---

## 7-Day Build Plan

### Day 1 (Jan 31): Planning & Setup
- [x] Define 3 core features
- [ ] Validate with 2-3 potential users (quick chats)
- [ ] Initialize Next.js project
- [ ] Set up Supabase
- [ ] Basic auth (sign up/login with Supabase)

### Day 2 (Feb 1): Core Webhook Feature
- [ ] Create API route to receive webhooks
- [ ] Generate unique webhook URLs per user
- [ ] Store webhook data in Supabase
- [ ] Test with Postman/curl

### Day 3 (Feb 2): Email Notifications
- [ ] Integrate Resend for email
- [ ] User can set notification email
- [ ] Send email when webhook received
- [ ] Test end-to-end flow

### Day 4 (Feb 3): Dashboard UI
- [ ] Landing page (copy template, no custom design)
- [ ] Dashboard: List webhooks
- [ ] Dashboard: View webhook details
- [ ] Basic styling with Tailwind

### Day 5 (Feb 4): Auth & Polish
- [ ] Complete auth flow (signup/login/logout)
- [ ] User settings page (notification email)
- [ ] Copy webhook URL button
- [ ] Basic error handling

### Day 6 (Feb 5): Deploy & Test
- [ ] Deploy to Vercel
- [ ] Set up environment variables
- [ ] Test production deployment
- [ ] Fix critical bugs only

### Day 7 (Feb 6): Payment & Launch Prep
- [ ] Create Stripe payment link
- [ ] Add simple paywall (free tier limits)
- [ ] Write launch post for Reddit
- [ ] Test with real form builder (Typeform/Google Forms)

### Feb 7: LAUNCH DAY
- [ ] Post on r/SideProject, r/Entrepreneur
- [ ] Tweet about it
- [ ] Email/message potential users
- [ ] Monitor for issues

---

## Success Metrics (V1)

- **Shipped by Feb 7**: YES/NO
- **Features built**: 3 (no more, no less)
- **First user signup**: Within 7 days of launch
- **First paying customer**: Within 30 days of launch

**Don't measure in V1:**
- Code quality
- Performance
- Design beauty
- Edge case handling

---

## Perfectionism Red Flags

If I catch myself doing ANY of these, STOP:

- ❌ Adding Slack integration in V1
- ❌ Custom email templates (plain text is fine)
- ❌ Advanced error handling (basic try/catch is enough)
- ❌ Webhook retry logic (V2 feature)
- ❌ Data validation beyond basic checks
- ❌ Beautiful dashboard design (functional > pretty)
- ❌ Writing tests (add after revenue)
- ❌ Rate limiting (add when you have scale problems)
- ❌ Multiple webhook URLs per user (V2)
- ❌ Custom domain for webhooks (V2)

---

## Emergency Brake

If by Day 5 I'm not done with the core features, I will:
1. Cut Feature 3 (Dashboard) to bare minimum (just a list)
2. Remove all nice-to-haves
3. Ship with bugs (document them for V2)

**Better to ship something working than nothing perfect.**

---

## Launch Plan

**Where to post:**
- r/SideProject
- r/Entrepreneur
- r/smallbusiness
- r/webdev (Show & Tell Saturday)
- Indie Hackers
- Twitter/X
- Product Hunt (maybe V2)

**Message:**
"I built a simple webhook forwarder because Zapier is too expensive for simple form notifications. $10/mo, no fluff. Looking for beta users."

---

## Validation Questions (Ask 3 people TODAY)

1. Do you use forms on your website/business?
2. What do you do with form submissions now?
3. Do you wish they went somewhere else automatically?
4. Would you pay $10/mo for automatic forwarding to email/Slack/Sheets?

**If 2/3 say yes, BUILD IT.**
**If 0/3 say yes, PIVOT or pick different idea.**

---

## Notes

- Keep it simple
- Ugly and shipped > perfect and hidden
- V1 is for learning, V2 is for revenue
- Ship by Feb 7 NO MATTER WHAT

**LET'S GO.**
