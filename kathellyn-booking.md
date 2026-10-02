# Kathellyn Cruz — Booking & Studio Website

[← Portfolio](README.md)

## Problem

A studio needs to collect appointment requests, control availability and retain manual approval over its schedule.

## Implementation

The demonstration project connects a responsive website to a booking flow and admin dashboard. Customers select a service, date and time; administrators review pending requests and manage appointment status, availability and blocks.

**Stack:** React 19, TypeScript, TanStack Start/Router, Vite 8, Tailwind CSS, Radix UI, PostgreSQL and PGlite for local development. The manifest specifies Node.js 24 and pnpm.

## Workflow

Service selection → available slot → customer details → pending request → manual approval → appointment lifecycle.

## Technical decisions

- Pending requests preserve administrator control rather than implying immediate confirmation.
- PGlite supports a local development workflow alongside the PostgreSQL production path.
- Server modules separate schedule rules, persistence, authentication and maintenance.
- The repository contains booking/hardening tests and a PostgreSQL integration script.

## Scope

The implementation includes rescheduling, history, optional email notifications and data-management features. WhatsApp communication remains manual. Payments, customer accounts and external calendar synchronization are outside the current scope.

Production configuration, credentials, backups and actual scheduling behavior must be checked before activation. No new test result or production readiness claim is made here.

## Em português

Projeto demonstrativo de site e agenda com aprovação manual, painel administrativo e regras de disponibilidade. Demonstra organização de regras de negócio, interface e persistência, com documentação de desenvolvimento e produção.
