# Prime Cuts Barber Shop Website

A modern 5-page barber shop website built with HTML, CSS, and JavaScript.

## Live Pages

- `index.html` - Home
- `about.html` - About
- `booking.html` - Booking (Calendly integration)
- `services.html` - Services
- `gallery.html` - Gallery

## Highlights

- Fully responsive layout (mobile, tablet, desktop)
- Clean premium UI design
- Sticky navigation with mobile menu
- Service cards and pricing section
- Gallery grid with high-quality barber images
- Online booking via Calendly

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript

## Local Development

Run a static server in the project folder:

```bash
python -m http.server 5500
```

Then open `http://localhost:5500`.

## Deployment

This is a static website and can be deployed directly on Vercel.

## Project Structure

```text
barbershop-premium-template/
├── index.html
├── about.html
├── booking.html
├── booking-config.js
├── services.html
├── gallery.html
├── styles.css
├── script.js
├── vercel.json
└── .gitignore
```

## Calendly booking URL

Your **GitHub username is not** your Calendly link. In Calendly, open an event type → **Share** → copy the link (for example `https://calendly.com/your-name/30minute`).

Paste that full URL into `booking-config.js` as `window.PRIME_CUTS_CALENDLY = "…";` then reload the booking page.

## Git: normal workflow

Always run git commands inside the project folder (not `D:\BarberShop Website` unless `.git` is there):

```powershell
cd "D:\BarberShop Website\barbershop-premium-template"
git add .
git commit -m "Describe your change"
git push origin main
```

If GitHub says **non-fast-forward** after you rebuilt history locally, your local `main` and GitHub `main` no longer share the same commits. To make **GitHub match your local** (overwrites remote history):

```powershell
git push -f origin main
```

Use **force push** only when you intend to replace what is on GitHub.

If `git push` fails with **could not connect to github.com:443**, fix network first (VPN, firewall, or try another connection), then:

```powershell
Test-NetConnection github.com -Port 443
```

## Notes

- Replace phone number, address, and opening hours with real business details.
- Replace image URLs with final brand images if needed.
