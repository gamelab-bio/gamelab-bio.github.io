---
layout: page
title: About
permalink: /about.html
---

<div class="lab-hero">
  <div class="hero-logo-scaler">
    <img class="hero-logo hero-logo-light" id="hero-logo-light" alt="GAME Lab" width="940" height="460">
    <img class="hero-logo hero-logo-dark" id="hero-logo-dark" alt="GAME Lab" width="940" height="460">
  </div>
</div>

<script>
(function () {
  // The logo is a static SVG, each in a light + dark variant. Pick ONE style
  // up front and keep it for the page view — toggling the theme only swaps
  // colors, never the logo version.
  var styles = {
    reads:   { light: '/assets/logos/static/wordmark-game-reads-static.svg',   dark: '/assets/logos/static/wordmark-game-reads-dark-static.svg' },
    plasmid: { light: '/assets/logos/static/wordmark-game-plasmid-static.svg', dark: '/assets/logos/static/wordmark-game-plasmid-dark-static.svg' }
  };
  var names = Object.keys(styles);
  var pick = styles[names[Math.floor(Math.random() * names.length)]];
  document.getElementById('hero-logo-light').src = pick.light;
  document.getElementById('hero-logo-dark').src = pick.dark;
})();
</script>

## Welcome to the GAME Lab

Cancer cells survive by adapting — switching strategies, competing for resources, cooperating when it pays. **GAME Lab** (Genomics & Adaptive Mechanisms) at [Institution] studies cancer as an evolving ecosystem of these strategies, combining experimental and computational approaches to learn how cells adapt, communicate, and survive — and how those same strategies expose new vulnerabilities.

By integrating CRISPR screening, genomic locus proteomics, single-cell technologies, and computational methods, we aim to identify vulnerabilities that emerge as cancer cells diversify their survival strategies.

---

## News

- **[Month Year]** — Placeholder news item.
- **[Month Year]** — Placeholder news item.

---

<div class="puzzle-link">
  <a href="/">← solve the entry puzzle again</a>
</div>
