PAYDAY — RELEASE CANDIDATE 1.0
================================

WHAT IS INCLUDED
- Installable Progressive Web App (PWA)
- Five UI languages: English, Bulgarian, Spanish, French and German
- Currency setting: EUR, USD or GBP
- Last/next payday cycle and suggested daily spending limit
- Income, expenses and unpaid/paid bills
- Savings goals with contributions
- Local storage (no account or bank connection)
- JSON backup and restore
- Draft storefront listing in STORE_LISTING.txt
- Responsive phone/tablet/desktop layout
- Basic offline shell caching

HOW TO TEST LOCALLY
1. Extract the ZIP.
2. Open index.html in a modern browser to test the main app features.
3. PWA installation and offline service-worker behavior require HTTPS hosting or localhost.

HOW TO PUBLISH FOR TESTING
Upload the contents of this folder (index.html, manifest.webmanifest, icon.svg, sw.js) to a static host such as Cloudflare Pages. Use the folder contents as the site root. Once it has an HTTPS URL, open it on a phone and use the browser menu -> Install app / Add to Home Screen.

IMPORTANT LIMITATIONS BEFORE SELLING
- This is a client-side app. Budget data is stored in the customer's browser/device and is not synced to a server.
- Clearing browser/site data may erase data; customers should use Export backup.
- There is no account/login, server-side license enforcement, payment integration, or automatic PayPal purchase verification included.
- Do not promise secure buyer-only access to a public URL until a licensing/access-control flow is implemented.
- The PayPal/Payhip storefront, legal business details, refund policy, privacy notice, and tax handling must be configured separately by the seller.
- Test on current iPhone Safari and Android Chrome before advertising it as installable on all devices.

QUICK QA CHECKLIST
[ ] Change language in each of the five languages
[ ] Add income, an expense and a bill; mark a bill paid/unpaid
[ ] Check daily safe-to-spend calculation against manual arithmetic
[ ] Create a savings goal and add a contribution
[ ] Edit and delete records
[ ] Export backup, reset data, then restore backup
[ ] Install from HTTPS and check offline launch
[ ] Test narrow mobile viewport and date inputs
