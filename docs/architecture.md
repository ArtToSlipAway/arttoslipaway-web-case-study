# Architecture

## High-level structure

Public website → Nginx → FastAPI → PostgreSQL / CRM / client cabinet / Telegram / AI workflows / content workflow.

## Public layer

The public-facing platform presents tattoo projects, artwork, portfolio content, request flows and SEO-oriented category pages.

## Client workflow

Requests become structured client/project records with protected access, project context, communication history and private files.

## CRM

The internal CRM links customers, projects, communication and operational status.

## Telegram integration

Telegram conversations are linked to CRM entities and handled as part of the same workflow.

## AI integration

AI features are controlled workflow components with human handoff and conversation state.

## Security

The production implementation includes private file authorization, protected client links, request validation, CSRF/origin checks, secret isolation, server-side access control and security headers.

## Verification

The private production repository uses automated checks for application startup, empty PostgreSQL initialization, unit tests, synthetic seed data, HTTP integration tests and authorization behaviour.
