# Bridge Investments Group — static website

Public site for **Bridge Investments Group** (legal entity: **Bridge Investments Group LLC**).

Production domain: [https://bridgebuyaz.com](https://bridgebuyaz.com)

This is a static HTML/CSS site. There is no application server and no form backend. The cash-offer form validates in the browser and shows a thank-you state. Connect a form handler (Formspree, Netlify Forms, a serverless function, etc.) later if you want submissions delivered by email.

## Pages

| File | URL |
| --- | --- |
| `index.html` | https://bridgebuyaz.com/ |
| `contact.html` | https://bridgebuyaz.com/contact.html |
| `privacy.html` | https://bridgebuyaz.com/privacy.html |
| `privacy-policy.html` | https://bridgebuyaz.com/privacy-policy.html (same policy; alternate path for 10DLC reviewers) |
| `terms.html` | https://bridgebuyaz.com/terms.html |
| `sms-terms.html` | https://bridgebuyaz.com/sms-terms.html |

Shared assets: `style.css`.

## 10DLC notes

- SMS opt-in is the website form: mobile number + an **unchecked-by-default** consent checkbox.
- Consent language sits next to the checkbox and links to `sms-terms.html` and `privacy.html`.
- Privacy Policy states phones are collected only from this form, numbers are never bought/rented/scraped, and SMS opt-in data is never sold.
- SMS Terms describe the program (follow-up on a request the person submitted), STOP/HELP, variable frequency, rates, and that consent is not required to receive an offer.
- Footer on every page includes Bridge Investments Group LLC, address, phone, email, Privacy | Terms | SMS Terms, and © 2026.

Use these live URLs on the 10DLC brand/campaign filing:

- Privacy: https://bridgebuyaz.com/privacy.html
- SMS Terms: https://bridgebuyaz.com/sms-terms.html
- Opt-in page: https://bridgebuyaz.com/

## Deploy (GitHub Pages)

1. Push this folder’s contents to a GitHub repository (or use the `gh-pages` branch). Include the `CNAME` file so Pages serves **bridgebuyaz.com**.
2. In the repo: **Settings → Pages → Source**: deploy from the branch that holds these files (usually `main` or `gh-pages`), root `/`.
3. Point DNS for **bridgebuyaz.com** (and www if used) at GitHub Pages with the A/AAAA or CNAME records GitHub shows for custom domains.
4. Enable HTTPS in the Pages settings once DNS propagates. Canonical links already use `https://bridgebuyaz.com`.
5. Confirm these URLs load:
   - https://bridgebuyaz.com/
   - https://bridgebuyaz.com/privacy.html
   - https://bridgebuyaz.com/privacy-policy.html
   - https://bridgebuyaz.com/terms.html
   - https://bridgebuyaz.com/sms-terms.html
   - https://bridgebuyaz.com/contact.html

Optional pretty URLs: configure so `/privacy`, `/terms`, `/sms-terms`, and `/contact` serve the matching `.html` files. Not required; the `.html` paths are linked in the site.

Do not rely on opening `index.html` from disk for a carrier screenshot — reviewers should see the live https://bridgebuyaz.com URLs.

## Local preview

```bash
python3 -m http.server 8080
```

Stop it when you are done.

## Contact (for host / DNS / 10DLC records)

- Public brand: Bridge Investments Group
- Legal: Bridge Investments Group LLC
- Contact: Alec Thomas
- Address: 1509 W Lobster Trap Drive, Gilbert, AZ 85233
- Phone: (815) 714-3499
- Email: arinrealfliphq@gmail.com
