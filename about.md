---
layout: page
title: About
permalink: /about.html
---

<div class="lab-hero">
  <div class="hero-logo-scaler" id="hero-scaler"></div>
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

  var scaler = document.getElementById('hero-scaler');
  var BASE_W = 720, BASE_H = 420;   // natural size of the wordmark canvas
  var frames = {};                  // theme -> iframe, created once then reused

  function theme() {
    return document.documentElement.getAttribute('data-theme') === 'dark' ? 'dark' : 'light';
  }
  function scaleOf() { return Math.min(1, scaler.clientWidth / BASE_W); }
  function sizeFrame(f) { f.style.transform = 'translateX(-50%) scale(' + scaleOf() + ')'; }

  // Each logo iframe is heavy (loads React + transpiles its art), so build it
  // once per theme and cache it. Toggling then just flips visibility — no reload,
  // no re-transpile — which is what made switching themes feel slow.
  function show(t) {
    if (!frames[t]) {
      var f = document.createElement('iframe');
      f.className = 'hero-logo';
      f.title = 'GAME Lab';
      f.setAttribute('scrolling', 'no');
      f.loading = 'lazy';
      f.src = pick[t];
      sizeFrame(f);
      scaler.appendChild(f);
      frames[t] = f;
    }
    for (var k in frames) frames[k].style.visibility = (k === t ? 'visible' : 'hidden');
    scaler.style.height = (BASE_H * scaleOf()) + 'px';
  }
  function fit() {
    for (var k in frames) sizeFrame(frames[k]);
    scaler.style.height = (BASE_H * scaleOf()) + 'px';
  }

  show(theme());   // load only the current theme up front
  fit();

  // Swap visibility (loading the other theme once, lazily) and rescale on resize.
  new MutationObserver(function () { show(theme()); }).observe(document.documentElement, {
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
