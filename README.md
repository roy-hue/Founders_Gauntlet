# 🧠 Idea Viability Builder

> **AI-powered business intelligence platform that transforms raw concepts into investor-ready business plans — with incentive stacking, stakeholder modeling, and viability scoring.**

---

## 🎯 What Makes This Different From Every Competitor

| Feature | Idea Viability Builder | Typical Competitors |
|---|---|---|
| Multi-layer incentive stacking | ✅ 3–5 layers mapped across stakeholders | ❌ Single-layer summaries |
| Stakeholder profit modeling | ✅ % profit increase per stakeholder | ❌ Generic audience sections |
| AI-structured JSON schema output | ✅ Enforced response schema via LLM | ❌ Freeform unstructured text |
| Operational blueprint generation | ✅ Activities, partnerships, cost structure | ❌ Surface-level suggestions |
| Phase-based scaling intelligence | ✅ Phases 1–3 triggered by customer count | ❌ Not offered |
| Subscription enforcement logic | ✅ Server-side limits + plan gating | ❌ Rarely enforced |
| Investor-ready summary output | ✅ Pitch-quality paragraphs from AI | ❌ Template fill-ins |
| Viability scoring (0–100) | ✅ Market + execution + profit scoring | ❌ Vague ratings |

---

## 🚀 Core Application Features

---

### 1. 🤖 AI-Powered Business Idea Analysis

- Users submit a business title and concept description
- A **precision-engineered system prompt** instructs the LLM to return a fully structured business model as valid JSON
- The AI identifies incentive layers, stakeholder benefits, pricing, operations, and investor summaries in a single inference call
- Response is validated against a **strict JSON schema** before being saved to the database
- Analysis is grounded in real-world financial logic, not generic suggestions

---

### 2. 🔁 Incentive Stacking Engine

- Analyzes **3–5 compounding incentive layers** across all business stakeholders
- Each layer identifies:
  - The incentive type (financial, social, business, customer)
  - The value created
  - The specific beneficiary
- This is the core differentiator — most tools give one-dimensional analysis; this maps the **full incentive ecosystem**

---

### 3. 👥 Stakeholder Benefit Modeling

- Identifies every stakeholder: vendors, customers, distributors, partners
- Calculates **specific profit increase percentages** per stakeholder
- Lists individual incentives per party
- Provides a complete economic picture of who wins, how much, and why

---

### 4. 💰 Pricing Intelligence Module

- AI generates:
  - Cost to produce
  - Wholesale price
  - Retail price range (low and high)
  - Competitor comparison with differentiation rationale
- Classifies market position: **Premium / Mass Market / Hybrid**
- Visualized as a pricing gradient with market positioning context

---

### 5. 🏗️ Operational Structure Generator

- Produces a complete operational blueprint including:
  - Key Activities
  - Key Partnerships
  - Revenue Streams
  - Cost Structure
- Modeled after **Business Model Canvas** principles, AI-generated per idea

---

### 6. 📊 Viability Scoring System

- Objective **0–100 score** per idea based on:
  - Market opportunity
  - Execution difficulty
  - Profit potential
- Color-coded scoring tiers: Highly Viable / Viable / Moderate / Needs Work

---

### 7. 📝 Investor-Ready Summary Output

- AI writes a **2–3 paragraph investor pitch** per idea
- Emphasizes stacked incentives and financial viability
- Suitable for direct use in pitch decks or funding conversations

---

### 8. 💳 Subscription & Monetization System

- **Free Tier:** Up to 3 idea analyses
- **Premium ($19.99/month):** Unlimited ideas, full feature access
- **Add-Ons available individually:**
  - 🔍 AI Analysis Boost — $9.99/mo
  - 📄 Export & Templates — $7.99/mo
  - 👥 Team Collaboration — $14.99/mo
- Subscription limits are enforced **server-side** (not client-side)
- Plan gating redirects users to upgrade flow automatically

---

### 9. 📈 Phase-Based Scaling Intelligence

- Tracks total paying customer count globally
- Automatically transitions the app through operational phases:
  - **Phase 1:** 0–49 customers → Early stage operations
  - **Phase 2:** 50–499 customers → Growth operations
  - **Phase 3:** 500+ customers → Legal risk threshold, scaled operations
- Phase transitions are logged with timestamps

---

### 10. 🔐 Security & Access Architecture

- Row-Level Security (RLS) on all business idea records
- Users can only access their own ideas
- Stripe secret keys are **100% server-side only** — never exposed to frontend
- Stripe webhook signature verification on every payment event
- JWT-based authentication via Base44 platform

---

## 🛠️ Technical Stack

---

### Frontend
- **React 18** — Component-based UI
- **Tailwind CSS** — Utility-first responsive styling
- **Framer Motion** — Fluid UI animations
- **React Query (TanStack)** — Server state management and caching
- **React Router DOM** — Client-side routing
- **Recharts** — Data visualization
- **Lucide React** — Icon system
- **Shadcn/UI** — Accessible component library

---

### Backend
- **Deno Deploy** — Serverless edge functions
- **Base44 SDK** — Auth, entities, integrations
- **Stripe API (v17)** — Subscription billing, checkout sessions, webhooks

---

### AI & Intelligence Layer
- **Base44 Core.InvokeLLM** — LLM inference with structured JSON schema enforcement
- Custom **multi-section system prompts** for business analysis
- **JSON Schema response validation** to guarantee structured outputs
- Incentive stacking, stakeholder modeling, pricing logic all derived from a **single optimized prompt**

---

### Database
| Entity | Purpose |
|---|---|
| `BusinessIdea` | Stores analyzed ideas with RLS |
| `Subscription` | User plans, Stripe IDs, add-ons |
| `AppPhase` | Global phase tracking by customer count |
| `User` | Auth, roles, profile data |

---

## 🧠 Prompt Engineering & System Thinking Skills Demonstrated

---

### Prompt Engineering
- **Structured output prompting** — Enforcing valid JSON responses via schema constraints
- **Role-based system prompting** — LLM instructed as a "business viability expert specializing in incentive stacking"
- **Multi-objective prompts** — Single prompt produces 6 distinct analytical outputs simultaneously
- **Domain-specific prompt design** — Language calibrated for investment, finance, and operational business concepts
- **Constraint-based generation** — Prompts define exact enum values, data types, and nested object structures
- **Contextual grounding** — User's title and concept are injected dynamically into the prompt context

---

### System Thinking & Architecture
- **Phase-based system design** — Application behavior evolves based on real-world customer thresholds
- **Incentive ecosystem modeling** — Multi-stakeholder value mapping at system level
- **Subscription enforcement architecture** — Limits enforced at function layer, not UI layer
- **Event-driven architecture** — Stripe webhooks trigger database state changes automatically
- **Security-first design** — RLS, server-side secrets, signature verification
- **Separation of concerns** — Frontend, backend, and AI layers independently scoped

---

### Business Intelligence with AI
- **AI-generated financial modeling** — Cost, wholesale, retail pricing derived from concept only
- **Automated stakeholder ROI analysis** — Profit percentage increases calculated per party
- **Market positioning classification** — AI determines premium vs. mass-market fit
- **Competitive differentiation analysis** — AI contextualizes the idea against market alternatives
- **Operational blueprint generation** — Business Model Canvas sections auto-populated
- **Investor pitch synthesis** — Structured narrative generation from raw business data

---

## 📌 ATS Keywords for Recruiters

Prompt Engineering · LLM Integration · Structured Output Design · JSON Schema Validation · System Prompt Architecture · AI Business Intelligence · Stakeholder Analysis · Financial Modeling · Operational Strategy · Business Model Canvas · SaaS Product Development · Subscription Billing · Stripe API · Webhook Architecture · React · Node.js · Deno · REST APIs · Serverless Functions · Data-Driven Decision Making · Market Positioning · Revenue Modeling · Investor Pitch Generation · Row-Level Security · Event-Driven Systems · API Design · Full-Stack Development · AI/ML Integration · Product Thinking · UX Design · Agile Development


---

## 👤 Built By

> A full-stack AI application architect with deep expertise in **prompt engineering**, **business intelligence systems**, **LLM-powered product design**, and **subscription SaaS architecture**.
> 
> This project demonstrates end-to-end ownership — from AI system design and prompt optimization to payment infrastructure, security architecture, and production-ready UI.

---

https://idea-catalyst-024894e5.base44.app

## 📄 License

MIT License — see `LICENSE` for details.
