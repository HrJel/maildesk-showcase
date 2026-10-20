# QA and acceptance checklist — Maildesk

## Application-specific validation

- [ ] Verify device switcher and no visible browser URL or external button.
- [ ] Verify the frame-ancestors policy in a browser against permitted and denied parent origins.
- [ ] Confirm direct-navigation handling in browser and note spoofable fetch metadata.
- [ ] Check no live email delivery, real user records, or production admin endpoints are exposed.
- [ ] Do not mark Android/iOS production-compatible until the documented API migration and device acceptance pass.

## Generic public-release validation

- [ ] README disclaimer includes independent Jelvan R. presentation, NDA/confidentiality limitations and no company endorsement.
- [ ] Status explicitly identifies what is source-documented, tested, unverified or proposed.
- [ ] No real environment values or operational endpoints in Markdown or JSON.
- [ ] GitHub secret scanning / code scanning enabled when available.
- [ ] Device selector does not infer native client availability from a mobile viewport.
- [ ] Public screenshots and media have consent and contain synthetic data.
- [ ] Accessibility checks for focus, color contrast and text resizing.
- [ ] Portfolio integration uses safe fallback if iframe refuses embedding.
- [ ] Browser response CSP and Fetch Metadata behavior tested if using Cloudflare frames.

## Acceptance result

**Not executed for real applications.** This checklist is an implementation plan, not a pass certificate.
