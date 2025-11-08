---
layout: page
title: Team
permalink: /team/
header:
  theme: dark
---

<style>
/* Team page specific styles */
.team { display: grid; gap: 2.5rem; }
.team-member { display: flex; gap: 1.75rem; align-items: flex-start; }
.team-avatar { width: 130px; height: 130px; border-radius: 50%; object-fit: cover; background: #f5f5f5; flex-shrink: 0; border: 3px }
@media (max-width: 640px) { .team-member { flex-direction: column; align-items: center; text-align: center; } }
</style>

<div class="team">
  <div class="team-member">
    <img src="/assets/images/alistair_johnsoncairem-birem.jpg" alt="Photo of Alistair Johnson" class="team-avatar" />
    <div class="team-info">
      <h3>Alistair Johnson, Director</h3>
      <p>World-renowned scientist and creator of the MIMIC databases, used by tens of thousands of researchers around the world. Extensive expertise in medical data analysis, natural language processing, and machine learning.</p>
    </div>
  </div>
  <div class="team-member">
    <!-- Image from https://commons.wikimedia.org/wiki/File:201705_Scientist_bench_F.svg -->
    <img src="/assets/images/scientist.png" alt="Photo of Placeholder Name" class="team-avatar" />
    <div class="team-info">
    <h3>Tianshu Feng, Director</h3>
    <p>Biologist with end-to-end small‑molecule discovery experience from hit finding to lead optimization. Extensive experience with in vivo pharmacology and a proven track record delivering multiple validated oncology targets from bench to IND.</p>
    </div>
  </div>
</div>
