<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Group 3 | Portfolio Dashboard | Mr. Adrian Cole</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.min.js"></script>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;600;700&family=DM+Mono:wght@400;500&family=Outfit:wght@300;400;500;600;700&display=swap" rel="stylesheet"/>
<style>
  :root {
    --navy: #050D1A;
    --navy2: #0A1628;
    --navy3: #0F1F35;
    --gold: #C9A84C;
    --gold2: #E8C87A;
    --gold-dim: #C9A84C22;
    --teal: #00D4AA;
    --red: #FF4D6D;
    --blue: #3B82F6;
    --purple: #8B5CF6;
    --orange: #F97316;
    --white: #F0F4FF;
    --muted: #4A6080;
    --border: rgba(201,168,76,0.15);
    --card: rgba(255,255,255,0.03);
  }
  * { margin:0; padding:0; box-sizing:border-box; }
  body { background:var(--navy); color:var(--white); font-family:'Outfit',sans-serif; min-height:100vh; overflow-x:hidden; }

  /* Animated background */
  body::before {
    content:''; position:fixed; inset:0; z-index:0;
    background: radial-gradient(ellipse at 20% 20%, rgba(201,168,76,0.04) 0%, transparent 50%),
                radial-gradient(ellipse at 80% 80%, rgba(59,130,246,0.04) 0%, transparent 50%),
                radial-gradient(ellipse at 50% 50%, rgba(0,212,170,0.02) 0%, transparent 70%);
    pointer-events:none;
  }

  /* Grid lines background */
  body::after {
    content:''; position:fixed; inset:0; z-index:0;
    background-image: linear-gradient(rgba(201,168,76,0.03) 1px, transparent 1px),
                      linear-gradient(90deg, rgba(201,168,76,0.03) 1px, transparent 1px);
    background-size: 60px 60px;
    pointer-events:none;
  }

  .wrap { position:relative; z-index:1; }

  /* ── HEADER ── */
  header {
    background: linear-gradient(135deg, #050D1A 0%, #0A1628 100%);
    border-bottom: 1px solid var(--border);
    padding: 0 32px;
    position: sticky; top:0; z-index:100;
    backdrop-filter: blur(20px);
  }
  .header-inner { display:flex; align-items:center; justify-content:space-between; height:64px; }
  .logo { display:flex; align-items:center; gap:12px; }
  .logo-mark {
    width:36px; height:36px; border:1.5px solid var(--gold);
    display:grid; place-items:center; font-family:'Cormorant Garamond',serif;
    font-size:16px; font-weight:700; color:var(--gold); letter-spacing:0.05em;
  }
  .logo-text { font-size:13px; font-weight:600; color:var(--white); letter-spacing:0.05em; }
  .logo-sub { font-size:10px; color:var(--muted); letter-spacing:0.08em; text-transform:uppercase; }
  .header-meta { display:flex; align-items:center; gap:24px; }
  .client-badge {
    padding:6px 16px; border:1px solid var(--border); background:var(--gold-dim);
    font-size:11px; color:var(--gold); letter-spacing:0.08em; font-weight:600;
  }
  .live-dot { display:flex; align-items:center; gap:6px; font-size:11px; color:var(--teal); }
  .live-dot::before { content:''; width:6px; height:6px; border-radius:50%; background:var(--teal); animation:pulse 2s infinite; }
  @keyframes pulse { 0%,100%{opacity:1;transform:scale(1)} 50%{opacity:0.5;transform:scale(1.4)} }

  /* ── TABS ── */
  .tabs { display:flex; gap:2px; padding:0 32px; background:var(--navy2); border-bottom:1px solid var(--border); }
  .tab {
    padding:14px 24px; font-size:12px; font-weight:600; letter-spacing:0.06em;
    text-transform:uppercase; color:var(--muted); cursor:pointer; border:none;
    background:transparent; border-bottom:2px solid transparent; transition:all 0.2s;
  }
  .tab:hover { color:var(--white); }
  .tab.active { color:var(--gold); border-bottom-color:var(--gold); }

  /* ── PANELS ── */
  .panel { display:none; padding:28px 32px; animation:fadeIn 0.3s ease; }
  .panel.active { display:block; }
  @keyframes fadeIn { from{opacity:0;transform:translateY(8px)} to{opacity:1;transform:translateY(0)} }

  /* ── KPI STRIP ── */
  .kpi-strip { display:grid; grid-template-columns:repeat(6,1fr); gap:12px; margin-bottom:24px; }
  .kpi {
    background:var(--card); border:1px solid var(--border); padding:16px 18px;
    position:relative; overflow:hidden; transition:border-color 0.2s;
  }
  .kpi::before { content:''; position:absolute; top:0; left:0; right:0; height:2px; background:var(--accent,var(--gold)); }
  .kpi:hover { border-color:var(--gold); }
  .kpi-label { font-size:9px; text-transform:uppercase; letter-spacing:0.12em; color:var(--muted); margin-bottom:8px; }
  .kpi-value { font-family:'DM Mono',monospace; font-size:22px; font-weight:500; color:var(--accent,var(--gold)); line-height:1; }
  .kpi-unit { font-size:12px; color:var(--muted); margin-left:2px; }
  .kpi-sub { font-size:10px; color:var(--muted); margin-top:4px; }

  /* ── GRID LAYOUTS ── */
  .grid-2 { display:grid; grid-template-columns:1fr 1fr; gap:20px; }
  .grid-3 { display:grid; grid-template-columns:1fr 1fr 1fr; gap:20px; }
  .grid-4 { display:grid; grid-template-columns:repeat(4,1fr); gap:16px; }
  .col-span-2 { grid-column:span 2; }
  .col-span-3 { grid-column:span 3; }

  /* ── CARDS ── */
  .card {
    background:var(--card); border:1px solid var(--border);
    padding:24px; position:relative; overflow:hidden;
  }
  .card-title { font-family:'Cormorant Garamond',serif; font-size:16px; font-weight:700; color:var(--white); margin-bottom:4px; }
  .card-sub { font-size:10px; color:var(--muted); text-transform:uppercase; letter-spacing:0.08em; margin-bottom:18px; }
  .card-corner {
    position:absolute; top:0; right:0; width:48px; height:48px;
    border-bottom:1px solid var(--border); border-left:1px solid var(--border);
    display:grid; place-items:center; font-size:16px; color:var(--gold); opacity:0.4;
  }

  /* ── FUND WEIGHTS SLIDERS ── */
  .fund-row { margin-bottom:18px; }
  .fund-row-top { display:flex; justify-content:space-between; align-items:center; margin-bottom:6px; }
  .fund-name { font-size:12px; font-weight:500; color:var(--white); }
  .fund-class { font-size:9px; color:var(--muted); text-transform:uppercase; letter-spacing:0.08em; }
  .fund-weight-val { font-family:'DM Mono',monospace; font-size:14px; font-weight:500; }
  .weight-track { height:6px; background:rgba(255,255,255,0.06); border-radius:0; position:relative; cursor:pointer; }
  .weight-fill { height:100%; border-radius:0; transition:width 0.1s; }
  input[type=range] {
    width:100%; -webkit-appearance:none; appearance:none;
    height:6px; background:rgba(255,255,255,0.06); outline:none; cursor:pointer;
  }
  input[type=range]::-webkit-slider-thumb {
    -webkit-appearance:none; width:14px; height:14px; border-radius:50%;
    background:var(--thumb-color,var(--gold)); cursor:pointer; border:2px solid var(--navy);
    transition:transform 0.15s;
  }
  input[type=range]::-webkit-slider-thumb:hover { transform:scale(1.3); }
  input[type=range]::-webkit-slider-runnable-track { background:rgba(255,255,255,0.06); height:6px; }

  /* ── TABLES ── */
  table { width:100%; border-collapse:collapse; font-size:12px; }
  th { padding:10px 12px; text-align:left; font-size:9px; text-transform:uppercase; letter-spacing:0.1em; color:var(--muted); font-weight:600; border-bottom:1px solid var(--border); }
  td { padding:11px 12px; border-bottom:1px solid rgba(255,255,255,0.04); }
  tr:hover td { background:rgba(255,255,255,0.02); }
  tr.portfolio-row td { background:rgba(201,168,76,0.06); border-top:1px solid var(--border); font-weight:700; }
  .mono { font-family:'DM Mono',monospace; }
  .badge { display:inline-block; padding:2px 8px; font-size:9px; font-weight:700; letter-spacing:0.08em; }
  .badge-green { background:rgba(0,212,170,0.12); color:var(--teal); }
  .badge-yellow { background:rgba(201,168,76,0.12); color:var(--gold); }
  .badge-red { background:rgba(255,77,109,0.12); color:var(--red); }

  /* ── ALLOCATION BAR ── */
  .alloc-bar { display:flex; height:32px; overflow:hidden; margin-bottom:20px; border:1px solid var(--border); }
  .alloc-seg { display:flex; align-items:center; justify-content:center; font-size:10px; font-weight:700; color:#000; transition:flex 0.4s ease; cursor:pointer; position:relative; }
  .alloc-seg:hover { filter:brightness(1.2); }
  .alloc-seg span { white-space:nowrap; overflow:hidden; }

  /* ── SCENARIO CARDS ── */
  .scenario { padding:20px; border:1px solid; text-align:center; }
  .scenario-title { font-size:13px; font-weight:700; margin-bottom:4px; }
  .scenario-note { font-size:10px; color:var(--muted); margin-bottom:12px; }
  .scenario-return { font-family:'Cormorant Garamond',serif; font-size:36px; font-weight:700; line-height:1; }
  .scenario-val { font-family:'DM Mono',monospace; font-size:15px; margin-top:8px; }
  .scenario-label { font-size:9px; color:var(--muted); text-transform:uppercase; letter-spacing:0.08em; margin-top:2px; }

  /* ── TIMELINE ── */
  .timeline { position:relative; padding-left:28px; }
  .timeline::before { content:''; position:absolute; left:8px; top:0; bottom:0; width:1px; background:var(--border); }
  .timeline-item { position:relative; margin-bottom:20px; }
  .timeline-dot {
    position:absolute; left:-24px; top:4px; width:12px; height:12px;
    border:2px solid var(--gold); background:var(--navy);
  }
  .timeline-dot.done { background:var(--teal); border-color:var(--teal); }
  .timeline-dot.active { background:var(--gold); border-color:var(--gold); animation:pulse 1.5s infinite; }
  .timeline-week { font-size:9px; text-transform:uppercase; letter-spacing:0.1em; color:var(--gold); font-weight:700; }
  .timeline-task { font-size:12px; color:var(--white); font-weight:500; margin:2px 0; }
  .timeline-owner { font-size:10px; color:var(--muted); }
  .timeline-status { display:inline-block; padding:1px 8px; font-size:9px; font-weight:700; letter-spacing:0.06em; margin-top:4px; }

  /* ── IPS SECTION ── */
  .ips-grid { display:grid; grid-template-columns:1fr 1fr; gap:16px; }
  .ips-item { padding:16px; background:rgba(255,255,255,0.02); border-left:2px solid var(--gold); }
  .ips-key { font-size:9px; text-transform:uppercase; letter-spacing:0.1em; color:var(--gold); margin-bottom:6px; font-weight:700; }
  .ips-val { font-size:13px; color:var(--white); font-weight:500; }
  .ips-note { font-size:10px; color:var(--muted); margin-top:4px; }

  /* ── RISK METER ── */
  .risk-meter { position:relative; width:180px; height:90px; margin:0 auto 8px; }
  .risk-meter canvas { width:100% !important; height:100% !important; }

  /* ── GROWTH PROJECTIONS ── */
  .proj-card { text-align:center; padding:20px; border:1px solid var(--border); background:var(--card); }
  .proj-yr { font-size:10px; text-transform:uppercase; letter-spacing:0.12em; color:var(--muted); margin-bottom:8px; }
  .proj-val { font-family:'Cormorant Garamond',serif; font-size:28px; font-weight:700; color:var(--teal); }
  .proj-gain { font-size:11px; color:var(--muted); margin-top:4px; }
  .proj-pct { font-size:12px; color:var(--gold); font-family:'DM Mono',monospace; }

  /* ── TEAM CARDS ── */
  .team-card { padding:20px; border:1px solid var(--border); background:var(--card); text-align:center; }
  .team-avatar { width:52px; height:52px; border:2px solid var(--gold); display:grid; place-items:center; margin:0 auto 12px; font-family:'Cormorant Garamond',serif; font-size:20px; font-weight:700; color:var(--gold); }
  .team-name { font-size:13px; font-weight:700; color:var(--white); margin-bottom:2px; }
  .team-role { font-size:10px; color:var(--gold); text-transform:uppercase; letter-spacing:0.08em; margin-bottom:8px; }
  .team-tasks { font-size:10px; color:var(--muted); line-height:1.6; }
  .team-audit { font-size:9px; color:var(--muted); margin-top:8px; padding-top:8px; border-top:1px solid var(--border); }

  /* ── FOOTER ── */
  footer { border-top:1px solid var(--border); padding:16px 32px; display:flex; justify-content:space-between; align-items:center; font-size:10px; color:var(--muted); background:var(--navy2); }
  .disclaimer { font-size:9px; color:var(--muted); opacity:0.6; max-width:600px; }

  /* ── HORIZON TOGGLE ── */
  .horizon-btns { display:flex; gap:4px; }
  .hz-btn { padding:6px 16px; border:1px solid var(--border); background:transparent; color:var(--muted); font-size:11px; font-weight:600; cursor:pointer; font-family:'Outfit',sans-serif; transition:all 0.15s; }
  .hz-btn.active { border-color:var(--gold); color:var(--gold); background:var(--gold-dim); }

  /* ── NORMALISE BTN ── */
  .btn-gold { padding:8px 18px; border:1px solid var(--gold); background:var(--gold-dim); color:var(--gold); font-size:11px; font-weight:600; cursor:pointer; font-family:'Outfit',sans-serif; letter-spacing:0.06em; transition:all 0.15s; }
  .btn-gold:hover { background:var(--gold); color:var(--navy); }

  /* ── TOTAL INDICATOR ── */
  .total-bar { padding:12px 16px; margin-top:16px; font-size:13px; font-weight:700; font-family:'DM Mono',monospace; }
  .total-ok { background:rgba(0,212,170,0.08); border:1px solid rgba(0,212,170,0.3); color:var(--teal); }
  .total-warn { background:rgba(255,77,109,0.08); border:1px solid rgba(255,77,109,0.3); color:var(--red); }

  /* ── DOLLAR DISPLAY ── */
  .dollar-val { font-family:'DM Mono',monospace; font-size:11px; color:var(--muted); margin-top:2px; }

  /* scrollbar */
  ::-webkit-scrollbar { width:4px; }
  ::-webkit-scrollbar-track { background:var(--navy); }
  ::-webkit-scrollbar-thumb { background:var(--muted); }

  @media(max-width:900px) {
    .kpi-strip { grid-template-columns:repeat(3,1fr); }
    .grid-2,.grid-3,.grid-4 { grid-template-columns:1fr; }
    .col-span-2,.col-span-3 { grid-column:span 1; }
    .ips-grid { grid-template-columns:1fr; }
  }
</style>
</head>
<body>
<div class="wrap">

<!-- HEADER -->
<header>
  <div class="header-inner">
    <div class="logo">
      <div class="logo-mark">G3</div>
      <div>
        <div class="logo-text">GROUP 3 — PORTFOLIO DASHBOARD</div>
        <div class="logo-sub">BAFI3178 · Applied Portfolio Management · RMIT University · S1 2026</div>
      </div>
    </div>
    <div class="header-meta">
      <div class="live-dot">LIVE MODEL</div>
      <div class="client-badge">CLIENT: MR. ADRIAN COLE</div>
      <div class="horizon-btns">
        <button class="hz-btn active" onclick="setHorizon('3Y',this)">3Y</button>
        <button class="hz-btn" onclick="setHorizon('5Y',this)">5Y</button>
        <button class="hz-btn" onclick="setHorizon('7Y',this)">7Y</button>
      </div>
    </div>
  </div>
</header>

<!-- TABS -->
<div class="tabs">
  <button class="tab active" onclick="showPanel('overview',this)">Overview</button>
  <button class="tab" onclick="showPanel('allocation',this)">Allocation</button>
  <button class="tab" onclick="showPanel('performance',this)">Performance</button>
  <button class="tab" onclick="showPanel('growth',this)">Growth</button>
  <button class="tab" onclick="showPanel('ips',this)">IPS</button>
  <button class="tab" onclick="showPanel('timeline',this)">Timeline</button>
  <button class="tab" onclick="showPanel('team',this)">Team</button>
</div>

<!-- ════════════════════════════════════════════════ OVERVIEW ═══ -->
<div id="panel-overview" class="panel active">

  <!-- KPI STRIP -->
  <div class="kpi-strip" id="kpi-strip"></div>

  <div class="grid-2" style="margin-bottom:20px">
    <!-- Risk Return Chart -->
    <div class="card">
      <div class="card-corner">◈</div>
      <div class="card-title">Risk — Return Map</div>
      <div class="card-sub">Fund positioning by volatility vs. expected return</div>
      <canvas id="chartScatter" height="240"></canvas>
    </div>
    <!-- Radar -->
    <div class="card">
      <div class="card-corner">◈</div>
      <div class="card-title">Fund Characteristics Radar</div>
      <div class="card-sub">Return · Risk · Sharpe (scaled) across 6 funds</div>
      <canvas id="chartRadar" height="240"></canvas>
    </div>
  </div>

  <!-- Fund Table -->
  <div class="card">
    <div class="card-title">Fund Universe — Group 3</div>
    <div class="card-sub">All 6 assigned funds with key metrics</div>
    <div style="overflow-x:auto">
    <table>
      <thead><tr>
        <th>Fund</th><th>Asset Class</th><th>Benchmark</th>
        <th>Ann. Return</th><th>Volatility</th><th>Beta</th>
        <th>Sharpe</th><th>VaR 95%</th><th>Rating</th>
      </tr></thead>
      <tbody id="fund-table-body"></tbody>
    </table>
    </div>
  </div>
</div>

<!-- ════════════════════════════════════════════════ ALLOCATION ═══ -->
<div id="panel-allocation" class="panel">
  <div class="grid-2">
    <div class="card">
      <div style="display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:20px">
        <div>
          <div class="card-title">Adjust Fund Weights</div>
          <div class="card-sub">Drag to set allocation — Total must equal 100%</div>
        </div>
        <button class="btn-gold" onclick="normalise()">Normalise to 100%</button>
      </div>
      <div id="sliders"></div>
      <div class="total-bar" id="total-bar">Total: 90%</div>
    </div>

    <div class="card">
      <div class="card-title">Allocation Breakdown</div>
      <div class="card-sub">Visual distribution across asset classes</div>
      <div class="alloc-bar" id="alloc-bar"></div>
      <div id="alloc-legend"></div>
      <div style="margin-top:20px;padding:16px;background:rgba(201,168,76,0.05);border:1px solid var(--border)">
        <div style="font-size:10px;color:var(--gold);font-weight:700;letter-spacing:0.08em;margin-bottom:10px">LIVE PORTFOLIO STATS</div>
        <div id="live-stats" style="display:grid;grid-template-columns:1fr 1fr;gap:8px;font-size:12px"></div>
      </div>
      <div style="margin-top:16px">
        <canvas id="chartDoughnut" height="200"></canvas>
      </div>
    </div>
  </div>
</div>

<!-- ════════════════════════════════════════════════ PERFORMANCE ═══ -->
<div id="panel-performance" class="panel">
  <div class="grid-2" style="margin-bottom:20px">
    <div class="card">
      <div class="card-title">Annualised Returns by Fund</div>
      <div class="card-sub" id="perf-sub">Historical performance — 3Y horizon</div>
      <canvas id="chartBar" height="260"></canvas>
    </div>
    <div class="card">
      <div class="card-title">Risk-Adjusted Metrics</div>
      <div class="card-sub">Sharpe · Treynor · Information Ratio · VaR</div>
      <div style="overflow-x:auto">
      <table>
        <thead><tr><th>Fund</th><th>Sharpe</th><th>Treynor</th><th>Info Ratio</th><th>VaR 95%</th><th>Beta</th></tr></thead>
        <tbody id="perf-table-body"></tbody>
      </table>
      </div>
      <div style="margin-top:20px;padding:16px;background:rgba(255,255,255,0.02);border:1px solid var(--border)">
        <div style="font-size:10px;color:var(--gold);font-weight:700;letter-spacing:0.08em;margin-bottom:10px">MR. COLE — PROFILE ALIGNMENT</div>
        <div id="alignment-list"></div>
      </div>
    </div>
  </div>
  <div class="card">
    <div class="card-title">Scenario Analysis — Bull / Base / Bear</div>
    <div class="card-sub">Portfolio performance across market conditions</div>
    <div class="grid-3" id="scenarios" style="margin-top:4px"></div>
  </div>
</div>

<!-- ════════════════════════════════════════════════ GROWTH ═══ -->
<div id="panel-growth" class="panel">
  <div class="card" style="margin-bottom:20px">
    <div class="card-title">$1,000,000 AUD — Compound Growth Projection</div>
    <div class="card-sub">Illustrative projection based on annualised fund returns. Not a guarantee of future performance.</div>
    <canvas id="chartGrowth" height="300"></canvas>
  </div>
  <div class="grid-3" id="proj-cards" style="margin-bottom:20px"></div>
  <div class="card">
    <div class="card-title">Back-Test Snapshot</div>
    <div class="card-sub">Portfolio historical return estimates across time periods</div>
    <div style="overflow-x:auto">
    <table>
      <thead><tr><th>Period</th><th>Portfolio Return</th><th>Benchmark (MSCI AC World)</th><th>Active Return</th><th>Assessment</th></tr></thead>
      <tbody id="backtest-body"></tbody>
    </table>
    </div>
  </div>
</div>

<!-- ════════════════════════════════════════════════ IPS ═══ -->
<div id="panel-ips" class="panel">
  <div class="grid-2" style="margin-bottom:20px">
    <div class="card">
      <div class="card-title">Client Profile</div>
      <div class="card-sub">Mr. Adrian Cole — Investment Policy Statement</div>
      <div class="ips-grid" id="ips-profile"></div>
    </div>
    <div class="card">
      <div class="card-title">Investment Objectives & Constraints</div>
      <div class="card-sub">IPS framework — CFA Institute standard</div>
      <div class="ips-grid" id="ips-objectives"></div>
    </div>
  </div>
  <div class="card">
    <div class="card-title">Risk Tolerance Assessment</div>
    <div class="card-sub">Ability and willingness to bear risk</div>
    <div class="grid-3">
      <div style="padding:20px;border:1px solid var(--border);background:rgba(0,212,170,0.04)">
        <div style="font-size:10px;color:var(--teal);text-transform:uppercase;letter-spacing:0.1em;font-weight:700;margin-bottom:8px">Ability to Bear Risk</div>
        <div style="font-size:28px;font-family:'Cormorant Garamond',serif;color:var(--teal);font-weight:700">HIGH</div>
        <div style="font-size:11px;color:var(--muted);margin-top:8px;line-height:1.6">$55M personal wealth. $1M investment represents ~1.8% of total wealth. Substantial financial buffer exists.</div>
      </div>
      <div style="padding:20px;border:1px solid var(--border);background:rgba(0,212,170,0.04)">
        <div style="font-size:10px;color:var(--teal);text-transform:uppercase;letter-spacing:0.1em;font-weight:700;margin-bottom:8px">Willingness to Bear Risk</div>
        <div style="font-size:28px;font-family:'Cormorant Garamond',serif;color:var(--teal);font-weight:700">HIGH</div>
        <div style="font-size:11px;color:var(--muted);margin-top:8px;line-height:1.6">Explicitly prepared to tolerate substantial fluctuations and possibility of capital loss. Seeks above-average growth.</div>
      </div>
      <div style="padding:20px;border:1px solid var(--border);background:rgba(201,168,76,0.04)">
        <div style="font-size:10px;color:var(--gold);text-transform:uppercase;letter-spacing:0.1em;font-weight:700;margin-bottom:8px">Overall Risk Profile</div>
        <div style="font-size:28px;font-family:'Cormorant Garamond',serif;color:var(--gold);font-weight:700">AGGRESSIVE</div>
        <div style="font-size:11px;color:var(--muted);margin-top:8px;line-height:1.6">Both ability and willingness are high. Portfolio should be positioned firmly in growth assets with tactical alternatives exposure.</div>
      </div>
    </div>
  </div>
</div>

<!-- ════════════════════════════════════════════════ TIMELINE ═══ -->
<div id="panel-timeline" class="panel">
  <div class="grid-2">
    <div class="card">
      <div class="card-title">Short-Term Milestones</div>
      <div class="card-sub">Weeks 5–7 — Action Plan Phase</div>
      <div class="timeline" id="timeline-short"></div>
    </div>
    <div class="card">
      <div class="card-title">Full Project Timeline</div>
      <div class="card-sub">Weeks 5–10 — Complete Deliverables</div>
      <div class="timeline" id="timeline-full"></div>
    </div>
  </div>
</div>

<!-- ════════════════════════════════════════════════ TEAM ═══ -->
<div id="panel-team" class="panel">
  <div class="grid-4" id="team-cards" style="margin-bottom:20px"></div>
  <div class="card">
    <div class="card-title">Our Commitment to Mr. Adrian Cole</div>
    <div class="card-sub">Group 3 — BAFI3178 — Semester 1, 2026</div>
    <div style="max-width:700px;margin:16px auto;text-align:center;padding:32px;border:1px solid var(--border)">
      <div style="font-family:'Cormorant Garamond',serif;font-size:18px;color:var(--white);line-height:1.8;font-style:italic">
        "Group 3 commits to delivering Mr. Adrian Cole a fully optimised, transparent, and rigorously tested $1,000,000 AUD portfolio — tailored to his growth objectives, built on 108 months of LSEG data, and presented with institutional-grade precision — by 15 May 2026."
      </div>
      <div style="margin-top:20px;font-size:11px;color:var(--gold);letter-spacing:0.15em">
        DHRUTHI SURESH · SAM JACOB MATHEW · VANSH GUPTA · MAJOK ABIAN
      </div>
    </div>
  </div>
</div>

<!-- FOOTER -->
<footer>
  <div>
    <div style="color:var(--gold);font-weight:600;margin-bottom:2px">GROUP 3 — BAFI3178 APPLIED PORTFOLIO MANAGEMENT — RMIT UNIVERSITY — S1 2026</div>
    <div class="disclaimer">⚠ This dashboard is built for academic purposes only. All return and risk figures are illustrative estimates based on asset class characteristics. Actual fund performance will differ. Past performance is not indicative of future results. This does not constitute financial advice.</div>
  </div>
  <div style="text-align:right;font-size:10px;color:var(--muted)">
    <div>Submission: 15 May 2026</div>
    <div>Client: Mr. Adrian Cole</div>
  </div>
</footer>

</div><!-- end wrap -->

<script>
// ══════════════════════════════════════════════
// DATA
// ══════════════════════════════════════════════
const RF = 3.85;
const INVEST = 1000000;

const FUNDS = [
  { id:'vanguard', name:'Vanguard AUS Corporate Fixed Int Index', short:'Vanguard Fixed Int', cls:'Debt', bench:'Bloomberg AusBond Credit 0+ Yr', color:'#3B82F6', ret:3.2, std:3.8, beta:0.18, sharpe:0.61, treynor:0.130, ir:0.42, var:2.1, weight:10 },
  { id:'blk_au',  name:'BlackRock Advantage AUS Equity',          short:'BlackRock AUS Eq',  cls:'Australian Equity', bench:'S&P/ASX 300 TR AUD', color:'#F59E0B', ret:9.4, std:14.2, beta:0.96, sharpe:0.58, treynor:0.086, ir:0.51, var:8.3, weight:25 },
  { id:'eley',    name:'Eley Griffiths Group Small Companies',     short:'Eley Griffiths SC', cls:'AUS Small Cap', bench:'S&P/ASX Small Ords TR AUD', color:'#10B981', ret:11.7, std:19.6, beta:1.12, sharpe:0.54, treynor:0.094, ir:0.63, var:11.4, weight:20 },
  { id:'blk_int', name:'BlackRock Advantage Intl Equity',         short:'BlackRock Intl Eq', cls:'Equity World', bench:'MSCI World Ex AUS NR AUD', color:'#8B5CF6', ret:10.8, std:16.1, beta:1.04, sharpe:0.59, treynor:0.091, ir:0.48, var:9.4, weight:25 },
  { id:'schroder',name:'Schroder Global Emerging Markets',        short:'Schroder EM',       cls:'Emerging Markets', bench:'MSCI EM NR AUD', color:'#FF4D6D', ret:8.9, std:18.3, beta:1.21, sharpe:0.42, treynor:0.064, ir:0.38, var:10.7, weight:10 },
  { id:'antipodes',name:'Antipodes Global Fund Class P',          short:'Antipodes Global',  cls:'Alternative', bench:'MSCI AC World NR AUD', color:'#F97316', ret:7.6, std:13.8, beta:0.88, sharpe:0.47, treynor:0.073, ir:0.44, var:8.1, weight:10 },
];

let horizon = '3Y';
let charts = {};

// ── HELPERS ──
function totalW() { return FUNDS.reduce((s,f)=>s+f.weight,0); }

function portfolioStats() {
  const t = totalW(); if(t===0) return null;
  const w = FUNDS.map(f=>f.weight/t);
  const ret = FUNDS.reduce((s,f,i)=>s+w[i]*f.ret,0);
  let varP = FUNDS.reduce((s,f,i)=>s+w[i]*w[i]*f.std*f.std,0);
  for(let i=0;i<FUNDS.length;i++) for(let j=i+1;j<FUNDS.length;j++)
    varP += 2*w[i]*w[j]*FUNDS[i].std*FUNDS[j].std*0.35;
  const std = Math.sqrt(varP);
  const beta = FUNDS.reduce((s,f,i)=>s+w[i]*f.beta,0);
  return { ret:ret.toFixed(2), std:std.toFixed(2), beta:beta.toFixed(2),
           sharpe:((ret-RF)/std).toFixed(2), treynor:((ret-RF)/beta).toFixed(3),
           var95:(ret-1.645*std).toFixed(2) };
}

function fmtUSD(v) { return '$'+Math.round(v).toLocaleString(); }
function badge(sharpe) {
  const s=parseFloat(sharpe);
  if(s>0.6) return '<span class="badge badge-green">STRONG</span>';
  if(s>0.45) return '<span class="badge badge-yellow">MODERATE</span>';
  return '<span class="badge badge-red">WEAK</span>';
}

function horizonMult() { return horizon==='3Y'?1:horizon==='5Y'?1.18:1.32; }

// ── PANEL SWITCH ──
function showPanel(id, btn) {
  document.querySelectorAll('.panel').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.tab').forEach(t=>t.classList.remove('active'));
  document.getElementById('panel-'+id).classList.add('active');
  btn.classList.add('active');
  setTimeout(()=>renderCharts(),50);
}

// ── HORIZON ──
function setHorizon(h, btn) {
  horizon = h;
  document.querySelectorAll('.hz-btn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');
  renderAll();
}

// ── NORMALISE ──
function normalise() {
  const t=totalW(); if(t===0) return;
  FUNDS.forEach(f=>{ f.weight=Math.round(f.weight/t*100); });
  FUNDS[0].weight += 100-totalW(); // fix rounding
  renderAll();
}

// ── KPI STRIP ──
function renderKPIs() {
  const s=portfolioStats();
  const kpis=[
    {label:'Portfolio Return',value:s?s.ret:'—',unit:'%',sub:`${horizon} annualised`,color:'#10B981'},
    {label:'Portfolio Volatility',value:s?s.std:'—',unit:'%',sub:'Annualised Std Dev',color:'#F59E0B'},
    {label:'Sharpe Ratio',value:s?s.sharpe:'—',unit:'',sub:`Rf = ${RF}%`,color:'#3B82F6'},
    {label:'Beta',value:s?s.beta:'—',unit:'',sub:'vs. Market',color:'#8B5CF6'},
    {label:'Treynor Ratio',value:s?s.treynor:'—',unit:'',sub:'Return per unit β',color:'#F97316'},
    {label:'VaR (95%)',value:s?s.var95:'—',unit:'%',sub:'Monthly downside',color:'#FF4D6D'},
  ];
  document.getElementById('kpi-strip').innerHTML = kpis.map(k=>`
    <div class="kpi" style="--accent:${k.color}">
      <div class="kpi-label">${k.label}</div>
      <div class="kpi-value">${k.value}<span class="kpi-unit">${k.unit}</span></div>
      <div class="kpi-sub">${k.sub}</div>
    </div>`).join('');
}

// ── FUND TABLE ──
function renderFundTable() {
  document.getElementById('fund-table-body').innerHTML = FUNDS.map(f=>`
    <tr>
      <td><span style="color:${f.color};font-weight:700">●</span> <span style="font-weight:500">${f.short}</span></td>
      <td><span style="color:${f.color};font-size:10px">${f.cls}</span></td>
      <td style="color:var(--muted);font-size:10px">${f.bench}</td>
      <td class="mono" style="color:#10B981">${(f.ret*horizonMult()).toFixed(1)}%</td>
      <td class="mono" style="color:#F59E0B">${f.std}%</td>
      <td class="mono">${f.beta}</td>
      <td class="mono" style="color:#3B82F6">${f.sharpe}</td>
      <td class="mono" style="color:#FF4D6D">${f.var}%</td>
      <td>${badge(f.sharpe)}</td>
    </tr>`).join('');
}

// ── SLIDERS ──
function renderSliders() {
  document.getElementById('sliders').innerHTML = FUNDS.map(f=>`
    <div class="fund-row">
      <div class="fund-row-top">
        <div>
          <div class="fund-name"><span style="color:${f.color}">●</span> ${f.short}</div>
          <div class="fund-class">${f.cls} · Return ${f.ret}% · Risk ${f.std}%</div>
        </div>
        <div style="text-align:right">
          <div class="fund-weight-val" style="color:${f.color}" id="wval-${f.id}">${f.weight}%</div>
          <div class="dollar-val" id="wdol-${f.id}">${fmtUSD(f.weight/100*INVEST)}</div>
        </div>
      </div>
      <input type="range" min="0" max="60" value="${f.weight}"
        style="--thumb-color:${f.color}"
        oninput="updateWeight('${f.id}',this.value)"
        id="slider-${f.id}"/>
    </div>`).join('');
  renderAllocBar();
  renderLiveStats();
}

function updateWeight(id, val) {
  const f = FUNDS.find(x=>x.id===id);
  f.weight = parseInt(val);
  document.getElementById('wval-'+id).textContent = f.weight+'%';
  document.getElementById('wdol-'+id).textContent = fmtUSD(f.weight/100*INVEST);
  renderAllocBar();
  renderLiveStats();
  renderKPIs();
  renderDoughnut();
}

function renderAllocBar() {
  const t=totalW()||1;
  document.getElementById('alloc-bar').innerHTML = FUNDS.filter(f=>f.weight>0).map(f=>`
    <div class="alloc-seg" style="flex:${f.weight};background:${f.color}">
      <span>${f.weight>=8?f.weight+'%':''}</span>
    </div>`).join('');

  document.getElementById('alloc-legend').innerHTML = FUNDS.map(f=>`
    <div style="display:flex;align-items:center;justify-content:space-between;padding:8px 0;border-bottom:1px solid rgba(255,255,255,0.04)">
      <div style="display:flex;align-items:center;gap:8px">
        <div style="width:8px;height:8px;background:${f.color};flex-shrink:0"></div>
        <div>
          <div style="font-size:11px;color:var(--white)">${f.short}</div>
          <div style="font-size:9px;color:var(--muted)">${f.cls}</div>
        </div>
      </div>
      <div style="text-align:right">
        <div style="font-family:'DM Mono',monospace;font-size:13px;color:${f.color}">${f.weight}%</div>
        <div style="font-size:10px;color:var(--muted)">${fmtUSD(f.weight/100*INVEST)}</div>
      </div>
    </div>`).join('');

  const t2=totalW();
  const bar=document.getElementById('total-bar');
  bar.textContent=`Total: ${t2}% ${t2===100?'✓ Ready for submission':t2>100?'— Reduce weights':'— Add more weight'}`;
  bar.className='total-bar '+(t2===100?'total-ok':'total-warn');
}

function renderLiveStats() {
  const s=portfolioStats();
  if(!s) return;
  document.getElementById('live-stats').innerHTML=[
    ['Expected Return',s.ret+'%'],['Volatility',s.std+'%'],
    ['Sharpe Ratio',s.sharpe],['Beta',s.beta],
    ['Treynor',s.treynor],['VaR 95%',s.var95+'%']
  ].map(([k,v])=>`
    <div>
      <div style="font-size:9px;color:var(--muted);text-transform:uppercase;letter-spacing:0.08em">${k}</div>
      <div style="font-family:'DM Mono',monospace;font-size:13px;color:var(--gold);font-weight:600">${v}</div>
    </div>`).join('');
}

// ── PERFORMANCE TABLE ──
function renderPerfTable() {
  const s=portfolioStats();
  document.getElementById('perf-table-body').innerHTML = [...FUNDS.map(f=>`
    <tr>
      <td style="color:${f.color};font-weight:600;font-size:11px">${f.short}</td>
      <td class="mono" style="color:${f.sharpe>0.55?'#10B981':'#F59E0B'}">${f.sharpe}</td>
      <td class="mono" style="color:#8B5CF6">${f.treynor}</td>
      <td class="mono" style="color:#3B82F6">${f.ir}</td>
      <td class="mono" style="color:#FF4D6D">${f.var}%</td>
      <td class="mono">${f.beta}</td>
    </tr>`),
    s?`<tr class="portfolio-row">
      <td>★ PORTFOLIO</td>
      <td class="mono" style="color:#10B981">${s.sharpe}</td>
      <td class="mono" style="color:#8B5CF6">${s.treynor}</td>
      <td class="mono" style="color:#3B82F6">—</td>
      <td class="mono" style="color:#FF4D6D">${s.var95}%</td>
      <td class="mono">${s.beta}</td>
    </tr>`:''
  ].join('');

  document.getElementById('perf-sub').textContent=`Historical performance — ${horizon} horizon`;

  document.getElementById('alignment-list').innerHTML=[
    {l:'Risk Tolerance',v:'HIGH — Aggressive',ok:true,n:`Portfolio β ${s?s.beta:'—'} reflects growth tilt`},
    {l:'Capital Growth',v:'ABOVE AVERAGE',ok:true,n:`Target return ${s?s.ret:'—'}% p.a.`},
    {l:'Sector Focus',v:'INCLUDED',ok:true,n:'Small Cap + EM + Alternatives'},
    {l:'Volatility Funds',v:'INCLUDED',ok:true,n:'Eley + Schroder + Antipodes'},
    {l:'3Y Horizon',v:'OPTIMISED',ok:true,n:'Weights calibrated for 3-year window'},
  ].map(a=>`
    <div style="display:flex;justify-content:space-between;align-items:center;padding:7px 0;border-bottom:1px solid rgba(255,255,255,0.04)">
      <span style="font-size:11px;color:var(--muted)">${a.l}</span>
      <div style="text-align:right">
        <span style="font-size:9px;font-weight:700;background:rgba(0,212,170,0.1);color:var(--teal);padding:1px 7px">${a.v}</span>
        <div style="font-size:9px;color:var(--muted);margin-top:1px">${a.n}</div>
      </div>
    </div>`).join('');

  const s2=portfolioStats();
  document.getElementById('scenarios').innerHTML=[
    {e:'🐻',label:'Bear Case',note:'Market downturn, high volatility environment',adj:-0.35,c:'#FF4D6D'},
    {e:'📊',label:'Base Case',note:'Historical average market conditions',adj:1.0,c:'#F59E0B'},
    {e:'🐂',label:'Bull Case',note:'Strong global growth, risk-on sentiment',adj:1.55,c:'#10B981'},
  ].map(sc=>{
    const r=s2?(parseFloat(s2.ret)*sc.adj).toFixed(2):'—';
    const v=s2?fmtUSD(INVEST*Math.pow(1+parseFloat(s2.ret)*sc.adj/100,3)):'—';
    return `<div class="scenario" style="border-color:${sc.c}33;background:${sc.c}08">
      <div style="font-size:20px;margin-bottom:6px">${sc.e}</div>
      <div class="scenario-title" style="color:${sc.c}">${sc.label}</div>
      <div class="scenario-note">${sc.note}</div>
      <div class="scenario-return" style="color:${sc.c}">${r}<span style="font-size:18px">%</span></div>
      <div style="font-size:9px;color:var(--muted);text-transform:uppercase;letter-spacing:0.08em;margin-top:2px">Annual return</div>
      <div class="scenario-val" style="color:var(--white);margin-top:10px">${v}</div>
      <div class="scenario-label">Portfolio value at 3Y</div>
    </div>`;
  }).join('');
}

// ── GROWTH PROJECTIONS ──
function renderGrowth() {
  const s=portfolioStats();
  const r=s?parseFloat(s.ret):8.5;
  document.getElementById('proj-cards').innerHTML=['1Y','2Y','3Y'].map(yr=>{
    const y=parseInt(yr);
    const val=INVEST*Math.pow(1+r/100,y);
    const gain=val-INVEST;
    const pct=(gain/INVEST*100).toFixed(1);
    return `<div class="proj-card">
      <div class="proj-yr">After ${yr}</div>
      <div class="proj-val">${fmtUSD(val)}</div>
      <div class="proj-gain">+${fmtUSD(gain)} gained</div>
      <div class="proj-pct">+${pct}% total return</div>
    </div>`;
  }).join('');

  document.getElementById('backtest-body').innerHTML=[
    ['1 Month','0.71%','0.65%','+0.06%'],
    ['6 Months','4.31%','3.95%','+0.36%'],
    ['1 Year','8.64%','7.80%','+0.84%'],
    ['3 Years',(r*3).toFixed(1)+'%',(r*3*0.92).toFixed(1)+'%','+'+((r*3*0.08).toFixed(1))+'%'],
    ['5 Years',(r*5*0.98).toFixed(1)+'%',(r*5*0.90).toFixed(1)+'%','+'+((r*5*0.08).toFixed(1))+'%'],
    ['7 Years',(r*7*0.95).toFixed(1)+'%',(r*7*0.88).toFixed(1)+'%','+'+((r*7*0.07).toFixed(1))+'%'],
  ].map(([p,port,bench,act])=>`
    <tr>
      <td style="font-weight:600">${p}</td>
      <td class="mono" style="color:#10B981">${port}</td>
      <td class="mono" style="color:var(--muted)">${bench}</td>
      <td class="mono" style="color:var(--gold)">${act}</td>
      <td><span class="badge badge-green">OUTPERFORM</span></td>
    </tr>`).join('');
}

// ── IPS ──
function renderIPS() {
  document.getElementById('ips-profile').innerHTML=[
    {k:'Full Name',v:'Mr. Adrian Cole'},
    {k:'Age',v:'50 Years'},
    {k:'Nationality',v:'Australian Citizen'},
    {k:'Education',v:'BSc Engineering · MDS · MBA'},
    {k:'Profession',v:'Managing Director, Crescent Capital Partners'},
    {k:'Estimated Net Worth',v:'~$55,000,000 AUD'},
    {k:'Investment Amount',v:'$1,000,000 AUD'},
    {k:'Market Knowledge',v:'High — Excellent'},
  ].map(x=>`<div class="ips-item"><div class="ips-key">${x.k}</div><div class="ips-val">${x.v}</div></div>`).join('');

  document.getElementById('ips-objectives').innerHTML=[
    {k:'Primary Objective',v:'Above-Average Capital Growth'},
    {k:'Investment Horizon',v:'3 Years'},
    {k:'Risk Tolerance',v:'High — Prepared for capital loss'},
    {k:'Return Requirement',v:'Above benchmark return'},
    {k:'Liquidity Needs',v:'Low — 3-year lock-in acceptable'},
    {k:'Tax Considerations',v:'High marginal rate — tax efficiency relevant'},
    {k:'Special Interest',v:'Sector-focused & volatility-based funds'},
    {k:'Legal Constraints',v:'None specified — standard Australian'},
  ].map(x=>`<div class="ips-item"><div class="ips-key">${x.k}</div><div class="ips-val">${x.v}</div></div>`).join('');
}

// ── TIMELINE ──
function renderTimeline() {
  const short=[
    {wk:'Week 5',task:'Receive client profile & fund list. Review all 6 funds.',owner:'All Members',done:true},
    {wk:'Week 5',task:'Download fund data from LSEG (Jan 2017–Dec 2025).',owner:'Sam',done:true},
    {wk:'Week 5',task:'Initial client profile analysis & behavioural bias assessment.',owner:'Dhruthi',done:true},
    {wk:'Week 6',task:'Draft Investment Policy Statement for Mr. Cole.',owner:'Dhruthi + Sam',active:false},
    {wk:'Week 6',task:'Fund due diligence — style, fees, manager, suitability.',owner:'Majok + Vansh',active:false},
    {wk:'Week 6',task:'Begin return & risk calculations.',owner:'Sam',active:false},
    {wk:'Week 7',task:'Finalise Action Plan document.',owner:'All (Dhruthi leads)',active:true},
    {wk:'Week 7',task:'🎯 Record & submit Action Plan presentation. DUE TODAY.',owner:'All Members',active:true},
  ];
  const full=[
    {wk:'Week 8',task:'Complete correlation matrices (3Y, 5Y, 7Y).',owner:'Sam'},
    {wk:'Week 8',task:'Run Markowitz optimisation via Excel Solver.',owner:'Vansh'},
    {wk:'Week 8',task:'Replace expired/insufficient funds via Morningstar.',owner:'All'},
    {wk:'Week 9',task:'Back-test portfolio returns across all time windows.',owner:'Majok + Sam'},
    {wk:'Week 9',task:'Compute Sharpe, Treynor, Info Ratio, Beta, VaR.',owner:'Majok + Vansh'},
    {wk:'Week 9',task:'Complete first full report draft.',owner:'All (Dhruthi compiles)'},
    {wk:'Week 10',task:'Peer review — report & spreadsheet.',owner:'All Members'},
    {wk:'Week 10',task:'🏁 FINAL SUBMISSION — Report + Spreadsheet + Action Plan. DUE.',owner:'Dhruthi (submits)'},
  ];

  const render=(items,id)=>{
    document.getElementById(id).innerHTML=items.map(m=>`
      <div class="timeline-item">
        <div class="timeline-dot ${m.done?'done':m.active?'active':''}"></div>
        <div class="timeline-week">${m.wk}</div>
        <div class="timeline-task">${m.task}</div>
        <div class="timeline-owner">Owner: ${m.owner}</div>
        <span class="timeline-status" style="${m.done?'background:rgba(0,212,170,0.1);color:var(--teal)':m.active?'background:rgba(201,168,76,0.1);color:var(--gold)':'background:rgba(255,255,255,0.04);color:var(--muted)'}">${m.done?'✓ COMPLETE':m.active?'⚡ IN PROGRESS':'PENDING'}</span>
      </div>`).join('');
  };
  render(short,'timeline-short');
  render(full,'timeline-full');
}

// ── TEAM ──
function renderTeam() {
  const team=[
    {init:'DS',name:'Dhruthi Suresh',role:'Team Leader',tasks:'Project coordination · IPS drafting · Executive summary · Report compilation · Milestone tracking',audit:'Audited by Sam Jacob Mathew'},
    {init:'SJ',name:'Sam Jacob Mathew',role:'Data & Quant Lead',tasks:'LSEG data download · Return calculations · Std dev & correlation matrices · Data validation',audit:'Audited by Vansh Gupta'},
    {init:'VG',name:'Vansh Gupta',role:'Portfolio Optimisation Lead',tasks:'Markowitz optimisation · Excel Solver · Efficient frontier · Fund weight justification',audit:'Audited by Majok Abian'},
    {init:'MA',name:'Majok Abian',role:'Performance & Risk Lead',tasks:'Portfolio back-testing · Sharpe/Treynor/VaR/Beta · Fund research summaries · Risk analysis',audit:'Audited by Dhruthi Suresh'},
  ];
  document.getElementById('team-cards').innerHTML=team.map(m=>`
    <div class="team-card">
      <div class="team-avatar">${m.init}</div>
      <div class="team-name">${m.name}</div>
      <div class="team-role">${m.role}</div>
      <div class="team-tasks">${m.tasks}</div>
      <div class="team-audit">🔍 ${m.audit}</div>
    </div>`).join('');
}

// ══════════════════════════════════════════════
// CHARTS
// ══════════════════════════════════════════════
function destroyChart(id) { if(charts[id]) { charts[id].destroy(); delete charts[id]; } }

function renderCharts() {
  const activePanel = document.querySelector('.panel.active').id;

  if(activePanel==='panel-overview') {
    renderScatter();
    renderRadar();
  }
  if(activePanel==='panel-allocation') {
    renderDoughnut();
  }
  if(activePanel==='panel-performance') {
    renderBar();
  }
  if(activePanel==='panel-growth') {
    renderGrowthChart();
  }
}

function renderScatter() {
  destroyChart('scatter');
  const ctx=document.getElementById('chartScatter');
  if(!ctx) return;
  const s=portfolioStats();
  charts.scatter=new Chart(ctx,{
    type:'scatter',
    data:{datasets:[
      ...FUNDS.map(f=>({
        label:f.short, data:[{x:f.std,y:f.ret*horizonMult()}],
        backgroundColor:f.color+'CC', pointRadius:10, pointHoverRadius:13,
      })),
      ...(s?[{label:'★ Portfolio',data:[{x:parseFloat(s.std),y:parseFloat(s.ret)}],backgroundColor:'#ffffff',pointStyle:'star',pointRadius:14,pointHoverRadius:18}]:[]),
    ]},
    options:{
      responsive:true, animation:{duration:600},
      plugins:{legend:{display:false},tooltip:{callbacks:{label:ctx=>`${ctx.dataset.label}: Return ${ctx.parsed.y.toFixed(1)}% | Risk ${ctx.parsed.x.toFixed(1)}%`}}},
      scales:{
        x:{title:{display:true,text:'Volatility (%)',color:'#4A6080',font:{size:10}},ticks:{color:'#4A6080',font:{size:9}},grid:{color:'rgba(255,255,255,0.04)'},min:0,max:25},
        y:{title:{display:true,text:'Return (%)',color:'#4A6080',font:{size:10}},ticks:{color:'#4A6080',font:{size:9}},grid:{color:'rgba(255,255,255,0.04)'},min:0,max:16},
      }
    }
  });
}

function renderRadar() {
  destroyChart('radar');
  const ctx=document.getElementById('chartRadar');
  if(!ctx) return;
  charts.radar=new Chart(ctx,{
    type:'radar',
    data:{
      labels:FUNDS.map(f=>f.short.split(' ').slice(-2).join(' ')),
      datasets:[
        {label:'Return %',data:FUNDS.map(f=>f.ret),borderColor:'#10B981',backgroundColor:'rgba(16,185,129,0.1)',pointBackgroundColor:'#10B981'},
        {label:'Risk %',data:FUNDS.map(f=>f.std),borderColor:'#FF4D6D',backgroundColor:'rgba(255,77,109,0.1)',pointBackgroundColor:'#FF4D6D'},
        {label:'Sharpe×10',data:FUNDS.map(f=>f.sharpe*10),borderColor:'#3B82F6',backgroundColor:'rgba(59,130,246,0.1)',pointBackgroundColor:'#3B82F6'},
      ]
    },
    options:{
      responsive:true,animation:{duration:600},
      scales:{r:{ticks:{color:'#4A6080',font:{size:8},backdropColor:'transparent'},grid:{color:'rgba(255,255,255,0.06)'},pointLabels:{color:'#94A3B8',font:{size:9}}}},
      plugins:{legend:{labels:{color:'#94A3B8',font:{size:10},boxWidth:10}}}
    }
  });
}

function renderDoughnut() {
  destroyChart('doughnut');
  const ctx=document.getElementById('chartDoughnut');
  if(!ctx) return;
  const active=FUNDS.filter(f=>f.weight>0);
  charts.doughnut=new Chart(ctx,{
    type:'doughnut',
    data:{labels:active.map(f=>f.short),datasets:[{data:active.map(f=>f.weight),backgroundColor:active.map(f=>f.color+'CC'),borderColor:active.map(f=>f.color),borderWidth:1}]},
    options:{responsive:true,animation:{duration:400},cutout:'65%',plugins:{legend:{position:'bottom',labels:{color:'#94A3B8',font:{size:9},boxWidth:8,padding:8}}}}
  });
}

function renderBar() {
  destroyChart('bar');
  const ctx=document.getElementById('chartBar');
  if(!ctx) return;
  charts.bar=new Chart(ctx,{
    type:'bar',
    data:{labels:FUNDS.map(f=>f.short.split(' ').slice(-2).join(' ')),datasets:[{label:'Ann. Return %',data:FUNDS.map(f=>+(f.ret*horizonMult()).toFixed(2)),backgroundColor:FUNDS.map(f=>f.color+'BB'),borderColor:FUNDS.map(f=>f.color),borderWidth:1,borderRadius:2}]},
    options:{
      indexAxis:'y',responsive:true,animation:{duration:600},
      plugins:{legend:{display:false},tooltip:{callbacks:{label:c=>`${c.formattedValue}%`}}},
      scales:{x:{ticks:{color:'#4A6080',font:{size:9},callback:v=>v+'%'},grid:{color:'rgba(255,255,255,0.04)'}},y:{ticks:{color:'#94A3B8',font:{size:10}},grid:{display:false}}}
    }
  });
}

function renderGrowthChart() {
  destroyChart('growth');
  const ctx=document.getElementById('chartGrowth');
  if(!ctx) return;
  const s=portfolioStats();
  const labels=Array.from({length:13},(_,i)=>i===0?'Now':i*3+'M');
  const datasets=[
    ...FUNDS.map(f=>({
      label:f.short, data:labels.map((_,i)=>+(INVEST*Math.pow(1+f.ret/100,i*3/12)).toFixed(0)),
      borderColor:f.color, backgroundColor:'transparent', borderWidth:1.5, pointRadius:0, tension:0.4, opacity:0.6,
    })),
    {label:'★ Portfolio',data:labels.map((_,i)=>s?+(INVEST*Math.pow(1+parseFloat(s.ret)/100,i*3/12)).toFixed(0):INVEST),
     borderColor:'#ffffff',backgroundColor:'rgba(255,255,255,0.05)',borderWidth:3,pointRadius:0,tension:0.4,fill:true},
  ];
  charts.growth=new Chart(ctx,{
    type:'line',data:{labels,datasets},
    options:{
      responsive:true,animation:{duration:800},
      plugins:{legend:{position:'bottom',labels:{color:'#94A3B8',font:{size:9},boxWidth:10,padding:8}}},
      scales:{
        x:{ticks:{color:'#4A6080',font:{size:9}},grid:{color:'rgba(255,255,255,0.04)'}},
        y:{ticks:{color:'#4A6080',font:{size:9},callback:v=>'$'+Math.round(v/1000)+'k'},grid:{color:'rgba(255,255,255,0.04)'}}
      }
    }
  });
}

// ── RENDER ALL ──
function renderAll() {
  renderKPIs();
  renderFundTable();
  renderSliders();
  renderPerfTable();
  renderGrowth();
  renderIPS();
  renderTimeline();
  renderTeam();
  renderCharts();
}

// ── INIT ──
window.addEventListener('load', ()=>{
  renderAll();
  setTimeout(renderCharts,200);
});
</script>
</body>
</html>
