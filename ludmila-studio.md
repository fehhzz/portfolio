# Ludmila Tavares — Lash Studio

[← Portfolio](README.md)

## Problem

Present a studio's services and visual identity in a responsive experience with a clear next action.

## Implementation

The frontend includes service sections, studio information, FAQ, image galleries, a dialog lightbox, mobile navigation and persistent contact actions. Business configuration is centralized in a dedicated module.

**Stack:** React 19, TypeScript, TanStack Start/Router, Vite 8, Tailwind CSS 4, Radix UI and Lucide.

## Technical decisions

- A centralized configuration file makes contact destinations easier to maintain.
- Shared components and state-driven interactions organize navigation and image exploration.
- Mobile contact actions support the same journey on smaller screens.

## Stage

The visual implementation is present. Booking and WhatsApp links still contain placeholders and must be configured, along with business content and asset review. Booking uses an external destination; no internal scheduling backend is implemented in this repository.

## Em português

Site editorial responsivo com serviços, galerias, FAQ e ações de contato. O projeto mostra trabalho de interface e experiência de navegação; a configuração de agendamento e WhatsApp ainda precisa ser concluída.
