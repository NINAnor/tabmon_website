---
title: "Resources & Tools"
date: 2025-09-04
draft: false
description: "Access TABMON's dashboard, code repositories, technical documentation, and data resources for Europe's acoustic biodiversity monitoring network"
---

<div class="pub-section-intro">
<p>Access TABMON's open-source tools, live dashboards, and data platforms powering Europe's largest acoustic biodiversity monitoring network.</p>
</div>

## Live Platforms

<div class="resource-grid">

<div class="resource-card resource-card--dashboard">
  <div class="resource-card-icon">
    <svg width="36" height="36" viewBox="0 0 24 24" fill="none" stroke="#06B6D4" stroke-width="1.5"><rect x="3" y="3" width="7" height="7" rx="1"/><rect x="14" y="3" width="7" height="4" rx="1"/><rect x="14" y="10" width="7" height="11" rx="1"/><rect x="3" y="13" width="7" height="8" rx="1"/></svg>
  </div>
  <div class="resource-card-content">
    <h3>Monitoring Dashboard</h3>
    <p>Real-time insights into data acquisition, device performance, and biodiversity patterns across <strong>100+ active sites</strong> with <strong>&lt;24-hour latency</strong>.</p>
    <ul class="resource-features">
      <li>Device status & network coverage</li>
      <li>Data ingestion & quality metrics</li>
      <li>Species occurrence & activity trends</li>
      <li>Audio signal diagnostics</li>
    </ul>
    <a href="https://tabmon.nina.no" class="resource-link" target="_blank">Open Dashboard <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M7 17L17 7M17 7H7M17 7V17"/></svg></a>
  </div>
</div>

<div class="resource-card resource-card--lab">
  <div class="resource-card-icon">
    <svg width="36" height="36" viewBox="0 0 24 24" fill="none" stroke="#10B981" stroke-width="1.5"><path d="M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"/><path d="M19 10v2a7 7 0 0 1-14 0v-2"/><line x1="12" y1="19" x2="12" y2="23"/><line x1="8" y1="23" x2="16" y2="23"/></svg>
  </div>
  <div class="resource-card-content">
    <h3>Listening Lab</h3>
    <p>Help us improve AI accuracy! Our citizen science platform lets <strong>acoustic ecologists and volunteers</strong> annotate sound samples to train better species recognition models.</p>
    <ul class="resource-features">
      <li>Train species recognition algorithms</li>
      <li>Improve detection confidence</li>
      <li>Contribute to open bioacoustics</li>
    </ul>
    <a href="https://tabmon-listening-lab.nina.no" class="resource-link" target="_blank">Start Annotating <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M7 17L17 7M17 7H7M17 7V17"/></svg></a>
  </div>
</div>

</div>

---

## Code & Repositories

TABMON is committed to **reproducible, open science**. All code and documentation are publicly available under open-source licenses.

<div class="repo-grid">

<div class="repo-card">
  <div class="repo-header">
    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#06B6D4" stroke-width="1.5"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
    <span class="repo-name">TABMON</span>
    <span class="repo-badge">Hub</span>
  </div>
  <p class="repo-desc">Central documentation hub linking all project repositories, protocols, and metadata standards.</p>
  <a href="https://github.com/NINAnor/TABMON" class="pub-link" target="_blank">View on GitHub <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M7 17L17 7M17 7H7M17 7V17"/></svg></a>
</div>

<div class="repo-card">
  <div class="repo-header">
    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#F59E0B" stroke-width="1.5"><circle cx="12" cy="12" r="3"/><path d="M12 1v4M12 19v4M4.22 4.22l2.83 2.83M16.95 16.95l2.83 2.83M1 12h4M19 12h4M4.22 19.78l2.83-2.83M16.95 7.05l2.83-2.83"/></svg>
    <span class="repo-name">Classification Pipeline</span>
    <span class="repo-badge">AI</span>
  </div>
  <p class="repo-desc">End-to-end AI pipeline from raw field audio to species detection, classification, uncertainty quantification, and EBV computation.</p>
  <a href="https://github.com/BenMcEwen1/TABMON-Classification-Pipeline" class="pub-link" target="_blank">View on GitHub <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M7 17L17 7M17 7H7M17 7V17"/></svg></a>
</div>

<div class="repo-card">
  <div class="repo-header">
    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#10B981" stroke-width="1.5"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>
    <span class="repo-name">Report Generator</span>
    <span class="repo-badge">Reports</span>
  </div>
  <p class="repo-desc">Automated generation of yearly monitoring reports with site-level summaries, temporal trends, and publication-ready visualizations.</p>
  <a href="https://github.com/NINAnor/tabmon_reporting" class="pub-link" target="_blank">View on GitHub <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M7 17L17 7M17 7H7M17 7V17"/></svg></a>
</div>

<div class="repo-card">
  <div class="repo-header">
    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#FB7185" stroke-width="1.5"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>
    <span class="repo-name">Zenodo Archive</span>
    <span class="repo-badge">Data</span>
  </div>
  <p class="repo-desc">Published monitoring reports, datasets, and supplementary materials — DOI-registered, citable, and permanently archived.</p>
  <a href="https://zenodo.org/records/17899019" class="pub-link" target="_blank">View on Zenodo <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M7 17L17 7M17 7H7M17 7V17"/></svg></a>
</div>

</div>

---

## Data Access & Integration

TABMON data follows **FAIR principles** and is integrated into major biodiversity portals:

<div class="data-integration-grid">
  <div class="data-badge"><strong>GBIF</strong><span>Species occurrence data</span></div>
  <div class="data-badge"><strong>EBV Portal</strong><span>Essential Biodiversity Variables</span></div>
  <div class="data-badge"><strong>National Schemes</strong><span>Country-specific databases</span></div>
  <div class="data-badge"><strong>Zenodo & OSF</strong><span>Open science repositories</span></div>
</div>

All datasets include comprehensive metadata, versioning, clear licensing, and DOI registration.

---

<div class="pub-cta">
  <p>Interested in collaborating? We welcome partnerships in data analysis, model development, and regional monitoring expansions. <a href="/team/">Get in touch with our team!</a></p>
</div>
