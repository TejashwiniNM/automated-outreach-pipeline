# 🚀 4-Stage Automated Outreach Pipeline Engine

A highly resilient, modular backend automation execution pipeline built with **Node.js** and **ES Modules** syntax. This application sequentially streams asynchronously chained stages—uncovering B2B lookalike account matrices, enriching C-suite executive identity coordinates, resolving communication channels, and dispatching live transactional payloads—all through a unified command-line prompt interface.

---

## 🛠️ Architecture & Core Chained Stages

The automation engine operates seamlessly by handling background network data inputs cascading through four distinct integration lifecycle layers:

* 🌐 **Stage 1 (Market Intelligence Core):** Accepts a seed domain and queries Apollo.io's `https://api.apollo.io/v1/mixed_companies/search` endpoint to discover lookalike B2B company domains with matching firmographics. Falls back gracefully to a curated target matrix if the API plan limit is reached.
* 👥 **Stage 2 (Executive Enrichment Engine):** Sends each discovered domain to Prospeo's `https://api.prospeo.io/domain-search` endpoint to extract C-suite and VP-level decision-makers along with their LinkedIn profile URLs and verified work emails.
* 🔍 **Stage 3 (Identity Profile Resolution):** Resolves contact identity coordinates using enriched Prospeo data — extracts and validates verified work email addresses for each discovered executive profile.
* ✉️ **Stage 4 (Transactional Mail Transmission):** Compiles verified contacts into a personalized cold outreach email and dispatches it via Brevo's `https://api.brevo.com/v3/smtp/email` transactional SMTP endpoint.

---

## 🚨 Automation Critical Review Layer Safety Checkpoint

To guarantee absolute compliance with strict enterprise deliverability standards and prevent automated systems from executing blind spam operations, this pipeline implements an interactive checkpoint constraint layer:
* **The System Intercept:** The data chain automatically stops right after Stage 3 to render a clear target data summary matrix visualization directly on the terminal screen.
* **Manual Verification Prompt:** The execution sequence remains locked until the user explicitly inputs confirmation choices (`yes`/`no`), protecting your server and IP health.

---

## ⚙️ Local Configuration & Dependency Installation

### 1. Clone the Source Directory Tree
```bash
git clone https://github.com/TejashwiniNM/automated-outreach-pipeline.git
cd automated-outreach-pipeline
```

### 2. Install Required Software Libraries
```bash
npm install
```

### 3. Environment Workspace Configuration (`.env`)
Create a secure, private configuration text file named exactly `.env` within the root project path to manage your server authentication token definitions:

```ini
# ==============================================================================
# AUTOMATION ENGINE PRIVACY CREDENTIAL MATRIX
# ==============================================================================

# STAGE 1: Market Intelligence Discovery Key (Apollo.io API Key)
MARKET_INTELLIGENCE_DISCOVERY_KEY=your_apollo_io_token_here

# STAGE 2: Core Executive Enrichment Key (Prospeo API Key)
ENRICHMENT_PIPELINE_SERVICE_KEY=your_prospeo_token_here

# STAGE 4: Transactional Mail Transmission Key (Brevo API Key)
OUTREACH_ENGINE_PROD_KEY=your_brevo_api_token_here

# SENDER PROFILE ROUTING PROPERTY
SENDER_EMAIL=your_verified_sender_email_here
```

---

## 🚀 Running the Pipeline

```bash
node index.js
```

---

## 🛡️ Resilience & Structural Fault Tolerance

Engineered using robust defensive programming patterns, all network boundary interactions are strictly isolated inside resilient `try/catch` logic blocks. If a token faces runtime exhaustion or a temporary API timeout, the core runtime automatically triggers pre-compiled structural fallback simulation nodes and prints explicit boundary logs to track sandbox states. The transmission gateway logs honest delivery errors during execution drops rather than masking failures, guaranteeing full transparent visibility across the pipeline.