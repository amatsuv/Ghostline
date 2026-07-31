# 👻 Ghostline

> Burner phone numbers for the privacy-obsessed. Swap n' Burn™ your number before it burns you.

## What is this?

Ghostline is a privacy-first VoIP service that gives you disposable phone numbers for SMS verification, anonymous communication, and breach protection. Swap numbers on demand. Burn compromised identities. Leave no trace.

## Features

- **Swap n' Burn™** — Destroy your current number and provision a fresh one instantly. No history, no residue.
- **Breach Monitor** — Real-time alerts when your number appears in data breaches.
- **Service Tracker** — Zero-knowledge encrypted log of which services have your number.
- **Crypto Payments** — Pay with BTC, XMR, LTC, ETH, USDT. No card required.
- **Zero Logging** — We can't hand over what doesn't exist. SMS retention is tier-based and aggressive.

## Tech Stack

- **Backend:** FastAPI · PostgreSQL · Redis · APScheduler
- **Frontend:** Next.js · Tailwind CSS
- **Telecom:** Telnyx API (SMS, MMS, Voice, Number Provisioning)
- **Payments:** Stripe · BTCPay Server (crypto)
- **Infra:** Docker · Nginx · Cloudflare

## Tiers

| Tier | Price | Numbers | SMS | Swap n' Burn | Retention |
|------|-------|---------|-----|--------------|-----------|
| Free | $0 | 1 | Inbound only | 1/day | 24 hours |
| Basic | $5/mo | 3 | Full | 5/mo | 30 days |
| Pro | $12/mo | 10 | Full | Unlimited | 30 days |
| Phantom | $25/mo | Unlimited | Full | Unlimited | 30 days |

## Quick Start

```bash
# Backend
cd mvp/backend
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env  # Fill in your keys
alembic upgrade head
uvicorn app.main:app --reload

# Frontend
cd mvp/frontend
npm install
npm run dev
```

## Legal

Operated by **Moja Holdings LLC** (Wyoming). We log nothing we don't legally have to.

This is a WIP, nothing works yet, pure placeholder
---

*"We log nothing. We can't hand over what doesn't exist."*
