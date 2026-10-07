# Thresh (🌾)

> **Real-action matchmaking, mutual aid, and community infrastructure.**

Modern dating platforms turn human connection into a disposable catalog. They exploit isolation, leaving single parents to carry households alone, fathers alienated from home, and disabled adults sidelined by superficial algorithms.

**Thresh** is open-source social infrastructure engineered to re-establish the village. It replaces endless swiping with tangible presence: connecting single parents, disabled individuals, and family-oriented singles through practical service, shared responsibilities, and genuine commitment.

Love is not a swipe. Love is a verb.

---

## 🛠 Core Pillars

- **Dual-Intent Profiles:** Profiles pair relationship intent with real-world capability:
  - *Where I Could Use a Hand:* Light home repair, mobility support, childcare coverage, tutoring, cooking.
  - *How I Offer Value:* Practical skills, handyman abilities, mechanical work, meal prep, emotional grounding.
- **Micro-Aid Action Board:** A hyper-local feed connecting verified users via low-stakes, practical tasks rather than vanity matching.
- **Radical Accessibility First:** Built from ground zero to conform strictly to WCAG 2.2 AAA accessibility standards for screen readers, high-contrast usability, and diverse motor needs.
- **Anti-Exploitation Protocols:** Built-in boundaries to prevent platform commercialization, transactional dynamics, or free-labor exploitation.

---

## 🛡 Trust, Family & Safety Architecture

Because Thresh directly interfaces with families, homes, and vulnerable individuals, safety is baked directly into the codebase:

1. **Mandatory Identity Verification:** Integrated ID check before users can exchange direct messages or post to local aid boards.
2. **"Public First" Milestone Gate:** In-person home visits are programmatically locked until a public meeting (or verified in-app video introduction) is confirmed by both parties.
3. **Child Privacy Guard:** Strict client-side and server-side image hashing/moderation preventing public child faces on dating discovery feeds.
4. **Non-Transactional Integrity:** Financial compensation features are permanently prohibited. The platform facilitates mutual aid and authentic relationship building, not gig labor.

---

## 🏗 Tech Stack

- **Framework:** Next.js 15 (App Router) / React Native (Expo)
- **Database:** PostgreSQL with PostGIS (for privacy-preserving geo-proximity matching)
- **ORM:** Prisma / Drizzle
- **Auth & ID Verification:** Auth.js (NextAuth) + Persona / Stripe Identity webhooks
- **Styling:** Tailwind CSS + Radix UI (accessible, headless design tokens)
- **State & Real-time:** tRPC + WebSockets (for secure real-time messaging)

---

## 🚀 Getting Started

### Prerequisites

- Node.js >= 20.x
- PostgreSQL >= 15
- pnpm >= 9.x

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-org/thresh.git
   cd thresh
   ```

2. **Install dependencies:**
   ```bash
   pnpm install
   ```

3. **Configure Environment Variables:**
   ```bash
   cp .env.example .env.local
   ```
   Provide your database URL, auth secrets, and identity verification API keys.

4. **Initialize Database:**
   ```bash
   pnpm prisma migrate dev --name init
   pnpm prisma db seed
   ```

5. **Run Development Server:**
   ```bash
   pnpm dev
   ```
   Open http://localhost:3000 in your browser.

---

## 📄 License
Distributed under the AGPL-3.0 License to ensure that all community infrastructure built upon Thresh remains open, transparent, and non-exploitative.
