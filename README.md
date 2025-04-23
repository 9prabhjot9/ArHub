# ArHub— Decentralized Community News Platform on Arweave

A token-curated, community-driven short news aggregator for the Arweave ecosystem.

---

## 🌟 Core Features

### 🔐 Frontend (Web App)

- **ArConnect Wallet Authentication**
- **Role Selection:**
  - 🗞️ **Publisher** – Share short news updates about Arweave and the community
  - 👍 **Voter** – Like (vote on) posts by purchasing tokens

### 📰 Posting & Voting

- **Post Creation:**
  - Publish short, Inshorts-style updates (text + optional image)
  - Posting requires a small AR fee (e.g., 0.01 AR)
- **Tokenized Likes:**
  - Each post has its own token contract
  - First voter sets the initial like price (default: 0.01 AR)
  - Each subsequent like increases the token price (bonding curve)
  - Tokens are locked for 24 hours

### 💸 Token Economy & Rewards

- **Early Voters Benefit:**
  - Early voters can sell their tokens after 24h for a higher price if the post is popular
- **Reward Distribution:**
  - 70% of total AR collected goes to the post creator
  - 27% goes to early voters (proportional to token holdings)
  - 3% platform fee (maintenance, development)
- **Trust & Curation:**
  - Posts with more tokens/votes are considered more trustworthy
  - Voters can earn reputation badges for successful curation

---

## 🧠 Backend & Smart Contract Logic

- **SmartWeave Contracts:**
  - Each post = unique token contract
  - Handles price curve, token minting, locking, and reward distribution
- **AO Integration:**
  - AO processes update token prices and manage auctions in real-time
- **Arweave Permanent Storage:**
  - All posts, votes, and transactions are stored permanently
  - Metadata includes content hash, voting history, and price evolution

---

## 🛠️ Technical Stack

| Layer      | Tech Stack                       |
|------------|----------------------------------|
| Frontend   | React, TypeScript, ArConnect SDK |
| Backend    | Node.js, AO.js SDK               |
| Storage    | Arweave, Bundlr                  |
| Contracts  | SmartWeave                       |
| Compute    | AO Processes                     |
| DevOps     | GitHub Actions, ArNS             |

---

## 🔄 MVP Workflow

### 🗞️ Post Submission

1. User logs in with ArConnect
2. Publishes a news update (text + optional image)
3. Pays 0.01 AR (base fee)
4. Post is stored permanently on Arweave

### 👍 Voting Phase

1. First voter sets the initial token price (e.g., 0.01 AR)
2. Each new like increases token price (bonding curve, e.g., +12% per vote)
3. Tokens are locked for 24 hours

### 💰 Settlement

1. After 24h, tokens unlock
2. Early voters can sell tokens at the final price
3. Rewards distributed:
   - 70% to the post creator
   - 27% to early voters
   - 3% platform fee

---

## 📊 Example Use Case

1. Alice posts “AO Network hits $600M TVL”
2. Bob likes the post first at 0.01 AR
3. 50 users like the post over 24 hours
4. Final token price: `0.01 × (1.12)^49 ≈ 18.57 AR`
5. Distribution:
   - Alice: 70% of 92.85 AR = 65 AR
   - Bob: Sells token at 18.57 AR (high ROI)
   - Platform: 2.79 AR

---

## ⚡️ Why ArHub?

- **Token-curated trust:** Aligns incentives for quality news and curation
- **Permanent, censorship-resistant storage:** Powered by Arweave
- **Early adopter rewards:** Incentivizes fast, accurate community updates
- **Web3 UX:** Seamless onboarding with ArConnect

---

## 📅 Development Timeline (1–2 Weeks)

| Day(s) | Task                                  |
|--------|---------------------------------------|
| 1–2    | Frontend setup (login, dashboards)    |
| 3–4    | Smart contract & AO integration       |
| 5–6    | Token logic, Arweave logging          |
| 7–8    | Demo use case testing                 |
| 9–10   | UI polish & pitch deck                |

---

## 🚀 Get Involved

- **Contribute:** PRs and feedback welcome!
- **Join the community:** [Discord](#) | [Twitter](#)
- **Demo:** Coming soon!

---

**This MVP shows the power of Arweave and AO for decentralized, community-driven news. Hackathon-ready, with room to grow into a full ecosystem for trustless, token-curated information.**
