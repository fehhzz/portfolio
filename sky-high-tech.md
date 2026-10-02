# Sky High Tech — Website & Lead Management

[← Portfolio](README.md)

## Problem

A service website needs a way to receive inquiries and organize them beyond a static contact page.

## Implementation

The Next.js application combines a public website, a lead submission API and an authenticated administration interface. Prisma stores records in PostgreSQL. The API validates input with Zod, includes a honeypot and applies process-local rate limiting; email integration can notify the configured recipient.

| Layer | Choice |
| --- | --- |
| Application | Next.js 16 App Router, React 19, TypeScript |
| Data | Prisma 6 and PostgreSQL |
| Authentication | Better Auth with Prisma adapter |
| Interaction | Tailwind CSS, Framer Motion, GSAP, Lenis |
| Checks present | Vitest and React Testing Library |

## Workflow

Visitor submits contact form → API validates input → lead is persisted → email notification is attempted → administrator manages records through protected routes.

## Technical decisions

- Validation sits at the API boundary instead of relying only on browser fields.
- Database access and authentication are organized in separate supporting modules.
- Public presentation and administration routes share the application while serving different workflows.

## Stage and next improvements

The code includes these application layers. Administrator provisioning, authorization, email delivery and deployment still need staging validation. A shared rate-limit store would be needed for multiple server instances. Existing test files are evidence of a validation structure; this portfolio does not assert a new passing run.

## Em português

Site institucional com captação de leads, banco PostgreSQL, autenticação e painel. Demonstra desenvolvimento full-stack, validação de dados e integração entre a experiência pública e a operação administrativa.
