# TicketWala — Landing Page Spec

## Purpose
A static single-page website deployable on GitHub Pages. Goal is to:
- Explain what TicketWala is and why it exists
- Build early waitlist signups (email capture)
- Feel trustworthy and modern to urban Indian users (22–45)
- Work beautifully on mobile (primary device for the target audience)

---

## Brand Identity

| Attribute | Decision |
|---|---|
| **Name** | TicketWala |
| **Tagline** | *"Book train tickets on WhatsApp. No portal. No hassle."* |
| **Tone** | Friendly, confident, desi — Hindi/English mix where it adds personality |
| **Primary Color** | WhatsApp Green `#25D366` |
| **Accent Color** | IRCTC/Indian Railway saffron-orange `#FF6B35` |
| **Background** | Off-white `#F9FAFB` with dark sections `#0F172A` |
| **Font** | Inter (Google Fonts) — clean, modern, widely supported |
| **Logo/Icon** | 🚂 + WhatsApp bubble concept (text-based in v1) |

---

## Page Sections (Top → Bottom)

### 1. Navbar
- Logo: "🚂 TicketWala" wordmark
- Nav links: How it Works · Features · Pricing
- CTA button: "WhatsApp Us" (sticky on scroll, links to wa.me)

---

### 2. Hero Section
- **Headline:** "Book Train Tickets by Sending a WhatsApp Message"
- **Sub-headline:** "TicketWala connects to your IRCTC account and books tickets for you — just tell it where you want to go."
- **CTA:** "Coming Soon — Chat with us on WhatsApp →" (links to wa.me)
- **Trust badge:** "Powered by Claude AI · Built for India · DPDP Compliant"
- **Visual:** Mock WhatsApp chat UI showing a sample conversation (e.g. user types "Delhi to Mumbai this Friday, sleeper" and TicketWala confirms the booking)

---

### 3. The Problem (Why TicketWala Exists)
- Short 2–3 line narrative: IRCTC portal is frustrating, captchas, slow, mobile-unfriendly
- Three pain point cards:
  - 😤 "Captchas at 10 AM on Tatkal day"
  - 🤯 "20 steps to book one ticket"
  - 📵 "App crashes when you need it most"

---

### 4. How It Works (3 Steps)
Step-by-step visual flow:

1. **Connect Once** — Link your IRCTC account to TicketWala securely (one time setup)
2. **Message Naturally** — Tell TicketWala where you're going, in Hindi or English
3. **Done. Ticket Booked.** — Get your booking confirmation right on WhatsApp

---

### 5. Features Grid
Six feature cards:

| Feature | Description |
|---|---|
| 💬 Natural Language | Type like you'd text a friend — "Mumbai to Pune Friday evening, 2A" |
| 🇮🇳 Hindi + English | Seamlessly understands Hinglish |
| 🔒 Secure by Design | IRCTC credentials encrypted with AWS KMS, never stored in plaintext |
| 📍 India-Only Servers | All data stays in AWS Mumbai (DPDP Act compliant) |
| ⚡ Instant Confirmation | Booking confirmation sent to you on WhatsApp |
| 🔎 Smart Station Search | Type "Bombay" or "VT" — TicketWala figures it out |

---

### 6. Pricing
Simple and transparent:

- **Convenience Fee:** ₹25–40 per booking
- **No subscription. No hidden charges.**
- Paid via UPI link sent on WhatsApp after confirmation
- Small print: IRCTC ticket cost is separate and paid directly to IRCTC

---

### 7. CTA Section (Full-width)
- Heading: "TicketWala is coming soon"
- Sub-text: "We're putting the finishing touches. Follow along or reach out directly."
- Single CTA button: "Chat with us on WhatsApp →" (links to `https://wa.me/91XXXXXXXXXX`)

---

### 8. Footer
- Logo + tagline
- Links: Privacy Policy · Terms · Contact (sharma18yash.ys@gmail.com)
- "Made with ❤️ in India"
- Social: GitHub icon (links to repo)

---

## Technical Constraints (GitHub Pages)
- Single `index.html` file — no build step, no framework
- All CSS inline or in a `<style>` block
- No forms, no backend — all CTAs are `wa.me` WhatsApp links
- Fonts via Google Fonts CDN
- Fully responsive (mobile-first)
- No cookies, no tracking scripts
- WhatsApp chat mockup built in pure HTML/CSS (no images required)

---

## What It Is NOT (v1 Scope)
- No live booking demo
- No login / dashboard
- No Tatkal section (product doesn't support it yet)
- No blog or press kit

---

## Deliverable
`index.html` — drop into a GitHub repo, enable Pages, done.
