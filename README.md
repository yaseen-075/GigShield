# 🛡️ GigShield
### AI-Powered Parametric Income Protection for India's Gig Delivery Workers

![Phase](https://img.shields.io/badge/Phase-1%20%7C%20Ideation-blue?style=for-the-badge)
![Stack](https://img.shields.io/badge/Stack-Node.js%20%7C%20React%20%7C%20FastAPI-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)
![Hackathon](https://img.shields.io/badge/Guidewire-DEVTrails%202026-orange?style=for-the-badge)

---

> **"GigShield predicts high-risk days before they arrive and offers riders a one-tap coverage upgrade — with full transparency on cost and payout, and zero obligation."**

---

## 📋 Table of Contents
- [The Problem](#-the-problem)
- [Our Solution](#-our-solution)
- [Persona & Scenarios](#-persona--scenarios)
- [Unique Feature — Earnings Forecast Shield](#-unique-feature--earnings-forecast-shield)
- [Parametric Triggers](#-parametric-triggers)
- [Weekly Premium Model](#-weekly-premium-model)
- [AI & ML Plan](#-ai--ml-plan)
- [Tech Stack](#-tech-stack)
- [Onboarding Flow](#-onboarding-flow)
- [Development Roadmap](#-development-roadmap)
- [Business Viability](#-business-viability)
- [Team](#-team)
- [Demo Video](#-demo-video)

---

## 🚨 The Problem

India's **5+ million food delivery riders** on Zomato and Swiggy are the backbone of our digital economy. But they are completely exposed to income loss caused by events entirely outside their control:

- A monsoon flood shuts down their zone → **zero earnings that day**
- A sudden Section 144 curfew is declared → **zero earnings that day**
- AQI crosses 400, government advises no outdoor activity → **zero earnings that day**

These riders have:
- ❌ No formal employer
- ❌ No ESI / PF coverage
- ❌ No income safety net of any kind
- ✅ A family depending on that week's pay

**A single disrupted week = missed rent, missed groceries, missed loan EMI.**

Currently, no insurance product in India addresses this gap specifically for gig delivery workers.

---

## 💡 Our Solution

**GigShield** is a mobile-first, AI-enabled parametric insurance platform that:

1. **Monitors** real-time weather, AQI, and civic alerts automatically
2. **Detects** threshold breaches using a real-time trigger engine
3. **Validates** the income loss with a multi-layer fraud detection system
4. **Transfers** a pre-agreed weekly wage-replacement directly to the rider's UPI account

**All within minutes. Zero paperwork. Zero calls. Zero forms.**

---

## 👤 Persona & Scenarios

### Who Is Our Customer?

| Attribute | Profile |
|---|---|
| Age | 20–35 years |
| Vehicle | Two-wheeler owner |
| Device | Android smartphone, 4G |
| Monthly Income | ₹12,000 – ₹22,000 |
| Pay Cycle | Weekly (Zomato / Swiggy) |
| Working Hours | 8–10 hrs/day, 6 days/week |
| Safety Net | None |

---

### Scenario A — Monsoon Flood (Mumbai, July)
> Rajesh, a Swiggy rider in Kurla, wakes up to flooded roads. GigShield detects rainfall > 80mm in 6 hours and waterlogging alerts in his registered zone. By 9 AM, **₹350 lands in his UPI account.** He stays home safely. No forms. No calls.

### Scenario B — Civic Curfew (Bengaluru, Election Day)
> Priya delivers for Zomato in Koramangala. A sudden Section 144 curfew is declared. GigShield's civic-alert feed picks it up. Platform signals show order volumes near zero. **Parametric trigger fires. Payout processed automatically.**

### Scenario C — AQI Spike (Delhi, November)
> AQI in Rohini crosses 400. Government advises no outdoor activity. GigShield's AQI monitor detects the breach. **Riders in affected pincodes receive automatic claim approval** with proportional payout for hours lost.

---

## 🔮 Unique Feature — Earnings Forecast Shield

**The feature no other team will build.**

Instead of only reacting to disruptions after they happen, GigShield **predicts high-risk days up to 7 days in advance** and proactively offers riders a coverage upgrade — before the disruption arrives.

### How It Works

```
Every Monday 6 AM
        ↓
Prophet model reads 7-day weather forecast
        ↓
XGBoost scores disruption probability per pincode
        ↓
Risk score > 70% threshold detected
        ↓
Push notification sent to rider:
"⚠️ High risk days ahead (Thu & Fri)
Upgrade to Shield Plus for just ₹20 extra?"
        ↓
        ├── Rider taps CONFIRM
        │       ↓
        │   UPI AutoPay deducts ₹20 extra
        │   Coverage upgraded to Shield Plus
        │   Payout cap raised to ₹1,400 ✅
        │
        └── Rider taps DECLINE
                ↓
            Original plan stays active
            No extra charge ✅
```

### Why Consent Is Non-Negotiable
GigShield **never auto-upgrades without explicit rider confirmation.** This is both an ethical and regulatory requirement under RBI and IRDAI guidelines. The rider always sees:
- Exact extra premium amount
- New payout cap unlocked
- 12-hour window to decide
- One-tap decline as easy as one-tap confirm

### What Makes This a Unicorn Feature
- Every other team's ML is **reactive** — ours is **predictive and proactive**
- Builds a **Shield Score** (financial health index) from forecast accuracy + claim history
- Riders with high Shield Scores earn **lower premiums and higher payout caps**
- Future roadmap: Shield Score becomes a **credit identity** for gig workers

---

## ⚡ Parametric Triggers

> **Excluded (Hard Constraints):** Health, Life, Accidents, Vehicle Repair.
> GigShield ONLY replaces lost weekly income caused by verifiable external disruptions.

| Disruption Type | Trigger Parameter | Threshold | Max Daily Payout |
|---|---|---|---|
| Heavy Rain / Flood | IMD rainfall + waterlogging index | ≥ 80mm in 6 hrs OR waterlog alert | ₹350/day |
| Extreme Heat | Heat index (temp + humidity) | ≥ 45°C feels-like for 4+ hrs | ₹200/day |
| Severe Air Pollution | AQI (PM2.5) | AQI ≥ 400 (Severe) for 3+ hrs | ₹250/day |
| Civic Disruption | Govt. advisory + platform order-drop | Section 144 OR order vol < 20% baseline | ₹350/day |
| Cyclone / Natural Disaster | IMD cyclone warning level | Yellow Alert or above in district | ₹350/day |

---

## 💰 Weekly Premium Model

### Why Weekly?
Zomato and Swiggy pay riders on a **weekly cycle**. Monthly premiums create cash-flow friction. A weekly model mirrors the rider's earnings rhythm perfectly.

### Premium Tiers

| Plan | Weekly Premium | Max Weekly Payout | Best For |
|---|---|---|---|
| Shield Basic | ₹29/week | ₹700 | Part-time / new riders |
| Shield Plus | ₹49/week | ₹1,400 | Full-time riders (recommended) |
| Shield Max | ₹79/week | ₹2,500 | High-earning / multi-app riders |

### AI-Driven Dynamic Pricing
Base premium is adjusted weekly by our ML risk engine using:
- Historical disruption frequency in rider's registered zone (pincode-level)
- Seasonal monsoon / AQI forecasting (7-day predictive window)
- Rider's own claim history (no-claim discount up to 15%)
- Platform-provided risk score (delivery zone volatility index)

**Example:** A rider in a low-waterlogging zone in Pune pays ₹39/week for Shield Plus. A rider in Dharavi during monsoon season pays ₹59/week for the same cover — reflecting real, hyper-local risk.

---

## 🤖 AI & ML Plan

### Model 1 — Dynamic Premium Calculation
- **Algorithm:** XGBoost (gradient-boosted regression)
- **Training Data:** Historical weather data (Open-Meteo API) + synthetic rider claims data
- **Inputs:** Zone rainfall history, AQI trend, civic event calendar, rider claim history, seasonal index
- **Output:** Adjusted weekly premium per rider at policy renewal
- **Retraining:** Weekly on new trigger events

### Model 2 — Earnings Forecast Shield (Unique Feature)
- **Algorithm:** Facebook Prophet (time-series forecasting)
- **Inputs:** 7-day weather forecast, historical disruption frequency, platform order trend
- **Output:** Daily risk score per pincode (0–100%)
- **Trigger:** Risk > 70% → proactive upgrade offer sent to rider

### Model 3 — Real-Time Parametric Trigger Engine
- **Type:** Rules-based engine + Isolation Forest anomaly detector
- **Polling:** Every 15 minutes — weather, AQI, platform-order APIs
- **Validation:** Cross-validates with second data source before firing claim trigger
- **Purpose:** Prevents false positives

### Model 4 — Intelligent Fraud Detection (3 Layers)

| Layer | Method | Action |
|---|---|---|
| Layer 1 | GPS Validation | Rider's location must be inside declared disruption zone at trigger time |
| Layer 2 | Activity Cross-Check | If order-acceptance rate is normal during claimed disruption → queue for review |
| Layer 3 | Isolation Forest | Flags riders whose claim frequency is statistical outlier vs cohort |

---



## 🛠️ Tech Stack

| Layer | Technology | Reason |
|---|---|---|
| Frontend | React PWA + Tailwind CSS | Mobile-first, offline support, no app store friction |
| Backend API | Node.js (Express, plain JS) | Non-blocking, perfect for real-time WebSocket trigger alerts |
| ML Service | Python (FastAPI) | Async, faster than Flask, auto-generates live API docs |
| Database | PostgreSQL | Industry standard for financial/insurance transactional data |
| Cache + Triggers | Redis | Sub-millisecond parametric trigger state management |
| Message Queue | Redis Pub/Sub | Instant claim event broadcasting across services |
| Weather API | Open-Meteo + IMD public feeds | Free tier, reliable, historical + real-time data |
| AQI API | SAFAR AQI API | Government-grade AQI data for Indian cities |
| Civic Alerts | Govt. district-collector scraper + mock fallback | Real alert source with demo-safe fallback |
| Payments | Razorpay test-mode (UPI + wallet) | Built for India, UPI simulation out of the box |
| Infra | Docker Compose | Single command spins entire platform — clean demo |

---

## 📱 Onboarding Flow

Designed for **sub-3-minute sign-up** on mobile, in Hindi and English:

```
1. Phone OTP Verification
   └── No email required, no password

2. Platform Link
   └── Enter Zomato/Swiggy Rider ID
   └── Auto-fetch registered delivery zones

3. Zone Confirmation
   └── Confirm 2–3 primary delivery pincodes
   └── Hyper-local risk calculation begins

4. Plan Selection
   └── 3 tile-based cards (Basic / Plus / Max)
   └── AI-personalised recommendation highlighted

5. UPI Setup
   └── Auto-detect UPI ID from phone
   └── One-tap save for instant payouts

6. Weekly Auto-Pay Consent
   └── UPI AutoPay mandate setup
   └── Deducted at start of each policy week
```

---

## 🗺️ Development Roadmap

| Week | Phase | Key Deliverables |
|---|---|---|
| 1–2 | Ideation & Foundation | Idea doc, tech stack, repo setup, Figma prototype, base PWA shell |
| 3 | Core Platform | Rider onboarding, OTP auth, zone selection, plan purchase, UPI AutoPay |
| 4 | Triggers & Claims | 5 parametric triggers, zero-touch claim engine, ML premium model v1, Forecast Shield v1 |
| 5 | Fraud & Payouts | GPS validation, Isolation Forest fraud model, Razorpay payout simulation |
| 6 | Polish & Submit | Admin dashboard, worker dashboard, load testing, 5-min demo video, pitch deck |

---

## 📊 Business Viability

### Market Sizing
- ~5 million active food delivery riders in India (Zomato + Swiggy, 2025)
- If 5% adopt Shield Plus @ ₹49/week → **~₹63 Cr annual gross premium**
- Target loss ratio: 55–65% (parametric products globally run 40–70%)

### Unit Economics (Shield Plus — illustrative)

| Item | Amount |
|---|---|
| Weekly premium collected | ₹49 |
| Expected weekly claim cost (loss ratio 60%) | ₹29.40 |
| Operating & tech cost per policy/week | ₹8 |
| **Net margin per policy per week** | **₹11.60 (24%)** |

---

## 👥 Team

| Member | Role |
|---|---|
| Member 1 | Node.js Backend — API & Parametric Triggers |
| Member 2 | React PWA Frontend & UX |
| Member 3 | Python FastAPI & ML Models |
| Member 4 | PostgreSQL, Redis & Docker Infrastructure |
| Member 5 | Integration, Testing & Demo |

---

## 🎬 Demo Video

📹 **[Watch the GigShield Phase 1 Prototype Walkthrough](https://youtube.com/shorts/zfXRVZexjsU?si=8nvd2x0sCY__LVMH)**
> *(https://youtube.com/shorts/zfXRVZexjsU?si=8nvd2x0sCY__LVMH)*

The 2-minute video covers:
- Rider onboarding flow
- Live monsoon flood trigger demo
- Earnings Forecast Shield — proactive upgrade consent flow
- Worker dashboard + Admin heatmap

---

*GigShield | Guidewire DEVTrails 2026 | Phase 1 Submission | March 20, 2026*
