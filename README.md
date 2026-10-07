# Home Bills family viewer — synthetic POC

Generic static read-only browser viewer code only. No financial dataset, encrypted payload, unlock secret, decryption key or private signing key belongs in this repository.

Code is served by GitHub Pages. Only existing synthetic encrypted payloads and a nonsensitive signed bootstrap descriptor may be served separately by Cloudflare R2 for this POC. Unlocking and verification happen locally in the browser.

Viewer version: 0.1.0. Build: 5885fbf6b692e64a. Storage configured: false.

Publish the main branch root with GitHub Pages and HTTPS. No custom workflow, runtime third-party JavaScript, analytics, domain, deploy token or Actions secret is required.

The restrictive CSP is in index.html. GitHub Pages does not apply the local builder's _headers file, so that unsupported file is omitted. A compromised code-host account could still replace root HTML/JavaScript and steal a future unlock secret; SRI does not eliminate this trust boundary.

Synthetic testing only. This is not a production financial service, authentication system, recovery system or enrollment/revocation implementation.
