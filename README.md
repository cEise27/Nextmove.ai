root {
  --bg: #07111f;
  --panel: rgba(255, 255, 255, 0.05);
  --line: rgba(141, 199, 255, 0.2);
  --text: #edf5ff;
  --muted: #9db5cf;
  --highlight: #8df3c8;
  --bg: #08131d;
  --bg-deep: #051018;
  --surface: rgba(11, 31, 45, 0.78);
  --surface-strong: rgba(12, 36, 50, 0.94);
  --surface-soft: rgba(255, 255, 255, 0.06);
  --line: rgba(157, 216, 255, 0.16);
  --line-strong: rgba(157, 216, 255, 0.3);
  --text: #f4f9ff;
  --muted: #a9c1d4;
  --highlight: #ffcf5a;
  --highlight-soft: rgba(255, 207, 90, 0.18);
  --accent: #49dcb1;
  --danger: #ff8f6d;
  --shadow: 0 30px 90px rgba(0, 0, 0, 0.35);
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: "Segoe UI", sans-serif;
  background: linear-gradient(180deg, #07111f 0%, #0c1730 100%);
  min-height: 100vh;
  font-family: "Avenir Next", "Segoe UI", sans-serif;
  color: var(--text);
  background:
    radial-gradient(circle at top left, rgba(73, 220, 177, 0.18), transparent 28%),
    radial-gradient(circle at top right, rgba(255, 143, 109, 0.18), transparent 24%),
    linear-gradient(180deg, #0a1621 0%, #08131d 42%, #061018 100%);
}

.page {
  width: min(1100px, calc(100% - 32px));
body::before {
  content: "";
  position: fixed;
  inset: 0;
  pointer-events: none;
  background:
    linear-gradient(90deg, rgba(255, 255, 255, 0.02) 1px, transparent 1px),
    linear-gradient(rgba(255, 255, 255, 0.02) 1px, transparent 1px);
  background-size: 40px 40px;
  mask-image: linear-gradient(180deg, rgba(0, 0, 0, 0.65), transparent);
}

a {
  color: inherit;
  text-decoration: none;
}

button,
input,
select,
textarea {
  font: inherit;
}

.page-shell {
  width: min(1240px, calc(100% - 32px));
  margin: 0 auto;
  padding: 48px 0 80px;
  padding: 28px 0 90px;
}

.hero,
.content-section,
.mission-strip {
  position: relative;
  z-index: 1;
}

.hero {
  padding: 14px 0 24px;
}

.topbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
  margin-bottom: 28px;
}

.eyebrow {
.brand-block {
  display: flex;
  flex-direction: column;
  gap: 6px;
}

.brand-mark,
.eyebrow,
.eyebrow-panel,
.sport-chip,
.signal-weight,
.review-meta,
.spotlight-market,
.score-pill {
  text-transform: uppercase;
  letter-spacing: 0.18em;
}

.brand-mark {
  margin: 0;
  font-family: "Avenir Next Condensed", "Arial Narrow", sans-serif;
  font-size: 0.86rem;
  color: var(--highlight);
}

.brand-copy,
.topbar-note,
.section-copy,
.panel-copy,
.form-note,
.stat-card p,
.signal-card p,
.checklist-item p,
.review-card p,
.spotlight-card p,
.sport-headline,
.sport-audience,
.lede {
  color: var(--muted);
  line-height: 1.65;
}

.topbar-note {
  max-width: 420px;
  margin: 0;
  text-align: right;
}

.hero-grid {
  display: grid;
  grid-template-columns: minmax(0, 1.3fr) minmax(320px, 420px);
  gap: 24px;
  align-items: stretch;
}

.hero-copy,
.hero-panel,
.feature-card,
.sport-card,
.spotlight-card,
.stat-card,
.mission-strip {
  border: 1px solid var(--line);
  background: var(--surface);
  box-shadow: var(--shadow);
  backdrop-filter: blur(20px);
}

.hero-copy,
.hero-panel,
.feature-card {
  border-radius: 34px;
}

.hero-copy {
  padding: 42px;
  background:
    linear-gradient(135deg, rgba(255, 207, 90, 0.12), transparent 42%),
    linear-gradient(180deg, rgba(255, 255, 255, 0.04), transparent 100%),
    var(--surface-strong);
  animation: fade-up 0.7s ease both;
}

.hero-panel {
  padding: 28px;
  background:
    radial-gradient(circle at top right, rgba(73, 220, 177, 0.18), transparent 32%),
    linear-gradient(180deg, rgba(255, 255, 255, 0.05), transparent),
    var(--surface-strong);
  animation: fade-up 0.9s ease both;
}

.eyebrow,
.eyebrow-panel {
  margin: 0 0 12px;
  font-size: 0.75rem;
  color: var(--highlight);
}

.hero h1,
.content-section h2,
.mission-strip p,
.hero-panel h2 {
  font-family: "Avenir Next Condensed", "Arial Narrow", "Trebuchet MS", sans-serif;
  letter-spacing: 0.01em;
}

.hero h1 {
  margin: 0;
  max-width: 12ch;
  font-size: clamp(3.4rem, 6vw, 6.3rem);
  line-height: 0.94;
}

.lede {
  max-width: 64ch;
  margin: 20px 0 0;
  font-size: 1.08rem;
}

.hero-actions,
.cta-row {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  margin-top: 28px;
}

.button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 48px;
  padding: 0 20px;
  border-radius: 999px;
  border: 1px solid transparent;
  cursor: pointer;
  transition:
    transform 180ms ease,
    border-color 180ms ease,
    background 180ms ease;
}

.button:hover {
  transform: translateY(-2px);
}

.button-primary {
  background: linear-gradient(135deg, #ffcf5a, #ff9c58);
  color: #10202c;
  font-weight: 700;
}

.button-secondary {
  border-color: var(--line-strong);
  background: rgba(255, 255, 255, 0.04);
}

.score-row {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
  margin-bottom: 14px;
}

.score-label,
.mini-label {
  margin: 0;
  font-size: 0.82rem;
  color: var(--muted);
  text-transform: uppercase;
  letter-spacing: 0.12em;
}

.score-value {
  margin: 8px 0 0;
  font-size: 4rem;
  line-height: 0.9;
  font-family: "Avenir Next Condensed", "Arial Narrow", sans-serif;
}

.score-pill {
  margin: 0;
  padding: 10px 14px;
  border-radius: 999px;
  background: var(--highlight-soft);
  color: var(--highlight);
  font-size: 0.72rem;
}

.hero-panel h2,
.content-section h2 {
  margin: 0;
  font-size: clamp(2rem, 3.4vw, 3.2rem);
  line-height: 0.95;
}

.hero-panel h2 {
  font-size: 2.15rem;
  margin-bottom: 16px;
}

.panel-stack {
  display: grid;
  gap: 18px;
  margin-top: 24px;
}

.lede,
.muted {
.bullet-list {
  margin: 12px 0 0;
  padding-left: 18px;
  display: grid;
  gap: 12px;
}

.bullet-list-muted {
  color: var(--muted);
  line-height: 1.6;
}

.grid {
.stats-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 20px;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 18px;
  margin-top: 24px;
}

.card {
  padding: 20px;
.stat-card {
  padding: 20px 22px;
  border-radius: 24px;
  animation: fade-up 1s ease both;
}

.stat-card:nth-child(2) {
  animation-delay: 60ms;
}

.stat-card:nth-child(3) {
  animation-delay: 120ms;
}

.stat-card:nth-child(4) {
  animation-delay: 180ms;
}

.stat-value {
  margin: 0 0 10px;
  font-size: 2rem;
  color: var(--highlight);
  font-family: "Avenir Next Condensed", "Arial Narrow", sans-serif;
}

.stat-card h2 {
  margin: 0 0 8px;
  font-size: 1.15rem;
}

.mission-strip {
  margin: 18px 0 30px;
  padding: 22px 26px;
  border-radius: 26px;
  background:
    linear-gradient(90deg, rgba(73, 220, 177, 0.16), rgba(255, 207, 90, 0.12)),
    var(--surface);
}

.mission-strip p {
  margin: 0;
  font-size: 1.35rem;
  line-height: 1.2;
}

.content-section {
  margin-top: 28px;
}

.section-heading {
  display: grid;
  gap: 10px;
  max-width: 760px;
  margin-bottom: 18px;
}

.section-heading p {
  margin: 0;
}

.sport-grid,
.spotlight-grid {
  display: grid;
  gap: 18px;
}

.sport-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.spotlight-grid {
  grid-template-columns: repeat(5, minmax(0, 1fr));
}

.sport-card,
.spotlight-card {
  position: relative;
  overflow: hidden;
}

.sport-card {
  padding: 24px;
  border-radius: 28px;
}

.sport-card::before,
.spotlight-card::before {
  content: "";
  position: absolute;
  inset: 0 auto auto 0;
  width: 100%;
  height: 4px;
  background: linear-gradient(90deg, rgba(255, 255, 255, 0), currentColor, rgba(255, 255, 255, 0));
  opacity: 0.8;
}

.sport-card--hockey,
.spotlight-card--hockey {
  color: #7ec7ff;
}

.sport-card--soccer,
.spotlight-card--soccer {
  color: #6fe29f;
}

.sport-card--lacrosse,
.spotlight-card--lacrosse {
  color: #ffb56b;
}

.sport-card--basketball,
.spotlight-card--basketball {
  color: #ff8f6d;
}

.sport-card--football,
.spotlight-card--football {
  color: #c0a2ff;
}

.sport-card > *,
.spotlight-card > * {
  position: relative;
  z-index: 1;
}

.sport-card-top,
.spotlight-header,
.spotlight-footer,
.review-meta {
  display: flex;
  justify-content: space-between;
  gap: 14px;
}

.sport-card-top {
  align-items: center;
}

.sport-chip {
  margin: 0;
  min-width: 56px;
  padding: 12px 14px;
  border-radius: 16px;
  background: rgba(255, 255, 255, 0.08);
  text-align: center;
  font-size: 0.78rem;
  color: currentColor;
}

.sport-audience {
  margin: 0;
  text-align: right;
}

.sport-card h3,
.signal-card h3,
.checklist-item h3,
.review-card h3,
.spotlight-card h3 {
  margin: 16px 0 10px;
  font-size: 1.25rem;
  color: var(--text);
}

.tag-row {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 18px;
}

.tag-row-secondary {
  margin-top: 12px;
}

.tag {
  display: inline-flex;
  align-items: center;
  min-height: 34px;
  padding: 0 12px;
  border-radius: 999px;
  border: 1px solid rgba(255, 255, 255, 0.12);
  background: rgba(255, 255, 255, 0.06);
  color: var(--text);
  font-size: 0.88rem;
}

.tag-muted {
  color: var(--muted);
}

.sport-detail {
  margin-top: 18px;
}

.pathway-list {
  margin: 12px 0 0;
  padding-left: 18px;
  display: grid;
  gap: 12px;
}

.pathway-list li {
  display: grid;
  gap: 4px;
}

.pathway-list span {
  color: var(--muted);
  line-height: 1.55;
}

.feature-grid,
.review-layout {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 18px;
}

.feature-card {
  padding: 28px;
}

.feature-card-contrast {
  background:
    linear-gradient(180deg, rgba(255, 207, 90, 0.08), transparent 35%),
    var(--surface-strong);
}

.signal-grid,
.checklist,
.review-grid {
  display: grid;
  gap: 14px;
  margin-top: 22px;
}

.signal-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.signal-card,
.checklist-item,
.review-card {
  padding: 18px;
  border-radius: 22px;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.08);
}

.signal-weight {
  margin: 0;
  font-size: 0.7rem;
  color: var(--highlight);
}

.spotlight-card {
  padding: 22px;
  border-radius: 26px;
  background:
    linear-gradient(180deg, rgba(255, 255, 255, 0.03), transparent),
    var(--surface);
}

.spotlight-header {
  align-items: flex-start;
}

.spotlight-market {
  margin: 0 0 8px;
  font-size: 0.7rem;
  color: currentColor;
}

.score-badge {
  min-width: 82px;
  padding: 12px;
  border-radius: 20px;
  background: rgba(255, 255, 255, 0.08);
  text-align: center;
}

.score-badge span {
  display: block;
  font-size: 2rem;
  line-height: 1;
  color: var(--text);
  font-family: "Avenir Next Condensed", "Arial Narrow", sans-serif;
}

.score-badge small {
  color: var(--muted);
  text-transform: uppercase;
  letter-spacing: 0.12em;
}

.spotlight-level,
.review-outcome {
  color: var(--highlight);
}

.spotlight-body {
  display: grid;
  gap: 14px;
  margin-top: 18px;
}

.spotlight-footer {
  margin-top: 18px;
  align-items: center;
  flex-wrap: wrap;
}

.review-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.review-card--hockey {
  box-shadow: inset 0 0 0 1px rgba(126, 199, 255, 0.18);
}

.review-card--soccer {
  box-shadow: inset 0 0 0 1px rgba(111, 226, 159, 0.18);
}

.review-card--lacrosse {
  box-shadow: inset 0 0 0 1px rgba(255, 181, 107, 0.18);
}

.review-card--basketball {
  box-shadow: inset 0 0 0 1px rgba(255, 143, 109, 0.18);
}

.review-card--football {
  box-shadow: inset 0 0 0 1px rgba(192, 162, 255, 0.18);
}

.review-meta {
  align-items: center;
  margin-bottom: 10px;
  font-size: 0.72rem;
  color: var(--muted);
}

.review-quote {
  color: var(--text);
}

.review-form {
  display: grid;
  gap: 14px;
  margin-top: 22px;
}

.review-form label {
  display: grid;
  gap: 8px;
  color: var(--text);
}

.review-form input,
.review-form select,
.review-form textarea {
  width: 100%;
  border: 1px solid var(--line);
  border-radius: 18px;
  background: rgba(2, 11, 18, 0.56);
  color: var(--text);
  padding: 14px 16px;
}

.review-form textarea {
  resize: vertical;
}

.review-categories {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
}

.category-pill {
  display: grid;
  gap: 6px;
  padding: 14px;
  border-radius: 18px;
  border: 1px solid var(--line);
  background: var(--panel);
  background: rgba(255, 255, 255, 0.05);
}

@media (max-width: 900px) {
  .grid {
.category-pill span {
  color: var(--muted);
  line-height: 1.5;
}

.closing-panel {
  margin-top: 28px;
  padding: 34px;
  border-radius: 34px;
  border: 1px solid var(--line);
  background:
    radial-gradient(circle at top left, rgba(255, 207, 90, 0.14), transparent 28%),
    linear-gradient(180deg, rgba(255, 255, 255, 0.05), transparent),
    var(--surface-strong);
  box-shadow: var(--shadow);
}

@keyframes fade-up {
  from {
    opacity: 0;
    transform: translateY(24px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@media (max-width: 1180px) {
  .spotlight-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .hero h1 {
    max-width: 14ch;
  }
}

@media (max-width: 960px) {
  .topbar,
  .hero-grid,
  .feature-grid,
  .review-layout,
  .sport-grid,
  .stats-grid,
  .signal-grid,
  .review-grid,
  .review-categories,
  .spotlight-grid {
    grid-template-columns: 1fr;
  }

  .topbar,
  .sport-card-top,
  .spotlight-header,
  .spotlight-footer,
  .review-meta,
  .hero-actions,
  .cta-row {
    flex-direction: column;
    align-items: flex-start;
  }

  .topbar-note,
  .sport-audience {
    text-align: left;
  }

  .hero-copy,
  .hero-panel,
  .feature-card,
  .sport-card,
  .spotlight-card,
  .closing-panel {
    padding: 24px;
  }

  .hero h1 {
    font-size: clamp(2.8rem, 13vw, 4.5rem);
    max-width: none;
  }

  .mission-strip p {
    font-size: 1.15rem;
  }

  .score-row {
    align-items: flex-start;
    flex-direction: column;
  }
}

@media (max-width: 640px) {
  .page-shell {
    width: min(100% - 20px, 1240px);
    padding-bottom: 56px;
  }

  .hero-copy,
  .hero-panel,
  .feature-card,
  .sport-card,
  .spotlight-card,
  .stat-card,
  .closing-panel,
  .mission-strip {
    border-radius: 24px;
  }

  .button {
    width: 100%;
  }
}
root {
  --bg: #07111f;
  --panel: rgba(255, 255, 255, 0.05);
  --line: rgba(141, 199, 255, 0.2);
  --text: #edf5ff;
  --muted: #9db5cf;
  --highlight: #8df3c8;
  --bg: #08131d;
  --bg-deep: #051018;
  --surface: rgba(11, 31, 45, 0.78);
  --surface-strong: rgba(12, 36, 50, 0.94);
  --surface-soft: rgba(255, 255, 255, 0.06);
  --line: rgba(157, 216, 255, 0.16);
  --line-strong: rgba(157, 216, 255, 0.3);
  --text: #f4f9ff;
  --muted: #a9c1d4;
  --highlight: #ffcf5a;
  --highlight-soft: rgba(255, 207, 90, 0.18);
  --accent: #49dcb1;
  --danger: #ff8f6d;
  --shadow: 0 30px 90px rgba(0, 0, 0, 0.35);
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: "Segoe UI", sans-serif;
  background: linear-gradient(180deg, #07111f 0%, #0c1730 100%);
  min-height: 100vh;
  font-family: "Avenir Next", "Segoe UI", sans-serif;
  color: var(--text);
  background:
    radial-gradient(circle at top left, rgba(73, 220, 177, 0.18), transparent 28%),
    radial-gradient(circle at top right, rgba(255, 143, 109, 0.18), transparent 24%),
    linear-gradient(180deg, #0a1621 0%, #08131d 42%, #061018 100%);
}

.page {
  width: min(1100px, calc(100% - 32px));
body::before {
  content: "";
  position: fixed;
  inset: 0;
  pointer-events: none;
  background:
    linear-gradient(90deg, rgba(255, 255, 255, 0.02) 1px, transparent 1px),
    linear-gradient(rgba(255, 255, 255, 0.02) 1px, transparent 1px);
  background-size: 40px 40px;
  mask-image: linear-gradient(180deg, rgba(0, 0, 0, 0.65), transparent);
}

a {
  color: inherit;
  text-decoration: none;
}

button,
input,
select,
textarea {
  font: inherit;
}

.page-shell {
  width: min(1240px, calc(100% - 32px));
  margin: 0 auto;
  padding: 48px 0 80px;
  padding: 28px 0 90px;
}

.hero,
.content-section,
.mission-strip {
  position: relative;
  z-index: 1;
}

.hero {
  padding: 14px 0 24px;
}

.topbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
  margin-bottom: 28px;
}

.eyebrow {
.brand-block {
  display: flex;
  flex-direction: column;
  gap: 6px;
}

.brand-mark,
.eyebrow,
.eyebrow-panel,
.sport-chip,
.signal-weight,
.review-meta,
.spotlight-market,
.score-pill {
  text-transform: uppercase;
  letter-spacing: 0.18em;
}

.brand-mark {
  margin: 0;
  font-family: "Avenir Next Condensed", "Arial Narrow", sans-serif;
  font-size: 0.86rem;
  color: var(--highlight);
}

.brand-copy,
.topbar-note,
.section-copy,
.panel-copy,
.form-note,
.stat-card p,
.signal-card p,
.checklist-item p,
.review-card p,
.spotlight-card p,
.sport-headline,
.sport-audience,
.lede {
  color: var(--muted);
  line-height: 1.65;
}

.topbar-note {
  max-width: 420px;
  margin: 0;
  text-align: right;
}

.hero-grid {
  display: grid;
  grid-template-columns: minmax(0, 1.3fr) minmax(320px, 420px);
  gap: 24px;
  align-items: stretch;
}

.hero-copy,
.hero-panel,
.feature-card,
.sport-card,
.spotlight-card,
.stat-card,
.mission-strip {
  border: 1px solid var(--line);
  background: var(--surface);
  box-shadow: var(--shadow);
  backdrop-filter: blur(20px);
}

.hero-copy,
.hero-panel,
.feature-card {
  border-radius: 34px;
}

.hero-copy {
  padding: 42px;
  background:
    linear-gradient(135deg, rgba(255, 207, 90, 0.12), transparent 42%),
    linear-gradient(180deg, rgba(255, 255, 255, 0.04), transparent 100%),
    var(--surface-strong);
  animation: fade-up 0.7s ease both;
}

.hero-panel {
  padding: 28px;
  background:
    radial-gradient(circle at top right, rgba(73, 220, 177, 0.18), transparent 32%),
    linear-gradient(180deg, rgba(255, 255, 255, 0.05), transparent),
    var(--surface-strong);
  animation: fade-up 0.9s ease both;
}

.eyebrow,
.eyebrow-panel {
  margin: 0 0 12px;
  font-size: 0.75rem;
  color: var(--highlight);
}

.hero h1,
.content-section h2,
.mission-strip p,
.hero-panel h2 {
  font-family: "Avenir Next Condensed", "Arial Narrow", "Trebuchet MS", sans-serif;
  letter-spacing: 0.01em;
}

.hero h1 {
  margin: 0;
  max-width: 12ch;
  font-size: clamp(3.4rem, 6vw, 6.3rem);
  line-height: 0.94;
}

.lede {
  max-width: 64ch;
  margin: 20px 0 0;
  font-size: 1.08rem;
}

.hero-actions,
.cta-row {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  margin-top: 28px;
}

.button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 48px;
  padding: 0 20px;
  border-radius: 999px;
  border: 1px solid transparent;
  cursor: pointer;
  transition:
    transform 180ms ease,
    border-color 180ms ease,
    background 180ms ease;
}

.button:hover {
  transform: translateY(-2px);
}

.button-primary {
  background: linear-gradient(135deg, #ffcf5a, #ff9c58);
  color: #10202c;
  font-weight: 700;
}

.button-secondary {
  border-color: var(--line-strong);
  background: rgba(255, 255, 255, 0.04);
}

.score-row {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
  margin-bottom: 14px;
}

.score-label,
.mini-label {
  margin: 0;
  font-size: 0.82rem;
  color: var(--muted);
  text-transform: uppercase;
  letter-spacing: 0.12em;
}

.score-value {
  margin: 8px 0 0;
  font-size: 4rem;
  line-height: 0.9;
  font-family: "Avenir Next Condensed", "Arial Narrow", sans-serif;
}

.score-pill {
  margin: 0;
  padding: 10px 14px;
  border-radius: 999px;
  background: var(--highlight-soft);
  color: var(--highlight);
  font-size: 0.72rem;
}

.hero-panel h2,
.content-section h2 {
  margin: 0;
  font-size: clamp(2rem, 3.4vw, 3.2rem);
  line-height: 0.95;
}

.hero-panel h2 {
  font-size: 2.15rem;
  margin-bottom: 16px;
}

.panel-stack {
  display: grid;
  gap: 18px;
  margin-top: 24px;
}

.lede,
.muted {
.bullet-list {
  margin: 12px 0 0;
  padding-left: 18px;
  display: grid;
  gap: 12px;
}

.bullet-list-muted {
  color: var(--muted);
  line-height: 1.6;
}

.grid {
.stats-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 20px;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 18px;
  margin-top: 24px;
}

.card {
  padding: 20px;
.stat-card {
  padding: 20px 22px;
  border-radius: 24px;
  animation: fade-up 1s ease both;
}

.stat-card:nth-child(2) {
  animation-delay: 60ms;
}

.stat-card:nth-child(3) {
  animation-delay: 120ms;
}

.stat-card:nth-child(4) {
  animation-delay: 180ms;
}

.stat-value {
  margin: 0 0 10px;
  font-size: 2rem;
  color: var(--highlight);
  font-family: "Avenir Next Condensed", "Arial Narrow", sans-serif;
}

.stat-card h2 {
  margin: 0 0 8px;
  font-size: 1.15rem;
}

.mission-strip {
  margin: 18px 0 30px;
  padding: 22px 26px;
  border-radius: 26px;
  background:
    linear-gradient(90deg, rgba(73, 220, 177, 0.16), rgba(255, 207, 90, 0.12)),
    var(--surface);
}

.mission-strip p {
  margin: 0;
  font-size: 1.35rem;
  line-height: 1.2;
}

.content-section {
  margin-top: 28px;
}

.section-heading {
  display: grid;
  gap: 10px;
  max-width: 760px;
  margin-bottom: 18px;
}

.section-heading p {
  margin: 0;
}

.sport-grid,
.spotlight-grid {
  display: grid;
  gap: 18px;
}

.sport-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.spotlight-grid {
  grid-template-columns: repeat(5, minmax(0, 1fr));
}

.sport-card,
.spotlight-card {
  position: relative;
  overflow: hidden;
}

.sport-card {
  padding: 24px;
  border-radius: 28px;
}

.sport-card::before,
.spotlight-card::before {
  content: "";
  position: absolute;
  inset: 0 auto auto 0;
  width: 100%;
  height: 4px;
  background: linear-gradient(90deg, rgba(255, 255, 255, 0), currentColor, rgba(255, 255, 255, 0));
  opacity: 0.8;
}

.sport-card--hockey,
.spotlight-card--hockey {
  color: #7ec7ff;
}

.sport-card--soccer,
.spotlight-card--soccer {
  color: #6fe29f;
}

.sport-card--lacrosse,
.spotlight-card--lacrosse {
  color: #ffb56b;
}

.sport-card--basketball,
.spotlight-card--basketball {
  color: #ff8f6d;
}

.sport-card--football,
.spotlight-card--football {
  color: #c0a2ff;
}

.sport-card > *,
.spotlight-card > * {
  position: relative;
  z-index: 1;
}

.sport-card-top,
.spotlight-header,
.spotlight-footer,
.review-meta {
  display: flex;
  justify-content: space-between;
  gap: 14px;
}

.sport-card-top {
  align-items: center;
}

.sport-chip {
  margin: 0;
  min-width: 56px;
  padding: 12px 14px;
  border-radius: 16px;
  background: rgba(255, 255, 255, 0.08);
  text-align: center;
  font-size: 0.78rem;
  color: currentColor;
}

.sport-audience {
  margin: 0;
  text-align: right;
}

.sport-card h3,
.signal-card h3,
.checklist-item h3,
.review-card h3,
.spotlight-card h3 {
  margin: 16px 0 10px;
  font-size: 1.25rem;
  color: var(--text);
}

.tag-row {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 18px;
}

.tag-row-secondary {
  margin-top: 12px;
}

.tag {
  display: inline-flex;
  align-items: center;
  min-height: 34px;
  padding: 0 12px;
  border-radius: 999px;
  border: 1px solid rgba(255, 255, 255, 0.12);
  background: rgba(255, 255, 255, 0.06);
  color: var(--text);
  font-size: 0.88rem;
}

.tag-muted {
  color: var(--muted);
}

.sport-detail {
  margin-top: 18px;
}

.pathway-list {
  margin: 12px 0 0;
  padding-left: 18px;
  display: grid;
  gap: 12px;
}

.pathway-list li {
  display: grid;
  gap: 4px;
}

.pathway-list span {
  color: var(--muted);
  line-height: 1.55;
}

.feature-grid,
.review-layout {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 18px;
}

.feature-card {
  padding: 28px;
}

.feature-card-contrast {
  background:
    linear-gradient(180deg, rgba(255, 207, 90, 0.08), transparent 35%),
    var(--surface-strong);
}

.signal-grid,
.checklist,
.review-grid {
  display: grid;
  gap: 14px;
  margin-top: 22px;
}

.signal-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.signal-card,
.checklist-item,
.review-card {
  padding: 18px;
  border-radius: 22px;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.08);
}

.signal-weight {
  margin: 0;
  font-size: 0.7rem;
  color: var(--highlight);
}

.spotlight-card {
  padding: 22px;
  border-radius: 26px;
  background:
    linear-gradient(180deg, rgba(255, 255, 255, 0.03), transparent),
    var(--surface);
}

.spotlight-header {
  align-items: flex-start;
}

.spotlight-market {
  margin: 0 0 8px;
  font-size: 0.7rem;
  color: currentColor;
}

.score-badge {
  min-width: 82px;
  padding: 12px;
  border-radius: 20px;
  background: rgba(255, 255, 255, 0.08);
  text-align: center;
}

.score-badge span {
  display: block;
  font-size: 2rem;
  line-height: 1;
  color: var(--text);
  font-family: "Avenir Next Condensed", "Arial Narrow", sans-serif;
}

.score-badge small {
  color: var(--muted);
  text-transform: uppercase;
  letter-spacing: 0.12em;
}

.spotlight-level,
.review-outcome {
  color: var(--highlight);
}

.spotlight-body {
  display: grid;
  gap: 14px;
  margin-top: 18px;
}

.spotlight-footer {
  margin-top: 18px;
  align-items: center;
  flex-wrap: wrap;
}

.review-grid {
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.review-card--hockey {
  box-shadow: inset 0 0 0 1px rgba(126, 199, 255, 0.18);
}

.review-card--soccer {
  box-shadow: inset 0 0 0 1px rgba(111, 226, 159, 0.18);
}

.review-card--lacrosse {
  box-shadow: inset 0 0 0 1px rgba(255, 181, 107, 0.18);
}

.review-card--basketball {
  box-shadow: inset 0 0 0 1px rgba(255, 143, 109, 0.18);
}

.review-card--football {
  box-shadow: inset 0 0 0 1px rgba(192, 162, 255, 0.18);
}

.review-meta {
  align-items: center;
  margin-bottom: 10px;
  font-size: 0.72rem;
  color: var(--muted);
}

.review-quote {
  color: var(--text);
}

.review-form {
  display: grid;
  gap: 14px;
  margin-top: 22px;
}

.review-form label {
  display: grid;
  gap: 8px;
  color: var(--text);
}

.review-form input,
.review-form select,
.review-form textarea {
  width: 100%;
  border: 1px solid var(--line);
  border-radius: 18px;
  background: rgba(2, 11, 18, 0.56);
  color: var(--text);
  padding: 14px 16px;
}

.review-form textarea {
  resize: vertical;
}

.review-categories {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 12px;
}

.category-pill {
  display: grid;
  gap: 6px;
  padding: 14px;
  border-radius: 18px;
  border: 1px solid var(--line);
  background: var(--panel);
  background: rgba(255, 255, 255, 0.05);
}

@media (max-width: 900px) {
  .grid {
.category-pill span {
  color: var(--muted);
  line-height: 1.5;
}

.closing-panel {
  margin-top: 28px;
  padding: 34px;
  border-radius: 34px;
  border: 1px solid var(--line);
  background:
    radial-gradient(circle at top left, rgba(255, 207, 90, 0.14), transparent 28%),
    linear-gradient(180deg, rgba(255, 255, 255, 0.05), transparent),
    var(--surface-strong);
  box-shadow: var(--shadow);
}

@keyframes fade-up {
  from {
    opacity: 0;
    transform: translateY(24px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@media (max-width: 1180px) {
  .spotlight-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .hero h1 {
    max-width: 14ch;
  }
}

@media (max-width: 960px) {
  .topbar,
  .hero-grid,
  .feature-grid,
  .review-layout,
  .sport-grid,
  .stats-grid,
  .signal-grid,
  .review-grid,
  .review-categories,
  .spotlight-grid {
    grid-template-columns: 1fr;
  }

  .topbar,
  .sport-card-top,
  .spotlight-header,
  .spotlight-footer,
  .review-meta,
  .hero-actions,
  .cta-row {
    flex-direction: column;
    align-items: flex-start;
  }

  .topbar-note,
  .sport-audience {
    text-align: left;
  }

  .hero-copy,
  .hero-panel,
  .feature-card,
  .sport-card,
  .spotlight-card,
  .closing-panel {
    padding: 24px;
  }

  .hero h1 {
    font-size: clamp(2.8rem, 13vw, 4.5rem);
    max-width: none;
  }

  .mission-strip p {
    font-size: 1.15rem;
  }

  .score-row {
    align-items: flex-start;
    flex-direction: column;
  }
}

@media (max-width: 640px) {
  .page-shell {
    width: min(100% - 20px, 1240px);
    padding-bottom: 56px;
  }

  .hero-copy,
  .hero-panel,
  .feature-card,
  .sport-card,
  .spotlight-card,
  .stat-card,
  .closing-panel,
  .mission-strip {
    border-radius: 24px;
  }

  .button {
    width: 100%;
  }
}
