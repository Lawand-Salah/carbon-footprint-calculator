# Ecometric — Carbon Footprint Calculator

A React web app for estimating a household's annual carbon footprint based on energy usage, travel, and recycling habits. This is an early-stage build — the calculator itself works, but several planned pages are still stubs.

## Features

- **Home** — placeholder landing page (not yet designed)
- **Carbon Footprint Calculator** — the main working feature. Takes monthly electricity, gas and oil usage, yearly mileage and flights, and recycling habits (newspaper, aluminium/tin), and returns an estimated annual footprint in pounds/year
- **Booking Schedule** — route and nav link exist, page not yet built
- **Auth** — route and nav link exist, page not yet built

## Tech stack

- [React 19](https://react.dev/) (bootstrapped with [Create React App](https://github.com/facebook/create-react-app))
- [React Router v7](https://reactrouter.com/) for client-side routing
- Plain CSS per component

## Getting started

```bash
npm install
npm start
```

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

Build a production bundle:

```bash
npm run build
```

No deployment is currently configured (no `homepage` field or `gh-pages` script in `package.json`).

## Project structure

```
src/
├── Assets/           # Icons and images
├── Components/
│   ├── CarbonFootprint/   # The calculator logic and form
│   ├── DesktopNavbar/
│   └── Logo/
├── Pages/
│   ├── Home/         # Placeholder
│   ├── Footprint/    # Wraps the CarbonFootprint component
│   ├── Booking/       # Stub — not yet implemented
│   └── Auth/          # Stub — not yet implemented
├── Pages.js           # Route definitions
└── App.js              # App shell (navbar + routed pages)
```

## Known limitations

- **Home**, **Booking**, and **Auth** pages (and their stylesheets) are currently empty — routes and nav links exist, but there's nothing to render yet
- No mobile navigation component (desktop navbar only)
- The default Create React App test in `App.test.js` checks for a "learn react" link that no longer exists, so `npm test` will currently fail
- Calculator results are rough estimates based on fixed multipliers, not a certified carbon accounting method

## Author

Lawand Salah
