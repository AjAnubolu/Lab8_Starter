# Lab 8 - Fetch API & ServiceWorkers

**Name:** Ajay Anubolu
**Partner(s):** none (solo)

**Deployed GitHub Pages URL:** https://ajanubolu.github.io/Lab8_Starter/

## How are graceful degradation and service workers related?

Graceful degradation means starting with the full, max-technology experience and
ensuring the app still works — just with less — when something it depends on goes
away. A web app's hardest dependency is the network: it is something we cannot
control and that fails constantly, especially on mobile. Service workers are the
mechanism that lets us degrade gracefully against exactly that failure. By sitting
between the app and the network, a service worker intercepts every request and
serves a cached copy when the network is slow or absent. So instead of a blank,
broken page when the connection drops (a hard failure), the user still gets the
HTML, CSS, JS, images, and recipe data straight from the browser cache — the app
keeps functioning, just without the ability to fetch brand-new data. The service
worker is what turns "no network = no app" into "no network = the app still works
with what it already has," which is graceful degradation in practice.

## PWA

`pwa.png` shows the recipe app installed as a Progressive Web App (manifest name
"Lab8_Starter").

## Part 3 - Expand

Not implemented (optional, no points).
