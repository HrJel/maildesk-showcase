# Source verification and claims — Maildesk

## Public verification status

Web source implementation documented; Android production API compatibility gap noted in source; iOS remains scaffold/API client.

## Evidence-backed claims

- Operava-Mail web README documents authentication, mail folders, admin features, AI writing, and Cloudflare backend.
- Operava-Mail package.json confirms Next.js 15, React 19, OpenNext/Cloudflare, Supabase client.
- MailDesk-Android is Flutter; its own October 17, 2026 audit warns the Android client contract is incompatible with the live API.
- MailDesk-iOS describes scaffold plus API client, not a complete signed iOS release.
- operava-maildesk-api is an OpenAPI template repository; do not misidentify it as the complete production service.

## Unknowns requiring confirmation

- No production mailbox, message contents, email addresses, authentication secrets, or internal access are published.
- Do not assert Android release compatibility, iOS App Store acceptance, or production feature parity.
- The viewer must hide the Maildesk address and external-open control; iframe controls do not provide secrecy.

## Why original repository URLs are omitted

Private source locations, client-associated names and internal environments are intentionally excluded from the public GitHub repository. The author can maintain a separate non-public mapping for personal audit and traceability. Do **not** convert that mapping into public README links.

**Last documentation review:** 2026-10-20. No live system deployment, signing status or release readiness was independently retested by this public documentation process.
