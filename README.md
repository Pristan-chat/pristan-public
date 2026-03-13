<p align="center">
  <img src="https://www.pristan.chat/logo.png" alt="Pristan" width="200" />
</p>

<h1 align="center">Pristan — Enterprise AI Agent Catalog</h1>

<p align="center">
  <strong>One place to manage every AI tool your teams use.</strong><br />
  Deploy, govern, and monitor AI agents across your organization — without rebuilding your stack.
</p>

<p align="center">
  <a href="https://www.pristan.chat">Website</a> •
  <a href="https://www.pristan.chat/features">Features</a> •
  <a href="https://www.pristan.chat/security">Security</a> •
  <a href="https://www.pristan.chat/pricing">Pricing</a> •
  <a href="https://www.pristan.chat/enterprise">Enterprise</a>
</p>

---

## What is Pristan?

Shadow AI is out of control. Teams are signing up for AI tools on their own, pasting sensitive data into unknown chatbots, and nobody knows what's being used or what it costs. Pristan gives you a single, governed catalog where employees find approved AI agents — and IT keeps full visibility.

Think of it as **Okta for AI** — a ServiceNow-style catalog purpose-built for AI agents.

### The Problem

- Employees use 5+ AI tools with no oversight
- Sensitive data leaks into unvetted AI services
- AI costs are invisible until the bill arrives
- No audit trail for AI interactions
- Security teams can't enforce policies on tools they don't know exist

### The Solution

Pristan provides a curated, governed catalog of AI agents. Employees get the AI tools they need. IT gets the controls they require. Everyone wins.

---

## Key Features

### 🤖 Universal AI Agent Catalog

Deploy and manage AI chatbots from any provider through a single interface. Connect OpenAI, Anthropic, Google, Azure, or any OpenAI-compatible endpoint. Your teams get one place to discover and use approved AI agents.

- **Multi-provider support** — OpenAI, Anthropic Claude, Google Gemini, Azure OpenAI, Ollama, and any OpenAI-compatible API
- **BYOK (Bring Your Own Keys)** — Customers use their own API keys. Pristan never touches your AI traffic or stores API responses
- **Agent marketplace** — Curated catalog of purpose-built AI agents for different teams and use cases
- **Custom system prompts** — Configure agent behavior, personality, and domain expertise per chatbot

### 📚 RAG & Knowledge Base

Ground every AI answer in your own data. Upload documents, and agents cite their sources — reducing hallucinations and making answers verifiable.

- **Multi-format ingestion** — PDF, DOCX, TXT, CSV, and more
- **Flexible vector storage** — Built-in vector database with chunking and embedding
- **Source citations** — Every AI response can reference the exact document and passage it drew from
- **Personal & team knowledge bases** — Scoped document collections per user, team, or organization

### 🔐 Enterprise Security & Governance

Security isn't an add-on — it's the foundation.

- **Full audit trail** — Every conversation, every prompt, every response — logged and searchable
- **DLP (Data Loss Prevention)** — Detect and block sensitive data (PII, credentials, proprietary info) before it reaches any AI provider
- **Prompt injection protection** — Multi-layer defense against prompt injection and jailbreak attempts
- **Role-based access control** — Global roles, group-level permissions, per-agent access policies
- **MFA enforcement** — Platform-wide or per-group multi-factor authentication requirements
- **SSO / SAML** — Enterprise single sign-on integration
- **CSRF protection & trusted hosts** — Defense-in-depth web security

### 💰 Cost Management

Know your AI costs before finance does.

- **Real-time dashboards** — Token usage, cost attribution, and spend tracking across all providers
- **Budget controls** — Set spending limits per user, team, or agent
- **Cost attribution** — See exactly which teams and agents drive costs
- **No bill shock** — Alerts and caps before budgets are exceeded

### 👥 Identity & Access Management

Enterprise-grade user and group management.

- **User management** — Create, edit, and manage users with global roles
- **Group-based access** — Assign AI agent access by group membership
- **Per-agent permissions** — Control exactly which users and groups can access each agent
- **Group policies** — Budget limits, MFA requirements, and usage policies per group

### 📊 Observability & Monitoring

Full visibility into how AI is being used across your organization.

- **Conversation history** — Searchable archive of all AI interactions
- **Team workspaces** — Isolated conversation spaces per team
- **Quality tracking** — Monitor response quality and user satisfaction
- **Platform health** — System metrics, provider status, and performance monitoring
- **Jaeger tracing** — Distributed tracing for debugging and performance analysis

### 🔗 Integrations

Connect Pristan to the tools your teams already use.

- **Slack integration** — Access AI agents directly from Slack channels
- **Microsoft Teams** — AI agents in your Teams workspace
- **N8N workflows** — Automate AI agent provisioning and management
- **Webhook support** — Event-driven integrations with your existing systems
- **Alert system** — Configurable alerts for security events, budget thresholds, and system health

### 📱 Multi-Platform

- **Web application** — Full-featured desktop experience
- **Mobile app** — Native mobile interface for on-the-go access
- **API** — RESTful API for programmatic access and automation

---

## Architecture

Pristan is a self-hosted platform designed for enterprise deployment:

- **Frontend** — Next.js (React) with TypeScript
- **Mobile** — React Native / Expo
- **Backend** — Python (FastAPI)
- **Database** — PostgreSQL (multi-database: platform, users, chatbots)
- **Cache** — Redis
- **Object Storage** — MinIO (S3-compatible)
- **Observability** — Jaeger (distributed tracing)
- **Deployment** — Docker Compose, CI/CD via GitHub Actions

### BYOK Model

Pristan operates on a **Bring Your Own Keys** model. Your organization provides its own AI provider API keys. This means:

- **Zero AI API costs for Pristan** — you pay your AI providers directly
- **No data passes through Pristan servers** — API calls go directly from your deployment to your AI provider
- **Full control** — switch providers, models, or keys at any time without vendor lock-in

---

## Deployment

Pristan is deployed as a self-hosted Docker stack on your infrastructure. Each customer gets a dedicated, isolated deployment.

### Requirements

- Linux server (Ubuntu 22.04+ recommended)
- Docker & Docker Compose
- 4+ CPU cores, 8+ GB RAM (recommended)
- PostgreSQL 15+
- Domain with SSL certificate

For deployment inquiries, contact us at [hello@pristan.chat](mailto:hello@pristan.chat).

---

## Pricing

**$14.99 / user / month** — single flat price, no tiers.

- All features included
- Unlimited AI agents
- Unlimited conversations
- Full security & governance suite
- Volume pricing available for 1,000+ users

See [pristan.chat/pricing](https://www.pristan.chat/pricing) for details.

---

## Security

Security is core to Pristan's design. For a detailed overview, visit our [Security page](https://www.pristan.chat/security).

Key highlights:

- End-to-end audit trail for all AI interactions
- DLP scanning on every message
- Prompt injection defense (multi-layer)
- Role-based access control with group policies
- MFA support (TOTP) with per-group enforcement
- SAML / SSO integration
- CSRF protection, trusted host validation
- No customer data stored on Pristan infrastructure (BYOK model)

---

## Status

Pristan is in **active development** and preparing for first customer pilots.

- ✅ Core platform built and functional
- ✅ Multi-provider AI agent support
- ✅ RAG / knowledge base with source citations
- ✅ Full identity & access management
- ✅ DLP, audit logging, prompt injection defense
- ✅ Cost tracking & budget controls
- ✅ Slack & Teams integration
- ✅ Mobile app
- 🔜 SOC 2 certification (roadmap)
- 🔜 Additional SSO providers

---

## Contributing

This is a **read-only informational repository**. The Pristan platform is developed in a private repository.

We do not accept pull requests, issues, or contributions on this repo.

If you're interested in Pristan, reach out:

- **Website:** [pristan.chat](https://www.pristan.chat)
- **Email:** [hello@pristan.chat](mailto:hello@pristan.chat)
- **LinkedIn:** [Pristan AI](https://www.linkedin.com/company/pristan-ai/)
- **X (Twitter):** [@PristanChat](https://x.com/PristanChat)

---

## License

All rights reserved. © 2025–2026 Pristan.

This repository is provided for informational purposes only. The Pristan platform, its source code, and associated materials are proprietary software. No license is granted to use, copy, modify, or distribute the platform software.

See [LICENSE](LICENSE) for details.
