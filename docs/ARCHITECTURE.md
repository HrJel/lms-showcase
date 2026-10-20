# Architecture — LMS

## Architecture status

**Runnable Django course/assessment scaffold described in source, not a verified full production LMS.**

## Public high-level flow

```text
Browser → Django templates / views → Django models / database; optional edge reverse proxy in front
```

## Verified high-level design

Conventional Django application with course views, models, admin and template-rendered pages. A separate Cloudflare Worker may function as a reverse proxy when a Python origin is hosted elsewhere.

## Technology references

- Python and Django
- Django templates and Bootstrap-style views
- Django admin and relational models
- Optional Cloudflare Worker reverse-proxy example

## Trust boundaries

1. The public showcase is a separate documentation/presentation boundary. It is not authorized to access production accounts or protected datasets.
2. Authentication, authorization, storage operations and confidential business rules, if applicable, belong to private reviewed services—not public mock UI.
3. An iframe is a nested browser context, not a substitute for server authentication or entitlement checks.
4. Device frames alter dimensions and appearance, not actual native runtime behavior.

## Unverified or intentionally omitted

- Do not claim enterprise LMS maturity, payment support, mobile-native apps, or a production cloud deployment.
- Demo user details and grading content must be synthetic.

## Security/design review before going live

- [ ] Confirm any referenced architecture is approved for public disclosure.
- [ ] Use invented demo identifiers, content and accounts.
- [ ] Verify no private URL or client organization names appear in HTML, CSS, JS, screenshots or history.
- [ ] Test browser permissions and iframe CSP on the actual demo host.
- [ ] Confirm accessibility and responsive behavior separately on representative devices.
