---
layout: page
title: About
permalink: /about.html
---

<div class="lab-hero">
  <div class="hero-logo-scaler" id="hero-scaler">
    <iframe class="hero-logo" id="hero-logo" title="GAME Lab" scrolling="no" loading="lazy"></iframe>
  </div>
</div>

<script>
(function () {
  // The animated logos are self-contained HTML pages, each in a light + dark
  // variant. Pick ONE style up front and keep it across both themes, so toggling
  // the theme only swaps colors — never the logo version.
  var styles = {
    reads:   { light: '/assets/logos/alive-reads-light.html',   dark: '/assets/logos/alive-reads-dark.html' },
    plasmid: { light: '/assets/logos/alive-plasmid-light.html', dark: '/assets/logos/alive-plasmid-dark.html' }
  };
  var names = Object.keys(styles);
  var pick = styles[names[Math.floor(Math.random() * names.length)]];

  var frame  = document.getElementById('hero-logo');
  var scaler = document.getElementById('hero-scaler');
  var BASE_W = 720, BASE_H = 420;   // natural size of the wordmark canvas

  function theme() {
    return document.documentElement.getAttribute('data-theme') === 'dark' ? 'dark' : 'light';
  }
  function applyLogo() {
    var src = pick[theme()];
    if (frame.getAttribute('src') !== src) frame.setAttribute('src', src);
  }
  function fit() {
    // Scale the fixed-size logo down to fit the column width (never up).
    var scale = Math.min(1, scaler.clientWidth / BASE_W);
    frame.style.transform = 'translateX(-50%) scale(' + scale + ')';
    scaler.style.height = (BASE_H * scale) + 'px';
  }

  applyLogo();
  fit();

  // Re-pick the matching-theme logo when the theme toggles, and rescale on resize.
  new MutationObserver(applyLogo).observe(document.documentElement, {
    attributes: true, attributeFilter: ['data-theme']
  });
  if (window.ResizeObserver) new ResizeObserver(fit).observe(scaler);
  else window.addEventListener('resize', fit);
})();
</script>

## Welcome to the GAME Lab

We are the **Genomics & Adaptive Mechanisms** laboratory at [Institution]. Our research sits at the intersection of cancer genomics, cell biology, and computational biology.

We use high-throughput sequencing, single-cell methods, and computational approaches to understand how cancer cells adapt, communicate, and survive under stress.

---

## News

- **[Month Year]** — Placeholder news item.
- **[Month Year]** — Placeholder news item.

---

<div class="puzzle-link">
  <a href="/">← solve the entry puzzle again</a>
</div>
