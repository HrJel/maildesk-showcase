# Implementation notes — Maildesk

## Evidence ledger

- Operava-Mail web README documents authentication, mail folders, admin features, AI writing, and Cloudflare backend.
- Operava-Mail package.json confirms Next.js 15, React 19, OpenNext/Cloudflare, Supabase client.
- MailDesk-Android is Flutter; its own October 17, 2026 audit warns the Android client contract is incompatible with the live API.
- MailDesk-iOS describes scaffold plus API client, not a complete signed iOS release.
- operava-maildesk-api is an OpenAPI template repository; do not misidentify it as the complete production service.

## Functional narrative

A private mailbox and communication workspace presented publicly as a sanitized UI/architecture case study; no real messages, contacts, login credentials or deployed mail systems are provided.

### Functional areas

- Mailbox navigation: inbox, sent, outbox and trash
- Authenticated multi-user account handling in web source
- Drafting/composing and server-side mail transport integrations
- Mobile client implementations at different maturity levels

## Implementation constraints

- No production mailbox, message contents, email addresses, authentication secrets, or internal access are published.
- Do not assert Android release compatibility, iOS App Store acceptance, or production feature parity.
- The viewer must hide the Maildesk address and external-open control; iframe controls do not provide secrecy.

## What this repository implements

- Markdown documentation, project-level metadata, safe viewer mode classification and release checklists.
- **No actual application runtime**, private source tree, database schema, email transport, credentials or deployment wiring.
- **No real live preview** is wired without an approved separate demo endpoint.

## Mapping from source to public presentation

The source references have been read for high-level technical accuracy, but private repositories and URLs are intentionally **not** disclosed in this publication. Documentation is paraphrased and stripped of confidential configuration. Technical assumptions requiring full source review remain marked as unverified.

## Upgrade path

1. Verify exact product and canonical source/version with the rights holder.
2. Inventory features that may safely be demonstrated.
3. Capture anonymized screenshots and create fake-data demo fixtures.
4. Independently test each indicated platform.
5. Update `portfolio.json` only after a reviewer approves the published claim.
