# QuickSync ⚡️ Soro
**The Voice-Native Emergency Liquidity Network (Powered by Wema Bank)**
*Built for Hackaholics 7.0*

## 🔗 Hackathon Submission Links
1. **Live Frontend Application (Command Center):** [Insert Vercel/Netlify URL Here]
2. **Live Backend API Endpoint (Soro Engine):** [Insert API URL Here]
3. **Recorded Loom Demo:** [Insert Loom URL Here]

---

## 1. Project Description: The Ultimate Financial Inclusion Engine
Everyday Nigerians frequently face micro-emergencies (the "Urgent 2k"). Currently, their only options are begging friends or using unregulated loan apps that rely on predatory debt traps and public shame. Furthermore, existing digital solutions require smartphones and internet access, locking out the bottom of the pyramid.

Our solution merges two powerful engines: **QuickSync** (The Liquidity Network) and **Soro** (The Conversational Voice Layer).

### A. The QuickSync Liquidity Network (The Engine)
QuickSync transforms micro-loans into a community-powered liquidity network based on **Trust Units**. 
* **Lenders / B2B Partners** use our sleek Web App to buy ₦2,000 "Units of Ownership." 
* Every unit carries a 5% return. We use a **60/40 Revenue Split**: The lender earns 60% (₦60) plus Trust Points, and the platform retains 40% (₦40).
* By giving liquidity, lenders earn "Priority Trust," guaranteeing they get funded instantly when they face their own emergencies.

### B. Soro Conversational AI (The Accessibility Layer)
Borrowers do not need to download an app. They simply call our toll-free number.
* **Voice-Native:** Our AI, Ayo, speaks Yoruba, Nigerian Pidgin, and English. A market woman can naturally say, "Ayo, I need 2k for market goods."
* **Deterministic Security:** Soro holds no funds and gives AI *zero* authority over money. AI only parses intent. The deterministic Fastify backend handles policy, executes the transfer via Wema Bank, and uses highly secure **DTMF keypad PIN authorization** (never sent to the LLM).

## 2. Wema Bank Integration (The ALAT Flywheel)
1. **The ALAT Zero-CAC Funnel:** When a web lender withdraws their QuickSync yield, they are routed to ALAT (Instant + 0 Fees). If they don’t have an account, we API-provision a Tier 1 ALAT wallet. We acquire pre-vetted, high-trust users for Wema Bank at ₦0 Customer Acquisition Cost.
2. **The Institutional Whale:** When community P2P liquidity runs low, Wema Bank’s backend acts as the algorithmic "Whale," automatically funding Soro voice requests from users with elite Trust Scores—deploying capital safely and earning the 60% profit at scale.

## 3. Architecture at a Glance
**Frontend (Lender Dashboard):** Next.js, React, Tailwind CSS.
**Backend (Soro Engine):** Node 24, Fastify, SQLite, Twilio.
* *Flow:* Phone → Twilio (live) / Scenario Engine (demo) → Voice Layer (Ayo) → Intent + Context → Policy + Validation (DTMF PIN) → Banking Engine → Wema Adapter → Command Center Web App.

## 4. The Forward Deployed Team
* **Ayomide** – Product Developer
* **Daniel** – Technical Lead
* **Abraham** – Business Developer
* **Victoria** – Design Lead
* **Emmanuel** – User Experience (UX) Lead
---

## 5. Local Setup & Quick Start (Soro Backend)
To run the deterministic AI backend and simulated Wema banking core locally:

```bash
# Ensure correct environment
nvm use && corepack enable          # Node 24.19.0, PNPM 11.22.0

# Setup Environment
cp .env.example .env

# Install Dependencies
pnpm install

# Check & Build
pnpm typecheck && pnpm lint && pnpm test && pnpm build

# Seed Local SQLite Demo Data
pnpm db:reset && pnpm db:seed       

# Start the Fastify API
pnpm --filter @soro/api start        # http://localhost:3000
```

### Run a Local Scenario Test (No Twilio required)
```bash
curl -s -X POST localhost:3000/api/demo/run-scenario   -H 'content-type: application/json'   -d '{"phone":"08030000001","turns":["I need an urgent 2k for transport","yes"],"demoPin":"1234"}'
```
*Note: Demo Mode utilizes simulated banking data but runs through the real engine path with strict security validations.*
