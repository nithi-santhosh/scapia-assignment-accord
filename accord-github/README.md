# Accord

A working prototype for sharing trip expenses and agreeing on repayment dates with friends.

## Files

- `index.html` — page shell, responsive styles, and animations.
- `app.js` — trips, expense splits, private requests, payment preferences, and Auto Pay interactions.
- `images/lake.jpg` and `images/mountains.jpg` — locally bundled travel photographs.
- `ASSETS.md` — image source information.

This export contains the latest published prototype. It has no build step, package installation, API key, or backend dependency.

## Run locally

From this folder, run:

```bash
python3 -m http.server 8000
```

Open http://localhost:8000 in your browser.



## Try the prototype

- Select **Explore as Nithi**. A fresh sample trip loads.
- After about 2.5 seconds, a reminder appears for the ₹600 repayment to Meera. The example uses the current date in India.
- **Pay now** asks for PIN **2001**, then offers payment-provider website shortcuts and a simulated payment action.
- **Enable Auto Pay** asks for confirmation and PIN **2001**. A due repayment starts a five-second countdown. Cancel payment or close the popup to stop it.
- **Profile & payments** has a separate Auto Pay toggle for every trip.
- PIN **2001** works for all sample users. It is a public prototype code, not a bank or UPI credential.
- Use **Switch user** to inspect both sides. Switching users does not trigger the login reminder.
- Signing out resets all sample data. Browser refreshes can retain the current session through local storage.

## Prototype boundaries

- No real Google authentication, bank connection, UPI mandate, payment processing, notification scheduling, or server-enforced private accounts.
- Payment-provider links open official websites; they do not start or prefill a transfer.
- Payments and Auto Pay debits are simulated. No real money moves.
- The browser stores sample data locally under `accord-app-v2`. Do not use this prototype for real personal financial records or enter bank credentials.
- Real production authentication and payment authorization must be implemented through appropriate backend and payment-provider integrations. The client-side PIN is for prototype interaction only.

## Images

Photographs are included in the ZIP, so they do not depend on live external image requests. See `ASSETS.md` for source links. They are travel inspiration, not photographs verified as Coorg.
