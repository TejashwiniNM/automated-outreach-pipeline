# 🚀 4-Stage Automated Outreach Pipeline Engine

A highly resilient, modular backend automation execution pipeline built with **Node.js** and **ES Modules** syntax. This application sequentially streams asynchronously chained stages—uncovering B2B lookalike account matrices, enriching C-suite executive identity coordinates, resolving communication channels, and dispatching live transactional payloads—all through a unified command-line prompt interface.

---

## 🛠️ Architecture & Core Chained Stages

The automation engine operates seamlessly by handling background network data inputs cascading through four distinct integration lifecycle layers:

* 🌐 **Stage 1 (Market Intelligence Core):** Accepts an entry seed domain parameter and executes dynamic, live asynchronous company lookalike matching searches via Apollo's live structural `/v1/mixed_companies/search` data engine endpoint.
* 👥 **Stage 2 (Executive Enrichment Engine):** Automatically processes the mapped company lookalikes, pinging Prospeo's direct `/domain-search` endpoint path to filter and extract active corporate decision-maker records and matching LinkedIn channels.
* 🔍 **Stage 3 (Identity Profile Resolution):** Routes discovered profile vectors through an asynchronous network loop modeling the data schema standards of Eazyreach API systems.
* ✉️ **Stage 4 (Transactional Mail Transmission):** Compiles the verified target recipient vectors into a high-converting, professional cold outreach message layout, hooking straight into Brevo's live transactional `/v3/smtp/email` endpoints to trigger automated outbound dispatches.

---

## 🚨 Automation Critical Review Layer Safety Checkpoint

To guarantee absolute compliance with strict enterprise deliverability standards and prevent automated systems from executing blind spam operations, this pipeline implements an interactive checkpoint constraint layer:
* **The System Intercept:** The data chain automatically stops right after Stage 3 to render a clear target data summary matrix visualization directly on the terminal screen.
* **Manual Verification Prompt:** The execution sequence remains locked until the user explicitly inputs confirmation choices (`yes`/`no`), protecting your server and IP health.

---

## ⚙️ Local Configuration & Dependency Installation

### 1. Clone the Source Directory Tree
```bash
git clone https://github.com
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

# STAGE 3: Identity Resolution Access Key (Eazyreach Gateway Placeholder)
IDENTITY_RESOLUTION_ACCESS_TOKEN=EAZYREACH_INTERNAL_WORKSPACE_TOKEN

# STAGE 4: Transactional Mail Transmission Key (Brevo API Key)
OUTREACH_ENGINE_PROD_KEY=your_brevo_api_token_here

# SENDER PROFILE ROUTING PROPERTY
SENDER_EMAIL=your_verified_account_sender_email_here
```

---

## 🚀 Execution & Performance Verification Tuning

To clear terminal states and launch your interactive command-line interface automation stream sessions locally:
```bash
node index.js
```

---

## 🛡️ Resilience & Structural Fault Tolerance

Engineered using robust defensive programming patterns, all network boundary interactions are strictly isolated inside resilient `try/catch` logic blocks. If a user token faces token runtime exhaustion or a temporary API service timeout, the core runtime automatically triggers pre-compiled structural fallback simulation target nodes and prints explicit boundary logs to track sandbox boundary states. Furthermore, the transmission gateway logs realistic delivery warnings during execution drops rather than masking runtime network errors, guaranteeing absolute transparent visibility across the pipeline loop mid-stream.
