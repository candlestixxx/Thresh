# MEMORY

## Internal Architectural Observations

*   **Database Schema:** The Prisma schema successfully structures `User`, `TaskAidPost`, `UserNeed`, `UserOffer`, and `Interaction`. It maps out necessary states like parenting status and task categories to fulfill dual-intent profile goals.
*   **Safety Integration:** The architecture intentionally places gates at the database/API level for things like unverified interactions. The design enforces meeting before unlocking more complex, home-oriented actions.
*   **Accessibility Priority:** Accessibility should not just be visual but baked into semantic HTML structure across the app router components to meet strict AAA goals.
*   **Monetization Ban:** We must intentionally omit any standard gig-labor payment hooks. This platform strictly trades in social currency/mutual aid.
