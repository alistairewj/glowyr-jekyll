---
layout: home
title: Glowyr Inc.
permalink: /
articles:
  excerpt_type: html
header:
  theme: dark
---

<section class="hero">
  <div class="hero__content">
    <h1>Scientific & Technical Expertise</h1>
    <p>For biotech, healthcare, and the life sciences.</p>
    <div class="cta">
      Get in touch: contact [at] glowyr [dot] ca
    </div>
  </div>
  <div class="hero__image">
    <img src="/assets/images/gnome.png" alt="Glowyr Inc." loading="lazy" />
  </div>
</section>

We offer expert services across the data lifecycle, including healthcare data stewardship, medical data analysis, and drug discovery.

<style>
/* Page-scoped minimalist enhancements */
.hero {display:grid;gap:3rem;align-items:center;padding:4.5rem 0;grid-template-columns:repeat(auto-fit,minmax(320px,1fr));}
.hero__content h1 {margin:0 0 1.25rem;font-size:clamp(2rem,5vw,3rem);line-height:1.05;font-weight:600;letter-spacing:.5px;}
.hero__content .lead {font-size:1.125rem;line-height:1.5;margin:0 0 1.5rem;color:var(--text-muted,#555);max-width:44ch;}
.pillars {list-style:none;padding:0;margin:0 0 2rem;display:grid;gap:.5rem;}
.pillars li {position:relative;padding:.6rem .9rem .6rem 2.1rem;border:1px solid #e2e5e9;border-radius:.6rem;background:#fff;box-shadow:0 1px 2px rgba(0,0,0,.04);font-size:.95rem;}
.pillars li:before {content:"";position:absolute;left:.9rem;top:50%;width:.55rem;height:.55rem;background:#2563eb;border-radius:50%;transform:translateY(-50%);}
.cta {display:flex;gap:1rem;flex-wrap:wrap;}
.hero__image {text-align:center;}
.hero__image img {width:100%;max-width:520px;border-radius:1rem;background:#0f1115;box-shadow:0 6px 20px -8px rgba(0,0,0,.35),0 2px 6px -1px rgba(0,0,0,.15);}
.sublede {margin:2rem auto 4rem;max-width:880px;font-size:1.05rem;line-height:1.55;color:#374151;padding:0 1rem;}
@media (prefers-color-scheme: dark){
  .pillars li {background:#1e2530;border-color:#2e3742;color:#d1d7de;}
  .pillars li:before {background:#3b82f6;}
  .hero__content .lead {color:#b0b9c3;}
  .sublede {color:#c7d0d9;}
}
@media (max-width:640px){
  .hero {padding:3rem 0 2.5rem;}
  .cta a {flex:1;text-align:center;}
}
</style>
