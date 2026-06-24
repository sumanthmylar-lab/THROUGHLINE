# Throughline — Mobile Design Brief

> **How to use this file:** Upload it to Claude Design and paste this prompt:
> *"Use this brief to design a polished, high-fidelity mobile app prototype (iOS, light mode, ~390px wide frames). Start with the 4 core mentee screens, then the mentor screen. Follow the design tokens and art direction exactly, use the real copy and sample data provided — no lorem ipsum — and make the 'continuity thread' the signature element. Keep everything else quiet and disciplined."*

---

## 1. The product in one breath
**Throughline** is a mobile app for keeping a valuable mentor–mentee relationship alive *after one person changes jobs*. The mentor publishes a few open time slots; the mentee books one in two taps; both get a reminder; and a shared history thread holds the context together over the years.

**Tagline:** *Keep the people who shaped your career — even after they leave.*

## 2. Audience & core insight
- **Who:** working professionals (25–45) who built a trusted 1:1 mentoring bond at a company, then one of them moved on.
- **The pain it kills:** LinkedIn messages get missed, people won't swap phone numbers, emails get lost — so good relationships quietly drift apart.
- **The one insight the whole design must express:** *the relationship is the constant; the job is the variable.* Companies change, the throughline doesn't.

## 3. Art direction
Warm, calm, premium, personal — a trusted professional keepsake, **not** a cold SaaS dashboard and **not** a flashy consumer-social app. Confident and quiet, with one memorable signature.

**Do**
- Warm off-white canvas, deep-navy ink, a single honey/amber accent used sparingly for warmth and for the "thread."
- Generous spacing, soft rounded corners (cards 16px, buttons 11–13px), gentle shadows.
- Real, human microcopy (provided below). Sentence case. Active voice.

**Don't (avoid the generic AI look)**
- No cream-background + high-contrast serif + terracotta cliché.
- No near-black background with an acid-green accent.
- No big-number hero, no decorative 01/02/03 numbering.
- No stocky gradients or emoji.

## 4. Design tokens

**Color**

| Token | Hex | Use |
|---|---|---|
| bg | `#F5F2EC` | App background (warm off-white) |
| surface | `#FFFFFF` | Cards, sheets |
| ink | `#1B2840` | Primary text, dark buttons, phone bezel |
| inkMuted | `#5C6478` | Secondary text |
| subtle | `#938C7E` | Captions, meta, icons |
| accent | `#D98E2B` | Honey accent — the "thread," key icons, highlights |
| accentDeep | `#B5731C` | Accent text on light |
| accentSoft | `#FBEEDA` | Accent chip/selected backgrounds |
| green | `#4F8A6B` | Confirmed / booked / active |
| greenSoft | `#E5F0E9` | Confirmed backgrounds |
| line | `#EAE4DA` | Borders, dividers |
| lineSoft | `#F1ECE3` | Faint dividers |

**Avatars** (initials on solid circle, cycle): `#C97B4A`, `#4F8A6B`, `#5B6FA8`, `#A8557B`, `#7A8A4F`

**Type** — system sans (SF Pro / -apple-system). Scale: screen title 23/700, section header 17/600, card name 15.5/600, body 14/500, meta 12.5–13/500, eyebrow 12/600 uppercase +0.05em tracking. Tighten large headings to -0.02em.

**Shape & motion** — radii: cards 16, buttons 11–13, chips 9–11, pills 20. Shadows soft and low. Micro-interactions only: slot select highlight, button press, toast slide-up, nudge dismiss.

## 5. Signature element — the continuity thread
On each person's detail screen, a vertical timeline connected by a continuous **honey-colored thread** (2px, ~40% opacity). Three node types:
- **Session** (filled navy dot) — a past conversation + one-line note.
- **Career move** (larger honey dot with a soft ring; italic honey text) — e.g., *"Priya moved from Stripe → Figma."* The thread runs **straight through** it, unbroken — this is the emotional core.
- **Origin** (hollow ring, honey outline) — where the two people first met.

Close the thread with a quiet caption: *"The thread holds even when the job changes — that's the whole point."*

## 6. Screens to design

### A. Connections (mentee home) — *priority 1*
- **Header:** greeting "Good morning, Maya" + title "Your throughlines."
- **Nudge card** (dark navy, dismissible): eyebrow "KEEP THE THREAD" with a spark icon → "It's been **9 weeks** since you and Priya talked. Worth grabbing 30 minutes before it drifts?" → honey button "Book time with Priya →".
- **Relationship list:** card per person — avatar, name, "role · company" with a briefcase icon, and either a green "Next: …" chip or muted "Last met …".
- **Roadmap teaser** (dashed, muted): "Find new mentors — People open for mentorship · coming soon."

### B. Relationship detail — *priority 1 (hero screen)*
- Back chevron; person header: large avatar, name, "role · company," and a subtle "You met at Stripe, 2023."
- **Goal chips** in accentSoft (e.g., "Grow into design leadership").
- **Primary action:** if no session booked → dark "Book your next session" button (honey calendar icon). If booked → green "Next session booked" card with time + "Reminder set" + bell.
- Secondary ghost button: "Send a note."
- **The continuity thread** (section 5).

### C. Book a session — *priority 1*
- Title "Book with Priya." Intro line: "Priya keeps a few slots open for the people they mentor. Pick one that works — you'll both get a reminder."
- Day groups (calendar icon + "Tue, Mar 25"), each with time-slot buttons (clock icon). Selected slot → accentSoft fill + honey border.
- Sticky bottom bar: dark "Confirm [time] →" button, disabled until a slot is chosen.
- On confirm → toast "Session booked — you'll both get a reminder" and return to detail in the booked state.

### D. Mentor home — *priority 2*
- Title "Your availability"; sub "You're mentoring 6 people."
- **Weekly availability pills** (toggle on/off, check when on): Tue 5:00 PM, Wed 12:00 PM, Fri 9:00 AM, Fri 4:00 PM, Mon 6:00 PM.
- **Incoming request card:** "Maya Chen wants to talk — Tue, Mar 25 · 5:00 PM" → "Accept" / "Not this week." Accepted → green confirmed row.
- **Coming up** list: mentee avatar, name, time, video icon.

### Roadmap screens — *priority 3, optional*
Onboarding (claim your identity not tied to a work email), async "Send a note," and "Discover / open for mentorship" (the influencer-mentor direction).

## 7. Copy bank (use verbatim)
- App: **Throughline** · Tagline: *Keep the people who shaped your career — even after they leave.*
- Home title: *Your throughlines* · Greeting: *Good morning, Maya*
- Nudge: *It's been 9 weeks since you and Priya talked. Worth grabbing 30 minutes before it drifts?* · Button: *Book time with Priya*
- Detail actions: *Book your next session* / *Next session booked* / *Reminder set* / *Send a note*
- Booking intro: *Priya keeps a few slots open for the people they mentor. Pick one that works — you'll both get a reminder.*
- Toast: *Session booked — you'll both get a reminder*
- Thread caption: *The thread holds even when the job changes — that's the whole point.*
- Mentor: *Your availability* / *Tap the weekly slots you're happy to keep open. The people you mentor can book these — no back-and-forth.* / *Maya Chen wants to talk* / *Not this week* / *Coming up*

## 8. Sample data (use real, not placeholders)

**The user (mentee):** Maya Chen

**Mentors**
1. **Priya Nair** — Design Director · Figma · met at Stripe, 2023 · last met 9 weeks ago · no session booked. Goals: *Grow into design leadership*, *Navigate the first director role.* Thread (newest→oldest): Mar 14 session "Giving hard feedback to senior reports" · **Jan 2025 move "Priya moved from Stripe → Figma"** · Dec 8 session "Mock panel for your promo case" · Oct 2 session "First catch-up after you left Stripe" · 2023 origin "You met at Stripe." Open slots: Tue Mar 25 (5:00, 5:30 PM), Wed Mar 26 (12:00 PM), Fri Mar 28 (9:00 AM, 4:00 PM), Mon Mar 31 (6:00 PM).
2. **Daniel Osei** — VP Engineering · Notion · met at your first job, 2019 · last met 3 weeks ago · **Next: Thu, Mar 27 · 4:30 PM.** Goal: *Move from IC to management.*
3. **Lena Fischer** — Product Lead · Duolingo · met at Google, 2021 · last met 6 weeks ago. Goal: *Break into product management.*

**Mentor view (as Priya):** upcoming — Maya Chen (Thu, Mar 27 · 4:30 PM), Tomas Reyes (Fri, Mar 28 · 9:00 AM).

## 9. Deliverables
1. Four mentee frames (Connections, Detail, Book, Detail-booked/toast) + one mentor frame, iOS light mode, ~390px wide.
2. The reusable component set: avatar, relationship card, nudge card, goal chip, slot button, availability pill, confirmed/booked card, toast, thread node.
3. Spend the boldness on the continuity thread; keep everything else calm.
