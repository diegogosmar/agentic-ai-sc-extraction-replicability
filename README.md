# Agentic AI Supply Chain Document Extraction - Replicability Framework

[![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/gosmar/agentic-ai-sc-extraction-replicability)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Paper](https://img.shields.io/badge/Paper-Submitted-blue.svg)](#paper-reference)
[![Code Size](https://img.shields.io/github/languages/code-size/gosmar/agentic-ai-sc-extraction-replicability)](https://github.com/gosmar/agentic-ai-sc-extraction-replicability)

## 📋 Overview

This repository provides a **complete, replicable use case** for agentic AI-based document extraction in supply chain contexts, with comprehensive **energy consumption and environmental impact assessment**. The project demonstrates how Gemini 2.5 Flash with extended thinking capability processes complex commercial documents (proforma invoices) while maintaining rigorous sustainability metrics.

### 🎯 Key Contributions

- **Transparent Token Accounting:** Detailed breakdown of input/output/thinking tokens (11,906 total)
- **Energy Footprint Analysis:** Energy, CO₂, and water consumption quantified for single and scaled operations
- **100% Numerical Accuracy:** All 15 invoice line items extracted with correct currency handling
- **Academic Rigor:** Fully compatible with research methodology for Green AI assessment
- **Reproducible Framework:** Complete GitHub structure enabling community validation and benchmarking

---

## 📊 Core Use Case: Proforma Invoice Extraction

**Document:** 8-page anonymized proforma invoice with 15 commercial line items  
**Task:** Extract Quantity, Unit Price, and Total Price for each item  
**Model:** Google Gemini 2.5 Flash with extended thinking enabled  
**Output Format:** Structured JSON array (100% validated accuracy)

### Token Composition

| Component | Tokens | % of Total |
|-----------|--------|-----------|
| Proforma Invoice (input) | 9,030 | 75.8% |
| Extraction Prompt (input) | 1,259 | 10.6% |
| JSON Output (output) | 217 | 1.8% |
| Thinking/Reasoning (hidden) | 1,400 | 11.8% |
| **TOTAL** | **11,906** | **100%** |

### Environmental Impact (Single Document)

| Metric | Value |
|--------|-------|
| Energy Consumption | 0.3572 kWh (1,286 Wh) |
| CO₂ Emissions | 102.87 g (Italian grid: 288 gCO₂/kWh) |
| Water Usage | 0.0643–0.1072 L (WUE: 0.18–0.30 L/kWh) |
| Reasoning Overhead | 6.45:1 (thinking:output tokens) |

### Scaling Analysis

| Documents/Day | Energy (kWh) | CO₂ (kg) | Water (L) | Operational Scale |
|--------------|-------------|---------|----------|------------------|
| 1 | 0.357 | 0.103 | 0.064–0.107 | Single |
| 100 | 35.718 | 10.283 | 6.429–10.716 | High volume |
| 1,000 | 357.18 | 102.87 | 64.294–107.155 | Pilot |
| 5,000 | 1,785.9 | 514.34 | 321.462–535.770 | HITL Baseline |

---

## 📁 Repository Structure


