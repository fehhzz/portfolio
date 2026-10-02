# Gabrielle Castilho — Studio Website

[← Portfolio](README.md)

## Problem

Bring service information and appointment requests into one consistent digital experience.

## Implementation

The Next.js website contains service, plan, FAQ and contact sections, a booking component and administration pages for agenda, services and settings. Supabase provides data and authentication integration.

**Stack:** Next.js 16, React 19, TypeScript, Tailwind CSS 4, Supabase and date-fns.

## Workflow

Visitor explores services → selects a date/time → submits appointment details → server checks the requested interval → pending appointment is stored.

## Technical decisions

- Server Actions keep appointment creation separate from the visual booking component.
- Availability calculation is centralized in a dedicated utility.
- Browser and server-side Supabase clients serve different integration needs.

## Stage

The implementation exists, but database provisioning, Row Level Security and administrator authorization need review. The current overlap check should be tested under concurrent requests; checking before insertion does not by itself guarantee atomic conflict prevention. Contact and business content also require final configuration.

## Em português

Site com apresentação de serviços, solicitação de agendamento e administração. Demonstra desenvolvimento de interface, integração com Supabase e separação entre a jornada visual e a criação de registros no servidor.
