# Lead Hunter Pro — Local Research & CRM

[← Portfolio](README.md)

## Problem

Organize business research and lead information in a local interface with enrichment and export workflows.

## Implementation

A Streamlit dashboard coordinates Python modules for research, business-profile analysis, local JSON persistence and CSV/XLSX export. Optional integrations include AI, Google Sheets, email and a separate Node.js messaging service.

**Stack:** Python, Streamlit, pandas, Playwright, JSON, Node.js and Express.

## Technical decisions

- Research, analysis, configuration and persistence are organized in distinct modules.
- Export supports working with data outside the dashboard.
- The optional messaging service runs separately from the Streamlit process.

## Scope and data

The dashboard is a local tool with optional external dependencies, not a fully offline application or hosted multi-tenant SaaS. The operational repository contains contact records and remains private. This case study contains no lead data, session files or credentials.

The existing scraper check is a manual external smoke script rather than an assertion-based unit test suite. A useful next step is a synthetic-data validation suite that exercises persistence and export without external research or message sending.

## Em português

Ferramenta local para pesquisa, organização, enriquecimento e exportação de leads. Demonstra integração de módulos Python e serviços opcionais. A apresentação pública descreve a arquitetura e preserva os contatos operacionais.
