# AushadhiChakra: Pharmaceutical Supply Resilience & FEFO Rebalancing Engine

[![Live Demo](https://img.shields.io/badge/Live_Demo-Replit_App-blue?style=for-the-badge&logo=replit)](https://aushadhi-chakra-command-center--kethanreddy342.replit.app)
[![Track](https://img.shields.io/badge/Track-Healthcare_%2F_SDG_3-green?style=for-the-badge)](https://aushadhi-chakra-command-center--kethanreddy342.replit.app)
[![Problem Statement](https://img.shields.io/badge/Problem_Statement-PS02-orange?style=for-the-badge)](https://aushadhi-chakra-command-center--kethanreddy342.replit.app)

> **Team Name:** CascadeNull  
> **Problem Statement:** PS02 — From One Empty Shelf to a Regional Shortage  
> **Target Domain:** Healthcare / Disability (UN SDG 3: Good Health and Well-Being)  
> **Live Deployed Prototype:** https://aushadhi-chakra-command-center--kethanreddy342.replit.app

---

## 1. Executive Overview
When rural Primary Health Centres (PHCs) run out of frontline essential medicines, displaced patients migrate to neighboring clinics, triggering burn-rate surges that collapse regional supply within 48 hours. Meanwhile, nearby district hospital warehouses hold surplus batches nearing expiration that end up incinerated.

AushadhiChakra is an intelligent, zero-hardware spatial-temporal healthcare supply platform that:
1. **Predicts stockout contagion** using spatial gravity displacement and cross-drug therapeutic substitution.
2. **Automates First-Expired, First-Out (FEFO) peer-to-peer rebalancing** between public health clinics before localized shortages turn regional.
3. **Generates legally binding, audit-proof CDSCO Form 17/18 transfer vouchers** with HMAC-SHA256 signatures.
4. **Routes rebalanced stock with zero extra CapEx** along returning 108 emergency ambulance corridors.

---

## 2. Core Architecture & Features
- **Geospatial Resilience Grid:** Real-time visualization of health facility inventory nodes and depletion states across Udupi District, Karnataka.
- **Dual-Objective FEFO Optimizer (MILP):** Minimizes transit distance while penalizing donor retention of batches expiring in < 90 days.
- **Offline-First SMS Telemetry:** Ingests structured 2-way SMS webhooks (`STK <facility_id> <drug_code> <units>`) for remote clinics lacking broadband.
- **AushadhiWatch Public Transparency Portal:** Real-time taluk-level essential drug availability view for citizens.

---

## 3. Tech Stack
- **Frontend:** React 19, Vite, TailwindCSS, Leaflet / React-Leaflet
- **Backend:** Node.js, Express, TypeScript
- **State & Routing:** TanStack Query, Wouter
- **Live Hosting:** Replit Core Container Environment

---

## 4. Live Verification & Quick Links
- **Interactive Command Center:** [https://aushadhi-chakra-command-center--kethanreddy342.replit.app](https://aushadhi-chakra-command-center--kethanreddy342.replit.app)
- **Primary Modules:**
  - `/` — Command Center & Geospatial Depletion Heatmap
  - `/rebalance` — Automated FEFO Dispatch & Transfer Optimizer
  - `/telemetry` — 2-Way SMS Ingestion & Facility Ledger
  - `/public` — Citizen Drug Availability Lookup
