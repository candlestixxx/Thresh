# Thresh Architecture

## Overview
Thresh is built as a Next.js (App Router) web application with an optional React Native (Expo) shell for mobile access. The application leverages PostgreSQL for data persistence with PostGIS for location-based matching (geo-proximity). It uses NextAuth for authentication, combined with identity verification hooks.

## Tech Stack
*   **Framework:** Next.js 15 (App Router)
*   **Database:** PostgreSQL (with PostGIS)
*   **ORM:** Prisma
*   **Auth:** NextAuth (Auth.js)
*   **Styling:** Tailwind CSS + Radix UI
*   **State / Real-time:** tRPC / WebSockets

## Key Components
*   **Profiles (Dual-Intent):** Representing an individual's personal intent and their practical aid offerings and needs.
*   **Micro-Aid Action Board:** A location-aware board that displays nearby requested or offered aid tasks.
*   **Identity & Verification:** Mandatory background or ID verification flows gated before accessing certain interactions.
*   **Safety Guards:** Implementation of public-first connection validations and child privacy hashing systems.
