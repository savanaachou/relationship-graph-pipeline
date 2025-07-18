# Founder Relationship Graph Pipeline

An automated pipeline that tracks billion-dollar tech exits and crypto events, enriches founder data with internal relationship intel, and generates visual warm-intro maps to support BD outreach—all in under 24 hours.

## ✨ What It Does

- **Tracks** recent tech M&A, IPOs, SPACs, and crypto token unlocks (≥ $1B FDV)
- **Enriches** founder records with warm-intro paths from email, calendar, CRM, and board overlaps
- **Visualizes** the internal + external relationship graph in Neo4j and Gephi
- **Exports** an interactive HTML map and static images for non-technical BD teams
- **Complies** with GDPR/CCPA by using only public or first-party data

## 🧱 Tech Stack

- **Data Sources:** Crunchbase, CoinMarketCap, Messari, Token Terminal, SEC RSS
- **ETL & Scripts:** Python, pandas, schedule
- **Staging DB:** PostgreSQL
- **Graph DB:** Neo4j (Community Edition)
- **CRM Enrichment:** Affinity, Introhive, LinkedIn Sales Navigator TeamLink
- **Visualization:** Gephi (via Gephi Toolkit CLI)
- **Orchestration:** GitHub Actions
- **Secrets Management:** HashiCorp Vault / AWS Secrets Manager

## 🚀 Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/your-org/founder-graph-pipeline.git
   cd founder-graph-pipeline

2. **Set up your enviroment variables**
  Copy the template and fill in credentials:
  ```bash
  cp .env.template .env
