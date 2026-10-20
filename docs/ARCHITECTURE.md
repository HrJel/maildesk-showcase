# Architecture — Maildesk

## Architecture status

**Web source implementation documented; Android production API compatibility gap noted in source; iOS remains scaffold/API client.**

## Public high-level flow

```text
Portfolio frame → Sanitized Maildesk preview (separate demo) → demo services only; production mail platform stays isolated
```

## Verified high-level design

The web implementation uses Next.js and Cloudflare Workers, with server-side integrations for identity, storage, and mail delivery. The Android client is Flutter and the iOS code is an API-client scaffold. Any public demo must use fake mailboxes and non-production transport.

## Technology references

- Next.js 15, React 19, Tailwind / DaisyUI (web)
- Cloudflare Workers via OpenNext
- Supabase persistence; email transport integrations
- Flutter (Android client)
- Swift package and native iOS client scaffold

## Trust boundaries

1. The public showcase is a separate documentation/presentation boundary. It is not authorized to access production accounts or protected datasets.
2. Authentication, authorization, storage operations and confidential business rules, if applicable, belong to private reviewed services—not public mock UI.
3. An iframe is a nested browser context, not a substitute for server authentication or entitlement checks.
4. Device frames alter dimensions and appearance, not actual native runtime behavior.

## Unverified or intentionally omitted

- No production mailbox, message contents, email addresses, authentication secrets, or internal access are published.
- Do not assert Android release compatibility, iOS App Store acceptance, or production feature parity.
- The viewer must hide the Maildesk address and external-open control; iframe controls do not provide secrecy.

## Security/design review before going live

- [ ] Confirm any referenced architecture is approved for public disclosure.
- [ ] Use invented demo identifiers, content and accounts.
- [ ] Verify no private URL or client organization names appear in HTML, CSS, JS, screenshots or history.
- [ ] Test browser permissions and iframe CSP on the actual demo host.
- [ ] Confirm accessibility and responsive behavior separately on representative devices.
