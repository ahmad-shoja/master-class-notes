# Editorial Warm Paper Design System — Master Style Guide

This style guide documents the exact design system, CSS variables, typography, and component architecture used in the **Class B** interactive HTML page.

---

## 1. Design System Overview

The **Editorial Warm Paper / Craft** design system uses a warm, editorial paper aesthetic paired with high-contrast ink typography, golden yellow key highlights, deep teal accents, and clean card containers.

---

## 2. Color Tokens & CSS Variables

```css
:root {
  color-scheme: light;

  /* Page and Surfaces: Warm Stone-White Paper */
  --background: #faf9f5;
  --surface-container-low: #ffffff;
  --surface-container: #f1efe8;
  --surface-container-high: #e6e2d6;

  /* Ink & Typography */
  --on-surface: #17181a;             /* Primary Ink */
  --on-surface-variant: #56585c;     /* Muted / Secondary Text */

  /* Borders & Rules */
  --outline: #17181a;
  --outline-variant: #dedad0;

  /* Accent Colors */
  --primary: #17181a;
  --on-primary: #faf9f5;
  --primary-container: #f2b705;     /* Warm Golden Yellow Highlight */
  --on-primary-container: #17181a;
  --secondary: #1f4e5f;             /* Deep Teal Accent */
  --tertiary: #785008;              /* Dark Amber */

  /* Semantic UI States */
  --positive: #1f6b48;
  --positive-bg: #eaf5ef;
  --warning: #8a5600;
  --warning-bg: #fbf2de;
  --error: #b42318;
  --error-bg: #fceceb;

  /* Data Series Visualization */
  --data-1: #1f4e5f;
  --data-2: #d99000;
  --data-3: #2b6e52;
  --data-4: #b84a39;
  --data-context: #c4bfb2;
}
```

---

## 3. Core Component Architecture

### A. Navigation & Table of Contents (`.toc-strip`)
```html
<nav class="toc-strip">
  <a href="#overview" class="toc-link">Overview</a>
  <a href="#islands" class="toc-link">Application Islands</a>
  <a href="#styles" class="toc-link">4 Integration Styles</a>
  <a href="#eip" class="toc-link">EIP 65 Patterns</a>
</nav>
```

### B. Dossier Pills & Tag Chips (`.dossier-pill`, `.tag-chip`)
```html
<span class="dossier-pill">الگو | Pattern</span>
<span class="tag-chip">Week 8–9</span>
```

### C. KPI & Metric Cards (`.kpi-grid`)
```html
<div class="kpi-grid">
  <div class="kpi-card">
    <div class="kpi-value">65</div>
    <div class="kpi-label">Total EIP Patterns</div>
  </div>
  <div class="kpi-card">
    <div class="kpi-value">4</div>
    <div class="kpi-label">Core Integration Styles</div>
  </div>
</div>
```

### D. Callout & Payload Cards (`.payload-box`, `.deep-dive`)
```html
<div class="payload-box">
  <h4>Case Study: Azad University Portals</h4>
  <p>Disjointed administrative software silos including Amozesh-yar, Meyar, Pajouhesh-yar, and Sajed.</p>
</div>
```

---

## 4. Full Prompt Template for Other LLMs

```text
Generate a responsive, standalone HTML5 page using the Editorial Warm Paper design system:
1. Palette: Warm paper background (#faf9f5), primary ink text (#17181a), crisp white card surfaces (#ffffff), warm golden container highlights (#f2b705), and deep teal accents (#1f4e5f).
2. Structure: Top sticky TOC strip navigation, KPI summary metric cards, dossier tag pills for bilingual or technical terms, callout payload cards for case studies, and responsive comparison tables.
3. Typography: Clean modern sans-serif with proper RTL support for non-English terms.
```
