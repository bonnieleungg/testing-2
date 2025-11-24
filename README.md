<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <title>YouFind AIPO｜Search Visibility Cloud & AI 搜尋能見度</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="YouFind AIPO Search Visibility Cloud：結合 SEO、AIPO、UMOT 與 Full Funnel Growth，打造 AI 搜尋時代的搜尋能見度雲與產品化方案。" />
  <style>
    :root {
      --color-bg-root: radial-gradient(circle at top left, #020617 0%, #020617 35%, #000 100%);
      --color-bg-dark: #020617;
      --color-bg-darker: #00010a;
      --color-bg-alt: #050816;
      --color-surface: #050816;
      --color-surface-soft: rgba(15, 23, 42, 0.88);
      --color-surface-alt: #0b1120;
      --color-surface-card: rgba(15, 23, 42, 0.78);
      --color-border: rgba(148, 163, 184, 0.35);
      --color-border-soft: rgba(148, 163, 184, 0.15);
      --color-text-main: #e5e7eb;
      --color-text-muted: #94a3b8;
      --color-text-soft: #64748b;
      --color-accent: #22c55e;
      --color-accent-soft: rgba(34, 197, 94, 0.18);
      --color-accent-strong: #16a34a;
      --color-danger: #ef4444;
      --shadow-soft: 0 20px 60px rgba(15, 23, 42, 0.8);
      --shadow-card: 0 18px 40px rgba(15, 23, 42, 0.65);
      --radius-xl: 26px;
      --radius-lg: 20px;
      --radius-md: 14px;
      --radius-sm: 10px;
      --max-width: 1180px;
    }

    * ,
    *::before,
    *::after {
      box-sizing: border-box;
    }

    html,
    body {
      margin: 0;
      padding: 0;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "SF Pro Text", "Noto Sans TC", sans-serif;
      background: var(--color-bg-root);
      color: var(--color-text-main);
      line-height: 1.7;
    }

    body {
      background-attachment: fixed;
    }

    img {
      max-width: 100%;
      display: block;
      border-radius: var(--radius-md);
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    /* Global layout */

    .page-shell {
      min-height: 100vh;
      background:
        radial-gradient(circle at 10% 0%, rgba(56, 189, 248, 0.16), transparent 52%),
        radial-gradient(circle at 90% 20%, rgba(34, 197, 94, 0.16), transparent 55%),
        radial-gradient(circle at 50% 120%, rgba(94, 234, 212, 0.16), transparent 60%),
        var(--color-bg-root);
    }

    .container {
      width: 100%;
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 0 22px;
      position: relative;
    }

    .section {
      padding: 80px 0;
      position: relative;
    }

    .section-alt {
      padding: 80px 0;
      position: relative;
    }

    .section::before {
      content: "";
      position: absolute;
      left: 50%;
      top: 0;
      width: 0;
      height: 1px;
      transform: translateX(-50%);
      background: linear-gradient(90deg,
        transparent 0%,
        rgba(148, 163, 184, 0.25) 20%,
        rgba(148, 163, 184, 0.35) 50%,
        rgba(148, 163, 184, 0.25) 80%,
        transparent 100%);
      opacity: 0.8;
    }

    h1, h2, h3, h4 {
      margin: 0 0 12px;
      line-height: 1.35;
    }

    h2 {
      font-size: 1.9rem;
      letter-spacing: 0.02em;
    }

    p {
      margin: 0 0 10px;
    }

    ul {
      padding-left: 20px;
      margin: 6px 0 10px;
    }

    li {
      margin-bottom: 4px;
    }

    /* Pills & tags */

    .tag {
      display: inline-flex;
      align-items: center;
      padding: 4px 11px;
      border-radius: 999px;
      font-size: 0.73rem;
      background: radial-gradient(circle at 0 0, rgba(56, 189, 248, 0.28), transparent 55%);
      color: #e5e7eb;
      border: 1px solid rgba(148, 163, 184, 0.6);
      gap: 6px;
      backdrop-filter: blur(22px);
    }

    .tag::before {
      content: "";
      width: 7px;
      height: 7px;
      border-radius: 999px;
      background: radial-gradient(circle, #4ade80, #22c55e);
      box-shadow: 0 0 0 4px rgba(34, 197, 94, 0.28);
    }

    /* Header */

    .site-header {
      position: sticky;
      top: 0;
      z-index: 40;
      background: radial-gradient(circle at 0 0, rgba(59, 130, 246, 0.12), transparent 40%) rgba(2, 6, 23, 0.96);
      border-bottom: 1px solid rgba(148, 163, 184, 0.45);
      backdrop-filter: blur(22px);
    }

    .nav-container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 70px;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 8px;
      color: #f9fafb;
    }

    .logo-mark {
      width: 30px;
      height: 30px;
      border-radius: 12px;
      background:
        conic-gradient(from 210deg, #22c55e, #22c55e 20%, #22c55e 35%, #22c55e 60%, #4ade80 80%, #22c55e 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 700;
      font-size: 0.8rem;
      box-shadow: 0 0 0 1px rgba(15, 23, 42, 0.9), 0 10px 22px rgba(22, 163, 74, 0.45);
    }

    .logo-text {
      font-weight: 600;
      letter-spacing: 0.14em;
      font-size: 0.95rem;
      text-transform: uppercase;
    }

    .main-nav {
      display: flex;
      gap: 18px;
      font-size: 0.88rem;
      color: #cbd5f5;
    }

    .main-nav a {
      padding: 5px 0;
      border-bottom: 2px solid transparent;
      opacity: 0.88;
      transition: opacity 0.16s ease, border-color 0.16s ease, transform 0.1s ease;
    }

    .main-nav a:hover {
      opacity: 1;
      border-color: var(--color-accent);
      transform: translateY(-1px);
    }

    /* Buttons */

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 9px 18px;
      border-radius: 999px;
      font-size: 0.9rem;
      font-weight: 500;
      border: 1px solid transparent;
      cursor: pointer;
      transition:
        background 0.18s ease,
        color 0.18s ease,
        border-color 0.18s ease,
        transform 0.12s ease,
        box-shadow 0.18s ease;
      white-space: nowrap;
    }

    .btn-primary {
      background: radial-gradient(circle at 0 0, #4ade80, #22c55e);
      color: #022c22;
      box-shadow: 0 18px 36px rgba(22, 163, 74, 0.7);
    }

    .btn-primary:hover {
      transform: translateY(-1px) translateZ(0);
      box-shadow: 0 22px 48px rgba(22, 163, 74, 0.9);
    }

    .btn-outline {
      border-color: rgba(148, 163, 184, 0.8);
      color: #e5e7eb;
      background: rgba(15, 23, 42, 0.4);
      backdrop-filter: blur(18px);
    }

    .btn-outline:hover {
      border-color: var(--color-accent);
      color: #f9fafb;
      background: rgba(15, 23, 42, 0.8);
    }

    .btn-light {
      background: rgba(15, 23, 42, 0.8);
      color: #e5e7eb;
      border-color: rgba(148, 163, 184, 0.6);
      box-shadow: 0 12px 28px rgba(15, 23, 42, 0.9);
    }

    .btn-light:hover {
      background: rgba(15, 23, 42, 1);
      border-color: var(--color-accent);
      color: #ecfeff;
    }

    .btn-full {
      width: 100%;
      margin-top: 12px;
    }

    /* Hero */

    .hero {
      position: relative;
      padding: 88px 0 80px;
    }

    .hero::before {
      content: "";
      position: absolute;
      inset: 0;
      background:
        radial-gradient(circle at 0 0, rgba(59, 130, 246, 0.16), transparent 52%),
        radial-gradient(circle at 100% 0, rgba(34, 197, 94, 0.22), transparent 55%);
      opacity: 0.86;
      pointer-events: none;
    }

    .hero-inner {
      position: relative;
      z-index: 1;
      border-radius: 36px;
      padding: 26px 26px 26px;
      background:
        radial-gradient(circle at top left, rgba(30, 64, 175, 0.45), transparent 60%),
        linear-gradient(135deg, rgba(15, 23, 42, 0.95), rgba(15, 23, 42, 0.9));
      border: 1px solid rgba(148, 163, 184, 0.5);
      box-shadow: var(--shadow-soft);
      overflow: hidden;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.35fr) minmax(0, 1fr);
      gap: 38px;
      align-items: center;
    }

    .hero-kicker {
      margin-bottom: 10px;
      display: flex;
      align-items: center;
      gap: 8px;
      font-size: 0.8rem;
      color: #a5b4fc;
    }

    .hero-kicker span {
      padding: 3px 10px;
      border-radius: 999px;
      background: radial-gradient(circle at 0 0, rgba(15, 23, 42, 0.92), rgba(15, 23, 42, 0.9));
      border: 1px solid rgba(129, 140, 248, 0.5);
    }

    .hero h1 {
      font-size: 2.25rem;
      margin-bottom: 10px;
      color: #f9fafb;
      letter-spacing: 0.02em;
    }

    .hero p {
      color: #cbd5f5;
      font-size: 0.98rem;
      max-width: 580px;
    }

    .hero-cta {
      margin: 18px 0 12px;
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .hero-sub {
      font-size: 0.84rem;
      color: #9ca3af;
    }

    .hero-bullets {
      margin-top: 12px;
      font-size: 0.84rem;
      color: #cbd5f5;
      list-style: none;
      padding-left: 0;
    }

    .hero-bullets li {
      position: relative;
      padding-left: 18px;
      margin-bottom: 4px;
    }

    .hero-bullets li::before {
      content: "";
      position: absolute;
      left: 0;
      top: 10px;
      width: 8px;
      height: 8px;
      border-radius: 999px;
      background: radial-gradient(circle, #4ade80, #22c55e);
      box-shadow: 0 0 0 3px rgba(34, 197, 94, 0.22);
    }

    .hero-visual {
      display: flex;
      justify-content: flex-end;
    }

    .glass-card {
      position: relative;
      border-radius: var(--radius-xl);
      padding: 18px 18px 16px;
      background: linear-gradient(135deg, rgba(15, 23, 42, 0.94), rgba(15, 23, 42, 0.88));
      border: 1px solid rgba(148, 163, 184, 0.55);
      box-shadow: var(--shadow-card);
      overflow: hidden;
      backdrop-filter: blur(26px);
      max-width: 380px;
    }

    .glass-card::before {
      content: "";
      position: absolute;
      inset: 0;
      background:
        radial-gradient(circle at 0 0, rgba(34, 197, 94, 0.22), transparent 50%),
        radial-gradient(circle at 120% 0, rgba(59, 130, 246, 0.18), transparent 55%);
      mix-blend-mode: screen;
      opacity: 0.9;
      pointer-events: none;
    }

    .glass-inner {
      position: relative;
      z-index: 1;
    }

    .glass-header {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      margin-bottom: 4px;
    }

    .glass-title {
      font-size: 0.98rem;
      color: #e5e7eb;
      font-weight: 600;
    }

    .glass-badge {
      font-size: 0.7rem;
      padding: 3px 9px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.9);
      border: 1px solid rgba(148, 163, 184, 0.7);
      color: #a5b4fc;
    }

    .glass-desc {
      font-size: 0.8rem;
      color: #cbd5f5;
      margin-bottom: 12px;
    }

    .hero-metrics {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 8px;
      margin-bottom: 9px;
    }

    .metric {
      background: radial-gradient(circle at -10% -20%, rgba(34, 197, 94, 0.25), transparent 50%) rgba(15, 23, 42, 0.96);
      border-radius: 14px;
      padding: 7px 9px;
      border: 1px solid rgba(148, 163, 184, 0.7);
    }

    .metric-label {
      display: block;
      font-size: 0.7rem;
      color: #9ca3af;
      margin-bottom: 2px;
    }

    .metric-value {
      font-size: 0.96rem;
      font-weight: 600;
      color: #e5e7eb;
    }

    .metric-value-bad {
      color: var(--color-danger);
    }

    .glass-footer {
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-top: 1px dashed rgba(148, 163, 184, 0.6);
      padding-top: 6px;
      margin-top: 4px;
    }

    .hero-note {
      font-size: 0.76rem;
      color: #9ca3af;
      max-width: 210px;
    }

    .glass-chip-row {
      display: flex;
      gap: 6px;
      flex-wrap: wrap;
    }

    .glass-chip {
      font-size: 0.7rem;
      padding: 3px 8px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.98);
      border: 1px solid rgba(148, 163, 184, 0.6);
      color: #cbd5f5;
    }

    /* Reusable layout */

    .section-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.15fr) minmax(0, 1fr);
      gap: 34px;
      align-items: flex-start;
    }

    .section h2 {
      margin-top: 10px;
    }

    .body-muted {
      color: var(--color-text-muted);
      font-size: 0.95rem;
    }

    /* Stat & feature cards */

    .stats-cards {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 12px;
      margin-top: 12px;
    }

    .stat-card {
      background: radial-gradient(circle at -10% 0, rgba(34, 197, 94, 0.28), transparent 55%) rgba(15, 23, 42, 0.94);
      color: #e5e7eb;
      padding: 12px 10px;
      border-radius: 16px;
      border: 1px solid rgba(148, 163, 184, 0.65);
      box-shadow: 0 14px 32px rgba(15, 23, 42, 0.7);
    }

    .stat-value {
      display: block;
      font-size: 1.12rem;
      font-weight: 600;
      margin-bottom: 4px;
      color: #bbf7d0;
    }

    .stat-label {
      font-size: 0.78rem;
      color: #cbd5f5;
    }

    .feature-card {
      background: radial-gradient(circle at 0 0, rgba(56, 189, 248, 0.12), transparent 50%) rgba(15, 23, 42, 0.96);
      padding: 18px 18px 16px;
      border-radius: var(--radius-lg);
      border: 1px solid rgba(148, 163, 184, 0.6);
      box-shadow: 0 18px 40px rgba(15, 23, 42, 0.8);
      font-size: 0.9rem;
    }

    .feature-card h3 {
      font-size: 1rem;
      margin-bottom: 6px;
      color: #e5e7eb;
    }

    .number-list {
      padding-left: 20px;
      font-size: 0.9rem;
      color: var(--color-text-muted);
    }

    /* Checklist */

    .checklist {
      list-style: none;
      padding-left: 0;
    }

    .checklist li {
      position: relative;
      padding-left: 20px;
      margin-bottom: 4px;
      font-size: 0.9rem;
    }

    .checklist li::before {
      content: "✔";
      position: absolute;
      left: 0;
      top: 0;
      font-size: 0.8rem;
      color: var(--color-accent);
    }

    /* Modules */

    .module-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 20px;
      margin-top: 24px;
    }

    .module-card {
      background: radial-gradient(circle at 0 0, rgba(34, 197, 94, 0.14), transparent 55%) rgba(15, 23, 42, 0.96);
      border-radius: var(--radius-lg);
      border: 1px solid rgba(148, 163, 184, 0.55);
      padding: 18px 16px 16px;
      box-shadow: 0 18px 38px rgba(15, 23, 42, 0.85);
      font-size: 0.9rem;
      position: relative;
      overflow: hidden;
    }

    .module-card::after {
      content: "";
      position: absolute;
      inset: 0;
      border-radius: inherit;
      border: 1px solid transparent;
      background: linear-gradient(135deg, rgba(148, 163, 184, 0.6), transparent 55%) border-box;
      mask:
        linear-gradient(#000 0 0) padding-box,
        linear-gradient(#000 0 0);
      mask-composite: exclude;
      opacity: 0.35;
      pointer-events: none;
    }

    .module-card h3 {
      font-size: 1.02rem;
      margin-bottom: 6px;
    }

    .module-card p {
      font-size: 0.88rem;
      color: var(--color-text-muted);
    }

    .module-list {
      font-size: 0.86rem;
      margin-top: 6px;
      color: var(--color-text-muted);
    }

    .module-meta {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-top: 10px;
      font-size: 0.8rem;
      color: var(--color-text-muted);
    }

    .module-meta .tag {
      border-color: rgba(74, 222, 128, 0.8);
      background: rgba(22, 163, 74, 0.16);
    }

    /* Plans */

    .plans-grid {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      gap: 18px;
      margin-top: 24px;
    }

    .plan-card {
      background: radial-gradient(circle at 0 0, rgba(34, 197, 94, 0.18), transparent 50%) rgba(15, 23, 42, 0.96);
      border-radius: var(--radius-xl);
      border: 1px solid rgba(148, 163, 184, 0.6);
      padding: 18px 16px 16px;
      box-shadow: 0 18px 40px rgba(15, 23, 42, 0.9);
      display: flex;
      flex-direction: column;
      font-size: 0.88rem;
      position: relative;
      overflow: hidden;
      transform-origin: center;
      transition: transform 0.18s ease, box-shadow 0.18s ease, border-color 0.18s ease;
    }

    .plan-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 26px 56px rgba(15, 23, 42, 0.98);
      border-color: rgba(74, 222, 128, 0.9);
    }

    .plan-card-featured {
      border-color: rgba(34, 197, 94, 0.9);
      box-shadow: 0 28px 70px rgba(22, 163, 74, 0.9);
      transform: translateY(-6px);
      background:
        radial-gradient(circle at 0 0, rgba(34, 197, 94, 0.32), transparent 48%),
        radial-gradient(circle at 120% 0, rgba(56, 189, 248, 0.22), transparent 55%),
        rgba(15, 23, 42, 0.98);
    }

    .plan-label {
      position: absolute;
      top: 10px;
      right: -38px;
      background: linear-gradient(135deg, #22c55e, #16a34a);
      color: #ecfeff;
      font-size: 0.7rem;
      padding: 3px 44px;
      text-align: center;
      transform: rotate(32deg);
      box-shadow: 0 8px 22px rgba(22, 163, 74, 0.8);
    }

    .plan-card h3 {
      font-size: 1rem;
      margin-bottom: 4px;
    }

    .plan-target {
      font-size: 0.82rem;
      color: var(--color-text-muted);
      margin-bottom: 8px;
    }

    .plan-list {
      font-size: 0.84rem;
      margin-top: 4px;
      flex: 1;
      color: var(--color-text-muted);
    }

    .plan-footer {
      margin-top: 10px;
      font-size: 0.8rem;
      color: var(--color-text-muted);
    }

    .plan-type {
      display: block;
      margin-bottom: 6px;
    }

    /* Three-column simple cards */

    .cards-3 {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 18px;
      margin-top: 22px;
    }

    .simple-card {
      background: radial-gradient(circle at 0 0, rgba(59, 130, 246, 0.18), transparent 55%) rgba(15, 23, 42, 0.96);
      border-radius: var(--radius-lg);
      border: 1px solid rgba(148, 163, 184, 0.55);
      padding: 14px 14px 13px;
      box-shadow: 0 18px 38px rgba(15, 23, 42, 0.9);
      font-size: 0.88rem;
    }

    .simple-card h3 {
      font-size: 0.98rem;
    }

    .case-number {
      font-size: 0.78rem;
      color: var(--color-text-muted);
      margin-bottom: 3px;
    }

    /* FAQ */

    .faq-item {
      border-radius: var(--radius-lg);
      border: 1px solid rgba(148, 163, 184, 0.6);
      padding: 10px 12px;
      margin-bottom: 8px;
      background: rgba(15, 23, 42, 0.96);
      font-size: 0.88rem;
      box-shadow: 0 16px 34px rgba(15, 23, 42, 0.9);
    }

    .faq-q {
      font-weight: 600;
      margin-bottom: 4px;
    }

    .faq-a {
      color: var(--color-text-muted);
      font-size: 0.86rem;
    }

    /* CTA */

    .cta-section {
      background:
        radial-gradient(circle at 0 0, rgba(34, 197, 94, 0.32), transparent 50%),
        radial-gradient(circle at 120% 0, rgba(56, 189, 248, 0.26), transparent 58%),
        #020617;
    }

    .cta-container {
      display: grid;
      grid-template-columns: minmax(0, 1.15fr) minmax(0, 1.1fr);
      gap: 28px;
      align-items: flex-start;
    }

    .cta-section h2 {
      color: #f9fafb;
    }

    .cta-section p {
      color: #cbd5f5;
      font-size: 0.95rem;
    }

    .cta-highlight {
      margin-top: 12px;
      padding: 9px 11px;
      border-radius: 14px;
      background: rgba(15, 23, 42, 0.86);
      border: 1px solid rgba(148, 163, 184, 0.7);
      font-size: 0.86rem;
      color: #e5e7eb;
    }

    .cta-form {
      background: radial-gradient(circle at 0 0, rgba(15, 23, 42, 0.9), rgba(15, 23, 42, 0.98));
      border-radius: 24px;
      padding: 18px 16px 16px;
      border: 1px solid rgba(148, 163, 184, 0.7);
      box-shadow: 0 30px 80px rgba(15, 23, 42, 1);
      position: relative;
      overflow: hidden;
    }

    .cta-form::before {
      content: "";
      position: absolute;
      inset: 0;
      background: radial-gradient(circle at 0 0, rgba(34, 197, 94, 0.24), transparent 55%);
      mix-blend-mode: screen;
      opacity: 0.95;
      pointer-events: none;
    }

    .cta-form-inner {
      position: relative;
      z-index: 1;
    }

    .form-row {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
      margin-bottom: 10px;
    }

    .cta-form input,
    .cta-form textarea {
      width: 100%;
      border-radius: 12px;
      border: 1px solid rgba(148, 163, 184, 0.8);
      background: rgba(15, 23, 42, 0.92);
      padding: 9px 10px;
      font-size: 0.85rem;
      color: #e5e7eb;
      outline: none;
    }

    .cta-form input::placeholder,
    .cta-form textarea::placeholder {
      color: #6b7280;
    }

    .cta-form input:focus,
    .cta-form textarea:focus {
      border-color: var(--color-accent);
      box-shadow: 0 0 0 1px rgba(34, 197, 94, 0.8);
      background: rgba(15, 23, 42, 1);
    }

    .cta-form textarea {
      margin-bottom: 10px;
      resize: vertical;
      min-height: 90px;
    }

    /* AIPO Intro card */

    .intro-card {
      margin-top: 18px;
      background: rgba(15, 23, 42, 0.96);
      border-radius: var(--radius-lg);
      border: 1px solid rgba(148, 163, 184, 0.6);
      padding: 16px 16px 14px;
      box-shadow: 0 18px 40px rgba(15, 23, 42, 1);
      font-size: 0.9rem;
    }

    .intro-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.25fr) minmax(0, 0.9fr);
      gap: 22px;
      align-items: flex-start;
    }

    .intro-side {
      border-left: 1px dashed rgba(148, 163, 184, 0.6);
      padding-left: 12px;
      font-size: 0.86rem;
      color: var(--color-text-muted);
    }

    /* Footer */

    .site-footer {
      background: #020617;
      color: #9ca3af;
      padding: 40px 0 20px;
      font-size: 0.84rem;
      border-top: 1px solid rgba(148, 163, 184, 0.5);
    }

    .footer-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.4fr) repeat(3, minmax(0, 1fr));
      gap: 20px;
      margin-bottom: 18px;
      align-items: flex-start;
    }

    .footer-logo .logo-text {
      font-size: 1.05rem;
    }

    .footer-text {
      margin-top: 6px;
      color: #9ca3af;
      max-width: 420px;
      font-size: 0.86rem;
    }

    .footer-col h4 {
      margin-bottom: 6px;
      color: #e5e7eb;
      font-size: 0.9rem;
    }

    .footer-col a {
      display: block;
      color: #9ca3af;
      margin-bottom: 4px;
      font-size: 0.84rem;
    }

    .footer-col a:hover {
      color: #e5e7eb;
    }

    .footer-bottom {
      border-top: 1px solid rgba(148, 163, 184, 0.5);
      padding-top: 10px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 0.8rem;
      color: #6b7280;
      flex-wrap: wrap;
      gap: 6px;
    }

    /* Responsive */

    @media (max-width: 1040px) {
      .hero-grid,
      .section-grid,
      .cta-container,
      .intro-grid,
      .footer-grid {
        grid-template-columns: minmax(0, 1fr);
      }
      .hero-visual {
        justify-content: flex-start;
        margin-top: 18px;
      }
      .plans-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
      .module-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
      .cards-3 {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
    }

    @media (max-width: 840px) {
      .main-nav {
        display: none;
      }
      .hero-inner {
        padding: 22px 18px 20px;
      }
      .section {
        padding: 60px 0;
      }
      .section-alt {
        padding: 60px 0;
      }
      .stats-cards {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
    }

    @media (max-width: 720px) {
      .plans-grid,
      .module-grid,
      .cards-3 {
        grid-template-columns: minmax(0, 1fr);
      }
      .form-row {
        grid-template-columns: minmax(0, 1fr);
      }
      .hero h1 {
        font-size: 1.8rem;
      }
      .hero-grid {
        gap: 26px;
      }
    }
  </style>
</head>
<body>
<div class="page-shell">

  <!-- Header -->
  <header class="site-header">
    <div class="container nav-container">
      <div class="logo">
        <span class="logo-mark">YF</span>
        <span class="logo-text">AIPO</span>
      </div>
      <nav class="main-nav">
        <a href="#home">首頁</a>
        <a href="#why">Why This Matters</a>
        <a href="#seo-aipo">SEO ＆ AIPO</a>
        <a href="#svc">Search Visibility Cloud</a>
        <a href="#modules">產品模組</a>
        <a href="#plans">服務方案</a>
        <a href="#full-funnel">Full Funnel</a>
        <a href="#cases">成功案例</a>
        <a href="#blog">GEO Blog</a>
        <a href="#faq">FAQ</a>
      </nav>
      <a href="#cta" class="btn btn-outline">免費 AIPO 報告</a>
    </div>
  </header>

  <!-- Hero -->
  <section class="hero" id="home">
    <div class="container hero-inner">
      <div class="hero-grid">
        <div>
          <div class="hero-kicker">
            <span>從 SEO 到 AIPO</span>
            <span>AI 時代，流量之外的品牌決策點</span>
          </div>
          <h1>YouFind AIPO｜AI 搜尋時代的 Search Visibility Cloud</h1>
          <p>
            近半數的谷歌搜索已顯示 AI 摘要。你的網站排名靠前，但 AI 卻推薦對手。掌握 AIPO 數據，在消費者決策的「零關鍵時刻」鎖定勝局。
          </p>
          <div class="hero-cta">
            <a href="#cta" class="btn btn-primary">免費 AIPO 報告</a>
            <a href="#aipo-intro" class="btn btn-light">了解 AIPO 介紹</a>
          </div>
          <p class="hero-sub">
            免費掃描你的品牌在 Google AI Overview、ChatGPT、Perplexity、Bing Copilot 中的能見度。
          </p>
          <ul class="hero-bullets">
            <li>從 SEO 排名到 AI 推薦，完整掌握 Search + AI Decision 引擎化。</li>
            <li>結合 ZMOT 與 UMOT 的 Search Strategy，精準捕捉決策瞬間。</li>
            <li>一份報告，同時覆蓋 Query Strategy、AI Overview、Competitor Gap。</li>
          </ul>
        </div>

        <div class="hero-visual">
          <div class="glass-card">
            <div class="glass-inner">
              <div class="glass-header">
                <div class="glass-title">AIPO Search Visibility Snapshot（示意）</div>
                <div class="glass-badge">7–10 Days</div>
              </div>
              <div class="glass-desc">
                一次性 AI 搜尋戰力體檢：AI Overview × SEO × Query Strategy × Competitor Gap。
              </div>
              <div class="hero-metrics">
                <div class="metric">
                  <span class="metric-label">AI Visibility Score</span>
                  <span class="metric-value">76 / 100</span>
                </div>
                <div class="metric">
                  <span class="metric-label">AI Query Coverage</span>
                  <span class="metric-value">58%</span>
                </div>
                <div class="metric">
                  <span class="metric-label">競品 AI 差距告警</span>
                  <span class="metric-value metric-value-bad">5</span>
                </div>
                <div class="metric">
                  <span class="metric-label">Schema 健康度</span>
                  <span class="metric-value">B+ 級</span>
                </div>
              </div>
              <div class="glass-footer">
                <div class="hero-note">
                  支援：Google Search／AI Overview、ChatGPT／GPT Search、Perplexity、Bing Copilot 等主流 AI 平台。
                </div>
                <div class="glass-chip-row">
                  <span class="glass-chip">ZMOT</span>
                  <span class="glass-chip">UMOT</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Section 1：Why This Matters -->
  <section class="section" id="why">
    <div class="container section-grid">
      <div>
        <span class="tag">Section 1：Why This Matters</span>
        <h2>AI 不是取代搜尋，而是重寫搜尋</h2>
        <p class="body-muted">世界頂尖研究機構（Gartner、BrightEdge、Sistrix）指出：</p>
        <p><strong>🔹 Search → Search + AI Decision 引擎化</strong></p>
        <ul class="body-muted">
          <li>62% 用戶會在 AI 平台（ChatGPT、Gemini、Perplexity）先做研究。</li>
          <li>18–70% Query 已觸發 Google AI Overview（AIO）。</li>
          <li>2028 前自然搜尋流量可能下降 30–50%。</li>
        </ul>
        <p><strong>🔹 但 SEO 仍佔網站流量 50%＋（BrightEdge 2024）</strong></p>
        <p class="body-muted">AI 不會毀掉 SEO，它重寫 SEO → AIPO（AI Platform Optimization）。</p>
        <p><strong>🔹 你的品牌需要出現在 4 個引擎：</strong></p>
        <ol class="number-list">
          <li>Google Search（可點擊，導向你的平台介紹頁）。</li>
          <li>Google AI Overview（AIO）－ 旁邊可嵌入示意影片。</li>
          <li>ChatGPT / GPT Search。</li>
          <li>Perplexity / Bing Copilot。</li>
        </ol>
        <p class="body-muted">→ 你若缺其中任何一個，就被競爭對手攔截流量。</p>
      </div>
      <div>
        <div class="stats-cards">
          <div class="stat-card">
            <span class="stat-value">62%</span>
            <span class="stat-label">用戶先在 AI 平台做研究</span>
          </div>
          <div class="stat-card">
            <span class="stat-value">18–70%</span>
            <span class="stat-label">查詢已觸發 Google AIO</span>
          </div>
          <div class="stat-card">
            <span class="stat-value">50%＋</span>
            <span class="stat-label">網站流量仍來自 SEO</span>
          </div>
        </div>
        <div class="feature-card" style="margin-top:16px;">
          <h3>Illustration：Search → AI Platforms</h3>
          <p>示意圖：左側為傳統 Google 搜尋結果頁，右側為 ChatGPT、Perplexity、Bing Copilot 的回答畫面，顯示某品牌在 AI 回答裡「完全沒有被提及」。</p>
          <p>文字說明：搜尋讓你曝光，AI 讓你成交。</p>
          <p>影片示意：可嵌入 Canva Demo Video（Google AIO 與 AI 平台的對照動態演示）。</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Section 2：SEO 與 AIPO 的新關係 -->
  <section class="section-alt" id="seo-aipo">
    <div class="container section-grid">
      <div>
        <span class="tag">Section 2：SEO 與 AIPO 的新關係</span>
        <h2>SEO 是內容存在的基礎，AIPO 是 AI 推薦的結果</h2>
        <p><strong>沒有 SEO，就沒有可被 AI 引用的素材。</strong></p>
        <p class="body-muted">AI 回答需要「可引用的可信來源」，而這些來源來自你的 SEO 基礎：</p>
        <ul class="body-muted">
          <li>FAQ、Schema 與實際數據。</li>
          <li>Chart、表格與可解釋的內容結構。</li>
          <li>Topic Cluster 與高權威反向連結。</li>
        </ul>
        <p><strong>但只有 AIPO，才能讓 AI「引用你」「推薦你」「比對你」。</strong></p>
        <p class="body-muted">SEO ＝ 讓你在搜尋被看到；AIPO ＝ 讓你在 AI 被選擇。</p>
      </div>
      <div class="feature-card">
        <h3>認知盲區：你以為 SEO 成功，其實 AI 推薦的是競爭對手</h3>
        <p>即使網站在傳統搜索結果中名列前茅，當用戶轉向 Google AI Overview 或 Perplexity 等平台進行開放式提問時，AI 系統很可能推薦競爭對手資訊。</p>
        <p>當客戶向 AI 提問而非搜索特定品牌時，若未能獲得 AI 推薦，品牌將徹底流失該客戶，讓你的 SEO 投資替競爭對手鋪路。</p>
        <p>示例：CityU 商學院在「mba hk」自然搜尋排第 2，但在 Perplexity 問「What is the best business school in hk?」時，AI 只列出 HKUST、HKU、CUHK、HKBU、PolyU，CityU 完全「隱形」。</p>
      </div>
    </div>
  </section>

  <!-- Section 3：Search Visibility Cloud -->
  <section class="section" id="svc">
    <div class="container">
      <span class="tag">Section 3：Search Visibility Cloud</span>
      <h2>YouFind 的獨家定位｜Search Visibility Cloud（搜尋能見度雲）</h2>
      <p class="body-muted">香港的 SEO Agency 很多，但能做 AI Search Visibility 的，只有 YouFind。</p>

      <div class="feature-card" style="margin-top:16px;">
        <h3>為何只有 YouFind 能做到 AI Search Visibility？</h3>
        <ul class="body-muted">
          <li><strong>20 年 SEO 數據庫</strong>：全香港最多產業 × 最深的 Search Data Assets。</li>
          <li><strong>20 年外部平台網絡（Third-party Placement Network）</strong>：AI 喜歡引用可信網站，而我們擁有最多可被引用的第三方資源。</li>
          <li><strong>AIPO 專有技術（AIPO Score™、Query Engine）</strong>：不是純人力代工，而是產品化、可擴展的技術能力。</li>
        </ul>
        <p class="body-muted">YouFind 不是一間 SEO 公司，我們是一間 AI Search Intelligence 公司 —— 香港唯一 AI 搜尋能見度專家。</p>
        <p class="body-muted">插圖位置：Search Visibility Cloud 圖像（將 SEO、AIPO、UMOT、Full Funnel Growth 串連的架構圖）。</p>
      </div>
    </div>
  </section>

  <!-- Section 4：Modules -->
  <section class="section-alt" id="modules">
    <div class="container">
      <span class="tag">Section 4：產品模組（Modules）</span>
      <h2>YouFind AIPO™ 服務 — Search Visibility Cloud 4 大模組</h2>
      <p class="body-muted">4 大模組可獨立採用，也可組合成企業級 Search Visibility Cloud，搭配透明定價與 SaaS 級體驗。</p>

      <div class="module-grid">
        <!-- 模組 1 -->
        <article class="module-card">
          <h3>模組 1｜AI Visibility Scanner（AI 能見度掃描）</h3>
          <p>第一步：讓你知道 AI 到底如何看待你。</p>
          <p class="body-muted"><strong>支援平台：</strong>Google AI Overview、ChatGPT、Perplexity、Bing Copilot 等。</p>
          <p class="body-muted"><strong>產出：</strong></p>
          <ul class="module-list">
            <li>你的品牌 AI 引用次數與出現位置。</li>
            <li>AIO Query 覆蓋度與關鍵缺口。</li>
            <li>競爭對手 AI 能見度差距。</li>
            <li>AI 回答來源（Source Attribution）。</li>
            <li>Risk Detection：錯誤資訊與負評引用偵測。</li>
          </ul>
          <div class="module-meta">
            <span class="tag">SaaS 掃描模組</span>
            <span>適合：想快速盤點 AI 風險的品牌</span>
          </div>
        </article>

        <!-- 模組 2 -->
        <article class="module-card">
          <h3>模組 2｜AIPO Content Factory（AI 可引用內容工廠）</h3>
          <p>你的內容不再只是 SEO Friendly，而是 AI Ready ＋ AI Preferred。</p>
          <p class="body-muted">由深圳團隊 + AI 自動生成工具運作，將關鍵 Query 轉化為 AI 最愛引用的內容格式。</p>
          <p class="body-muted"><strong>產出：</strong></p>
          <ul class="module-list">
            <li>FAQ（AI 引用率最高格式）。</li>
            <li>Comparison Pages（品牌／方案比較頁）。</li>
            <li>Data Pages（Chart、數據摘要、表格）。</li>
            <li>Topic Cluster（10×3 Query Model）。</li>
            <li>全套 Schema（FAQPage／QAPage／Article／Product）。</li>
            <li>AIO-Friendly Content Structure（AI 摘要格式）。</li>
          </ul>
          <div class="module-meta">
            <span class="tag">SaaS ＋ 內容服務</span>
            <span>適合：內容／品牌／產品團隊</span>
          </div>
        </article>

        <!-- 模組 3 -->
        <article class="module-card">
          <h3>模組 3｜AIPO Score™（AI 能見度評分）</h3>
          <p>全球首創「AI 能見度分數」：用一個分數看清你在 AI 搜尋世界中的位置。</p>
          <p class="body-muted"><strong>分數來源：</strong></p>
          <ul class="module-list">
            <li>AI 引用率（%）。</li>
            <li>AIO 出現機會（%）。</li>
            <li>Query Coverage（查詢覆蓋度）。</li>
            <li>Schema 健康度與錯誤狀況。</li>
            <li>競爭對手比較與行業 Benchmark（百分位）。</li>
          </ul>
          <p class="body-muted">可視化地圖讓你知道：在哪裡贏、在哪裡輸、下一步如何提升。</p>
          <div class="module-meta">
            <span class="tag">SaaS 指標模組</span>
            <span>適合：管理層／地區總部</span>
          </div>
        </article>

        <!-- 模組 4 -->
        <article class="module-card">
          <h3>模組 4｜UMOT™（Ultimate Moment of Truth）</h3>
          <p>涵蓋「聲譽 × 內容 × AI 決策」一體化循環，解決的是：AI 為什麼要推薦你，而不是對手？</p>
          <p class="body-muted"><strong>流程：</strong></p>
          <ul class="module-list">
            <li>Social Buzz Monitoring。</li>
            <li>Public Concerns Mining（提問情境抽取）。</li>
            <li>Content Angle & Narrative 設計。</li>
            <li>Copywriting（AI ＋ SEO Friendly）。</li>
            <li>多平台佈局（Google Business、Reddit、Quora、Medium、論壇）。</li>
            <li>AI 與 SEO 報告回流，持續優化 Narrative × Signals。</li>
          </ul>
          <div class="module-meta">
            <span class="tag">SaaS ＋ 顧問模組</span>
            <span>適合：金融／醫療／保險／地產／上市公司</span>
          </div>
        </article>
      </div>

      <div class="feature-card" style="margin-top:20px;">
        <h3>重塑「零關鍵時刻」Zero Moment of Truth</h3>
        <p>傳統模式中，品牌透過廣告接觸用戶；如今「零關鍵時刻」（Zero Moment of Truth）已成為潛在客戶的初始接觸點，消費者會先通過各類 AI 平台進行調研才接觸品牌。</p>
        <p>消費者完成購買並使用產品後，在線分享使用體驗與評價則構成「終極關鍵時刻」（Ultimate Moment of Truth），此時用戶已轉化為品牌倡導者，影響下一批新客戶的決策。</p>
        <p>品牌必須在 ZMOT 與 UMOT 上進行戰略性佈局，才能在 AI 驅動的決策時代贏得先機。</p>
        <p>插圖位置：4 大模組與 ZMOT／UMOT 的流程示意圖。</p>
      </div>
    </div>
  </section>

  <!-- Section 5：Plans -->
  <section class="section" id="plans">
    <div class="container">
      <span class="tag">Section 5：服務方案（產品化套裝）</span>
      <h2>4 個產品化方案，升級為 SaaS 級體驗</h2>
      <p class="body-muted">根據不同成熟度與資源配置，YouFind 提供 4 個 AIPO 產品化方案，從 3 個月快速驗證到 Full Funnel 搜尋成長。</p>

      <div class="plans-grid">
        <!-- Plan 1 -->
        <article class="plan-card">
          <h3>Plan 1｜Pure AIPO（3 個月快速驗證）</h3>
          <p class="plan-target">適合：想快速測試 AI 能見度的品牌。</p>
          <p><strong>Deliverables：</strong></p>
          <ul class="plan-list">
            <li>AIO Audit：一次性 AI 搜尋體檢。</li>
            <li>10–20 條高 Intent FAQ 制定。</li>
            <li>技術修復（AI Crawlability）。</li>
            <li>Schema 套件部署（FAQPage／QAPage／Article／Product 基礎）。</li>
            <li>AIO Tracking 30 天：核心 Query 的 AI 能見度追蹤。</li>
          </ul>
          <div class="plan-footer">
            <span class="plan-type">SaaS ＋ 專家工作坊簡報</span>
            <a href="#cta" class="btn btn-primary btn-full">索取 Pure AIPO 範本報告</a>
          </div>
        </article>

        <!-- Plan 2 -->
        <article class="plan-card">
          <h3>Plan 2｜On‑Going AIPO（6–12 個月）</h3>
          <p class="plan-target">適合：需要穩定 AIO 增長與持續優化的品牌。</p>
          <p><strong>Deliverables（示意）：</strong></p>
          <ul class="plan-list">
            <li>每月新增 FAQ 20–40 條，涵蓋核心與長尾 Query。</li>
            <li>每月 Query Group 擴展與優先級調整。</li>
            <li>AIO Recommendation Tracking（每週）：追蹤 AI 推薦變化。</li>
            <li>內容優化迭代（Content Refresh + Angle 調整）。</li>
            <li>Schema 維護與錯誤修正。</li>
            <li>季度 Benchmark Report：與競品／行業指標比對。</li>
          </ul>
          <div class="plan-footer">
            <span class="plan-type">SaaS ＋ 內容與技術顧問團隊</span>
            <a href="#cta" class="btn btn-primary btn-full">安排 On‑Going AIPO 諮詢</a>
          </div>
        </article>

        <!-- Plan 3 -->
        <article class="plan-card plan-card-featured">
          <div class="plan-label">最推薦</div>
          <h3>Plan 3｜SEO + AIPO（Search AI 雙軌增長）</h3>
          <p class="plan-target">適合：需要 Search + AI 雙重增長的成長型品牌。</p>
          <p><strong>Deliverables：</strong></p>
          <ul class="plan-list">
            <li>Full SEO：網站結構、內容、技術健康度全面優化。</li>
            <li>Full AIPO：整合 AI Visibility Scanner、Content Factory、AIPO Score™。</li>
            <li>Topic Cluster（10×3）：以 Query Group 為核心的內容集群佈局。</li>
            <li>Content Refresh：既有內容的 AI 化與 SEO 更新策略。</li>
            <li>Ranking Growth ＋ AI Visibility Growth 雙軌 KPI 管理。</li>
          </ul>
          <div class="plan-footer">
            <span class="plan-type">一站式 Search AI 增長方案</span>
            <a href="#cta" class="btn btn-primary btn-full">索取 SEO + AIPO 詳細方案</a>
          </div>
        </article>

        <!-- Plan 4 -->
        <article class="plan-card">
          <h3>Plan 4｜SEO + AIPO + UMOT（旗艦級）</h3>
          <p class="plan-target">適合：金融｜醫療｜保險｜地產｜上市公司等高聲譽要求的領先品牌。</p>
          <p><strong>Deliverables：</strong></p>
          <ul class="plan-list">
            <li>Full Funnel Search Visibility：從搜尋到 UMOT 的全旅程佈局。</li>
            <li>高階 Narrative Management：管理關鍵議題與品牌敘事。</li>
            <li>Reputation & Trust Signals：第三方平台口碑與信任訊號設計。</li>
            <li>Third‑party Signal Distribution：Google Business、Reddit、Quora、Medium、論壇等渠道佈署。</li>
            <li>企業級 CXO 搜尋戰略簡報。</li>
            <li>AI × SEO × Reputation 全套護城河設計。</li>
          </ul>
          <div class="plan-footer">
            <span class="plan-type">策略顧問 ＋ 平台 ＋ 執行落地</span>
            <a href="#cta" class="btn btn-primary btn-full">預約 CXO Briefing</a>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!-- Section 6：Full Funnel -->
  <section class="section-alt" id="full-funnel">
    <div class="container section-grid">
      <div>
        <span class="tag">Section 6：Full Funnel Growth（同一預算，更多線索）</span>
        <h2>Full Funnel＝Paid Media × SEO × AIPO × UMOT × AI 優化</h2>
        <p class="body-muted">傳統做法：買流量。新做法：買增長。</p>
        <p class="body-muted">YouFind Promise：在同一預算下，為你帶來可被驗證的 YoY 線索與收入增長。</p>
        <p><strong>流程：</strong></p>
        <ul class="checklist">
          <li>Google／Meta Ads：短期轉換與高 Intent 導流。</li>
          <li>SEO：中期累積穩定、低成本自然流量。</li>
          <li>AIPO：在 AI 賦能的決策點提升曝光與推薦機率。</li>
          <li>UMOT：透過聲譽與敘事信號提升轉化率與信任度。</li>
          <li>Optimization：動態調整關鍵字 × Query × 投放策略。</li>
        </ul>
        <p class="body-muted">→ 形成耐用、疊加、可複製的線索引擎。</p>
      </div>
      <div class="feature-card">
        <h3>Full Funnel Growth Illustrations</h3>
        <p>可於此放置 Full Funnel Growth 圖像，展示從 Awareness → Consideration → Decision → UMOT 的完整旅程，以及 SEO、AIPO、Paid Media、UMOT 在每個階段的角色。</p>
        <p>同時可示意 KPI 例子：曝光 Coverage%、AI Recommendation 出現率、Leads、Revenue YoY Growth 等。</p>
      </div>
    </div>
  </section>

  <!-- Section 8：CTA -->
  <section class="section cta-section" id="cta">
    <div class="container cta-container">
      <div>
        <span class="tag">Section 8：CTA（最強轉換）</span>
        <h2>立即領取《AI 搜尋戰力體檢》</h2>
        <p>AI Overview × SEO 技術 × Query Strategy × Competitor Gap，7–10 日內為你輸出一份專屬報告。</p>
        <p>這是 SEO、AIPO、UMOT 三條產品線的共同入口，適用於：行銷主管、數碼營銷經理、CXO、品牌與公關團隊。</p>
        <p>留下聯絡資料，我們會與你確認 7–10 組優先查詢，並安排 30 分鐘說明會。</p>
        <div class="cta-highlight">
          「你現在的 SEO 成效，正在替誰鋪路？」讓這份報告告訴你，AI 決策世界裡，真正被推薦的是誰。
        </div>
      </div>
      <form class="cta-form">
        <div class="cta-form-inner">
          <div class="form-row">
            <input type="text" placeholder="公司名稱 Company" />
            <input type="text" placeholder="姓名 Name" />
          </div>
          <div class="form-row">
            <input type="email" placeholder="公司電郵 Business Email" />
            <input type="text" placeholder="電話 / WhatsApp" />
          </div>
          <textarea placeholder="請簡單描述你的行業、目標市場與目前 SEO／AI 搜尋情況，以及你最關心的 3 個決策問題。"></textarea>
          <button type="submit" class="btn btn-primary btn-full">提交並領取《AI 搜尋戰力體檢》</button>
        </div>
      </form>
    </div>
  </section>

  <!-- Section 9：Cases -->
  <section class="section" id="cases">
    <div class="container">
      <span class="tag">Section 9：客戶成功案例</span>
      <h2>成功案例｜Search Visibility Cloud 實戰成果</h2>
      <p class="body-muted">以實際數據說話，從曝光 Coverage% 到 AI Recommendation 率，讓你清楚看到 AIPO 帶來的增長。</p>

      <div class="cards-3">
        <article class="simple-card">
          <div class="case-number">Case 01｜教育行業（MBA）</div>
          <h3>從 SEO Top 3 到 AI 回答主角</h3>
          <p>原本僅在「mba hk」自然搜尋排前列，卻在 AI 問答中完全缺席。透過 AIPO Content Factory 與 AI Visibility Scanner，讓品牌成功被 ChatGPT、Perplexity 納入首輪推薦名單。</p>
          <p>量化指標示例：AI Query Coverage、Brand Mention 次數、對手差距縮小比例等，可於此以圖像方式呈現。</p>
        </article>

        <article class="simple-card">
          <div class="case-number">Case 02｜金融服務</div>
          <h3>從關鍵字爭奪戰，到 AI 信任戰</h3>
          <p>透過 UMOT 模組，重構品牌敘事與第三方信任信號，在高風險關鍵字上減少負面推薦與錯誤資訊，提升 AI 推薦率與轉化率。</p>
        </article>

        <article class="simple-card">
          <div class="case-number">Case 03｜電商與零售</div>
          <h3>以 Topic Cluster 帶動整體銷售</h3>
          <p>透過 10×3 Query Model 與 Comparison Pages，讓 AI 在比較產品與方案時更多提及品牌，帶來高 Intent 流量與訂單成長。</p>
        </article>
      </div>
    </div>
  </section>

  <!-- Section 10：Blog -->
  <section class="section-alt" id="blog">
    <div class="container">
      <span class="tag">Section 10：部落格文章（GEO Blog）</span>
      <h2>GEO Insight Blog｜GEO 關鍵字沿用</h2>
      <p class="body-muted">在部落格區域保留「GEO」作為關鍵字，用於教育市場與 SEO 積累，同時為 AIPO 與 UMOT 導流。</p>

      <div class="cards-3">
        <article class="simple-card">
          <h3>What is GEO？為何 AI 時代比以往更重要？</h3>
          <p>介紹 GEO 的核心概念，解釋 Search Visibility 與 GEO 的關係，以及傳統 SEO 到 GEO／AIPO 的演進。</p>
        </article>
        <article class="simple-card">
          <h3>GEO vs 傳統 SEO：決策點的差異</h3>
          <p>比較單純追求關鍵字排名 vs 以決策 Query 與 AI Recommendation 為核心的 GEO 策略。</p>
        </article>
        <article class="simple-card">
          <h3>GEO in Practice：實戰 Query Strategy 案例</h3>
          <p>分享 7–10 組 Query Group 的實戰設計方法與測試結果，並連結到 AIPO 方案。</p>
        </article>
      </div>
    </div>
  </section>

  <!-- Section 11：FAQ -->
  <section class="section" id="faq">
    <div class="container">
      <span class="tag">Section 11：常見問題</span>
      <h2>常見問題｜FAQ</h2>

      <div class="faq-item">
        <div class="faq-q">Q1：AIPO 與傳統 SEO 有什麼不同？可以只做 AIPO 而不做 SEO 嗎？</div>
        <div class="faq-a">A1：SEO 是內容存在與被搜尋引擎收錄的基礎，AIPO 則專注於讓 AI 在回答中「選擇你」。沒有 SEO，AI 沒有足夠可信素材；沒有 AIPO，這些素材未必會被 AI 優先引用。</div>
      </div>

      <div class="faq-item">
        <div class="faq-q">Q2：多久可以看到 AIPO 帶來的效果？</div>
        <div class="faq-a">A2：Pure AIPO 方案約 3 個月可看到 AI Query Coverage 與 AI Recommendation 的初步變化，On‑Going AIPO 與 SEO + AIPO 通常在 6–12 個月形成穩定成長曲線。</div>
      </div>

      <div class="faq-item">
        <div class="faq-q">Q3：如果我已經有內部 SEO 團隊，還需要 YouFind AIPO 嗎？</div>
        <div class="faq-a">A3：內部 SEO 團隊是重要資產，而 AIPO 聚焦在 AI 搜尋視角、AIPO Score™ 與 UMOT，會與你的內部團隊形成互補，共同擴大投資效益。</div>
      </div>

      <div class="faq-item">
        <div class="faq-q">Q4：AIPO 是否適用於高度監管行業（如金融、醫療）？</div>
        <div class="faq-a">A4：是。Plan 4（SEO + AIPO + UMOT）特別針對金融、醫療、保險、地產與上市公司設計，重視合規、聲譽與敘事風險管理。</div>
      </div>

      <div class="faq-item">
        <div class="faq-q">Q5：如何開始？</div>
        <div class="faq-a">A5：建議由《AI 搜尋戰力體檢》開始，透過 7–10 組 Query Group 快速盤點你的現況，再由顧問團隊共同設計適合的模組與方案。</div>
      </div>
    </div>
  </section>

  <!-- AIPO 介紹 -->
  <section class="section-alt" id="aipo-intro">
    <div class="container">
      <span class="tag">AIPO 介紹</span>
      <h2>您佔領了搜索排名，卻輸掉了 AI 的「決策對話」</h2>
      <div class="intro-card">
        <div class="intro-grid">
          <div>
            <p>您的品牌在搜索引擎上名列前茅，網站流量節節攀升。這曾是數字營銷成功的終極證明。然而，一個無聲的戰場正在客戶決策的最後一英里悄然展開。</p>
            <p>當您的潛在客戶站在決策的十字路口，他們不再只是反覆點擊搜索結果，而是轉向一個更智能、更個人化的「顧問」—— 他們的 AI 助手。</p>
            <p>潛在客戶會問：</p>
            <ul>
              <li>「我應該為 ［某需求］ 選擇哪家品牌？」</li>
              <li>「［您的行業］ 中，哪家公司在創新和客戶服務方面口碑最好？」</li>
              <li>「比較一下 A 品牌和 B 品牌的優缺點。」</li>
            </ul>
            <p><strong>排名領先的假象：</strong>AI 不像傳統搜索引擎那樣簡單地匹配關鍵詞和鏈接，它整合全域資訊，而非單一網頁。若你的品牌在 AI 的「認知」中存在缺陷，AI 推薦的，可能不是你，而是你的競爭對手。</p>
            <p>在這個時候，你便需要 GEO 與 AIPO。當遊戲規則已經改變，你的策略也必須進化。我們的核心使命是：系統性地塑造與管理你的品牌在 AI 認知世界中的形象，確保你在關鍵的決策對話中，成為那個無可爭議的推薦答案。</p>
          </div>
          <div class="intro-side">
            <p><strong>Illustration 建議：</strong></p>
            <p>左邊：Search Page × Brand Top 3。右邊：AI 回答中沒有你，卻有 3–5 間競爭對手。</p>
            <p>可加入一段 Demo Video（例如 Canva 或 Loom）讓客戶看到「AI 決策落差」的實際畫面。</p>
            <p>這亦是 AIPO Sales Deck 中最關鍵的一張「覺醒頁」。</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="site-footer">
    <div class="container footer-grid">
      <div>
        <div class="logo footer-logo">
          <span class="logo-mark">YF</span>
          <span class="logo-text">AIPO</span>
        </div>
        <p class="footer-text">
          YouFind AIPO Search Visibility Cloud｜結合 20 年 SEO 數據庫、Third‑party Placement Network 與專有 AIPO 技術，為品牌打造 AI 搜尋時代的搜尋能見度護城河。
        </p>
      </div>
      <div class="footer-col">
        <h4>Solutions</h4>
        <a href="#modules">AIPO Modules</a>
        <a href="#plans">AIPO Plans</a>
        <a href="#full-funnel">Full Funnel Growth</a>
      </div>
      <div class="footer-col">
        <h4>Company</h4>
        <a href="#cases">成功案例</a>
        <a href="#blog">GEO Blog</a>
        <a href="#faq">常見問題</a>
      </div>
      <div class="footer-col">
        <h4>Contact</h4>
        <a href="#cta">預約諮詢</a>
        <a href="#">LinkedIn</a>
        <a href="#">Facebook</a>
      </div>
    </div>
    <div class="container footer-bottom">
      <span>© YouFind Ltd. All rights reserved.</span>
      <span>Google Certified Partner｜AI Search Intelligence Company</span>
    </div>
  </footer>

</div>
</body>
</html>
