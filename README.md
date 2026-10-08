# sync-network
A digital emergency liquidity network redefining the 'Urgent 2k' as community trust units. Built for Wema Hackaholics 7.0

## 🔗 Hackathon Submission Links
1. **Live Frontend Application:** [Insert Vercel/Netlify URL Here]
2. **Live Backend API Endpoint:** [Insert API URL Here]
3. **Recorded Loom Demo:** [Insert Loom URL Here]

---

## 1. Project Description: The "Urgent 2k" Dilemma
Everyday Nigerians frequently face micro-emergencies (transport, data, food). Currently, their only options for an "Urgent ₦2k" are begging friends (loss of dignity) or using unregulated loan apps (entering a predatory ₦5k debt trap). 

**QuickSync Network** solves this by transforming micro-loans into a community-powered liquidity network based on **Trust Units**. Inspired by how the Dangote IPO democratized ownership, we have turned the "Urgent 2k" into a low-risk, high-velocity financial reward system for the masses.

### How It Works: The Give-to-Get Priority System
* **For the Requester:** Need ₦2,000 urgently? Get matched with a community provider instantly. Identities are masked to protect user dignity.
* **For the Provider:** Have idle cash? Buy a ₦2,000 "Unit of Ownership". By helping the community, you earn Trust Points and a fast ROI.
* **The Magic:** Giving increases your points. Taking converts your points. When you consistently fund units, you build an "Excellent" Trust Score. When *you* eventually experience an emergency, the network prioritizes your request and funds you in seconds.

## 2. The Unit Economics (The 60/40 Split)
QuickSync is highly profitable on day one. Every ₦2,000 micro-unit carries a flat 5% (₦100) return.
* **The Provider** takes 60% (₦60) as their ROI.
* **The Platform** retains 40% (₦40) as a transaction fee.
* At just 10,000 micro-transactions a day, the platform generates ₦400,000 in daily revenue purely from micro-fees.

## 3. Wema Bank Integration (The ALAT Flywheel)
QuickSync is designed to be a massive, zero-CAC user acquisition and deposit-generating engine for Wema Bank:
1. **The ALAT Zero-CAC Funnel:** When a provider wants to withdraw their yield, they are prompted to route it instantly to an ALAT account (0 fees). If they don’t have one, we API-provision a Tier 1 ALAT wallet. We acquire pre-vetted, high-trust users for Wema Bank at ₦0 Customer Acquisition Cost.
2. **B2B Emergency Circles (CASA Deposits):** We provide SaaS infrastructure for universities and corporations to run their own internal emergency funds. To launch a circle, organizations must hold their liquidity pool in a Wema Corporate Account, generating massive zero-cost deposits (CASA).
3. **The Institutional Whale:** When community P2P liquidity runs low, Wema Bank’s backend acts as the algorithmic "Whale," automatically buying up ₦2k units from users with elite Trust Scores—deploying capital safely and earning the 60% provider profit at scale.

## 4. Technical Architecture & Alternative Data
* **Frontend:** Next.js, React, Tailwind CSS (Mobile-first SPA).
* **Backend:** Python / FastAPI.
* **The Trust Engine:** Instead of relying purely on backward-looking credit bureaus, our proprietary algorithm tracks high-frequency community behavior (funding speed, repayment velocity, "Pay it Forward" donations) to generate a dynamic Alternative Data Risk Score for Wema Bank.

## 5. Local Setup Instructions
To run this repository locally:

```bash
# Clone the repository
git clone [https://github.com/yourusername/quicksync-network.git](https://github.com/yourusername/quicksync-network.git)

# Navigate into the frontend directory
cd quicksync-network

# Install dependencies
npm install

# Run the development server
npm run dev
