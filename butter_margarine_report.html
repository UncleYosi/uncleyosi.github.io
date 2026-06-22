<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Butter & Margarine Category Report — FoodByUs</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --red: #C8392B;
    --bg: #F8F9FA;
    --surface: #FFFFFF;
    --border: #E2E4E8;
    --text-primary: #1A1A1A;
    --text-secondary: #6B7280;
    --text-muted: #9CA3AF;
    /* butter */
    --unsalted: #D9A441;
    --pc: #378ADD;
    --salted: #1D9E75;
    --bakery: #534AB7;
    /* margarine */
    --marg: #E0A82E;
    --marg-pc: #378ADD;
    --blend: #D85A30;
    --plant: #1D9E75;
  }

  body { font-family: 'Inter', sans-serif; background: var(--bg); color: var(--text-primary); font-size: 13px; line-height: 1.5; -webkit-font-smoothing: antialiased; }

  /* ── HEADER ── */
  .header { background: var(--surface); border-bottom: 3px solid var(--red); padding: 32px 48px 0; }
  .header-inner { max-width: 1100px; margin: 0 auto; display: flex; align-items: flex-start; justify-content: space-between; gap: 24px; padding-bottom: 24px; }
  .header-logo { font-size: 13px; font-weight: 600; letter-spacing: .08em; text-transform: uppercase; color: var(--red); }
  .header-title { font-size: 22px; font-weight: 600; color: var(--text-primary); margin-top: 6px; letter-spacing: -.3px; }
  .header-meta { font-size: 12px; color: var(--text-secondary); text-align: right; line-height: 1.7; padding-top: 4px; }
  .header-meta strong { color: var(--text-primary); }

  /* ── TABS ── */
  .tabs { max-width: 1100px; margin: 0 auto; display: flex; gap: 0; }
  .tab-btn {
    padding: 12px 24px;
    font-size: 13px;
    font-weight: 500;
    color: var(--text-secondary);
    background: none;
    border: none;
    border-bottom: 2px solid transparent;
    cursor: pointer;
    letter-spacing: .01em;
    transition: color .15s, border-color .15s;
  }
  .tab-btn:hover { color: var(--text-primary); }
  .tab-btn.active { color: var(--red); border-bottom-color: var(--red); }

  /* ── LAYOUT ── */
  .tab-panel { display: none; }
  .tab-panel.active { display: block; }
  .page { max-width: 1100px; margin: 0 auto; padding: 40px 48px 80px; }

  /* ── SECTION LABEL ── */
  .section-label { font-size: 10px; font-weight: 600; letter-spacing: .1em; text-transform: uppercase; color: var(--text-muted); margin-bottom: 14px; margin-top: 40px; }
  .section-label:first-child { margin-top: 0; }

  /* ── METRIC CARDS ── */
  .metrics { display: grid; grid-template-columns: repeat(5, 1fr); gap: 1px; background: var(--border); border: 1px solid var(--border); border-radius: 6px; overflow: hidden; }
  .metric { background: var(--surface); padding: 20px 20px 18px; }
  .metric-label { font-size: 11px; color: var(--text-muted); margin-bottom: 6px; font-weight: 500; }
  .metric-value { font-size: 24px; font-weight: 600; color: var(--text-primary); letter-spacing: -.5px; line-height: 1; margin-bottom: 4px; }
  .metric-sub { font-size: 11px; color: var(--text-secondary); }

  /* ── CHARTS ── */
  .chart-row { display: grid; grid-template-columns: 1fr 380px; gap: 16px; margin-top: 16px; }
  .chart-card { background: var(--surface); border: 1px solid var(--border); border-radius: 6px; padding: 22px 24px; }
  .chart-card-full { background: var(--surface); border: 1px solid var(--border); border-radius: 6px; padding: 22px 24px; margin-top: 16px; }
  .chart-title { font-size: 11px; font-weight: 600; letter-spacing: .07em; text-transform: uppercase; color: var(--text-secondary); margin-bottom: 16px; }
  .chart-wrap { position: relative; }

  /* ── LEGEND ── */
  .legend { display: flex; flex-wrap: wrap; gap: 14px; margin-top: 14px; padding-top: 14px; border-top: 1px solid var(--border); }
  .legend-item { display: flex; align-items: center; gap: 6px; font-size: 11px; color: var(--text-secondary); }
  .legend-swatch { width: 8px; height: 8px; border-radius: 2px; flex-shrink: 0; }

  /* ── CATEGORY TABLES ── */
  .cat-grid   { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; margin-top: 16px; }
  .cat-grid-2 { display: grid; grid-template-columns: repeat(2, 1fr); gap: 16px; margin-top: 16px; }
  .cat-card { background: var(--surface); border: 1px solid var(--border); border-radius: 6px; overflow: hidden; }
  .cat-card-header { display: flex; align-items: center; gap: 10px; padding: 14px 16px; border-bottom: 1px solid var(--border); }
  .cat-colour-bar { width: 3px; height: 28px; border-radius: 2px; flex-shrink: 0; }
  .cat-card-title { font-size: 13px; font-weight: 600; color: var(--text-primary); }
  .cat-card-total { font-size: 11px; color: var(--text-secondary); margin-top: 1px; }
  .cat-table { width: 100%; border-collapse: collapse; font-size: 12px; }
  .cat-table th { padding: 8px 16px; text-align: left; font-size: 10px; font-weight: 600; letter-spacing: .07em; text-transform: uppercase; color: var(--text-muted); border-bottom: 1px solid var(--border); background: #FAFAFA; }
  .cat-table th:last-child, .cat-table td:last-child { text-align: right; }
  .cat-table td { padding: 9px 16px; color: var(--text-primary); border-bottom: 1px solid var(--border); }
  .cat-table tr:last-child td { border-bottom: none; }
  .cat-table td:first-child { display: flex; align-items: center; }
  .brand-dot { display: inline-block; width: 7px; height: 7px; border-radius: 50%; margin-right: 7px; flex-shrink: 0; vertical-align: middle; position: relative; top: -1px; }
  .share-bar-wrap { display: flex; align-items: center; gap: 8px; }
  .share-bar-bg { flex: 1; height: 4px; background: #F0F0F0; border-radius: 2px; min-width: 60px; }
  .share-bar-fill { height: 4px; border-radius: 2px; }

  /* ── FOOTNOTE ── */
  .footnote { margin-top: 48px; padding-top: 20px; border-top: 1px solid var(--border); font-size: 11px; color: var(--text-muted); line-height: 1.7; }
</style>
</head>
<body>

<div class="header">
  <div class="header-inner">
    <div>
      <div class="header-logo">FoodByUs</div>
      <div class="header-title">Butter &amp; Margarine Category Report</div>
    </div>
    <div class="header-meta">
      <strong>Period:</strong> July 2025 – June 2026<br>
      <strong>Scope:</strong> FBU platform · All channels<br>
      <strong>Prepared by:</strong> Manufacturer Sales, FoodByUs
    </div>
  </div>
  <div class="tabs">
    <button class="tab-btn active" onclick="switchTab('butter')">Butter</button>
    <button class="tab-btn" onclick="switchTab('marg')">Margarine</button>
  </div>
</div>

<!-- ══════════════════════════════════════════════════════════ -->
<!-- TAB 1 — BUTTER                                             -->
<!-- ══════════════════════════════════════════════════════════ -->
<div id="tab-butter" class="tab-panel active">
<div class="page">

  <div class="section-label">Category overview</div>
  <div class="metrics">
    <div class="metric"><div class="metric-label">Total Sales</div><div class="metric-value">$1.92M</div><div class="metric-sub">12-month period</div></div>
    <div class="metric"><div class="metric-label">Monthly average</div><div class="metric-value">$160.0k</div><div class="metric-sub">Across 12 months</div></div>
    <div class="metric"><div class="metric-label">Active categories</div><div class="metric-value">4</div><div class="metric-sub">Unsalted leads at 64%</div></div>
    <div class="metric"><div class="metric-label">Largest brand</div><div class="metric-value">Western Star</div><div class="metric-sub">22.4% · $430k</div></div>
    <div class="metric"><div class="metric-label">No. 2 brand</div><div class="metric-value">Devondale</div><div class="metric-sub">17.2% · $331k</div></div>
  </div>

  <div class="chart-row">
    <div class="chart-card">
      <div class="chart-title">Monthly Sales by butter type ($)</div>
      <div class="chart-wrap" style="height:240px"><canvas id="typeBar"></canvas></div>
      <div class="legend">
        <div class="legend-item"><span class="legend-swatch" style="background:var(--unsalted)"></span>Unsalted</div>
        <div class="legend-item"><span class="legend-swatch" style="background:var(--pc)"></span>Portion control</div>
        <div class="legend-item"><span class="legend-swatch" style="background:var(--salted)"></span>Salted</div>
        <div class="legend-item"><span class="legend-swatch" style="background:var(--bakery)"></span>Bakery / pastry</div>
      </div>
    </div>
    <div class="chart-card">
      <div class="chart-title">Category mix — 12-month share</div>
      <div class="chart-wrap" style="height:240px"><canvas id="catDonut"></canvas></div>
    </div>
  </div>

  <div class="chart-card-full">
    <div class="chart-title">Monthly Sales by brand — top 6 ($)</div>
    <div class="chart-wrap" style="height:220px"><canvas id="brandBar"></canvas></div>
    <div class="legend">
      <div class="legend-item"><span class="legend-swatch" style="background:#D9A441"></span>Western Star</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#378ADD"></span>Devondale</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#9CA3AF"></span>Unbranded</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#1D9E75"></span>Pauls</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#534AB7"></span>Pepe Saya</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#D85A30"></span>Anchor</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#D1D5DB"></span>Other brands</div>
    </div>
  </div>

  <div class="section-label">Brand share by category</div>
  <div class="cat-grid-2">
    <div class="cat-card">
      <div class="cat-card-header"><div class="cat-colour-bar" style="background:var(--unsalted)"></div><div><div class="cat-card-title">Unsalted</div><div class="cat-card-total">$1,227,275 · 63.9% of category</div></div></div>
      <table class="cat-table"><thead><tr><th>Brand</th><th>Sales</th><th>Share</th></tr></thead><tbody id="unsaltedTable"></tbody></table>
    </div>
    <div class="cat-card">
      <div class="cat-card-header"><div class="cat-colour-bar" style="background:var(--pc)"></div><div><div class="cat-card-title">Portion control</div><div class="cat-card-total">$422,691 · 22.0% of category</div></div></div>
      <table class="cat-table"><thead><tr><th>Brand</th><th>Sales</th><th>Share</th></tr></thead><tbody id="bpcTable"></tbody></table>
    </div>
  </div>
  <div class="cat-grid-2">
    <div class="cat-card">
      <div class="cat-card-header"><div class="cat-colour-bar" style="background:var(--salted)"></div><div><div class="cat-card-title">Salted</div><div class="cat-card-total">$191,137 · 10.0% of category</div></div></div>
      <table class="cat-table"><thead><tr><th>Brand</th><th>Sales</th><th>Share</th></tr></thead><tbody id="saltedTable"></tbody></table>
    </div>
    <div class="cat-card">
      <div class="cat-card-header"><div class="cat-colour-bar" style="background:var(--bakery)"></div><div><div class="cat-card-title">Bakery / pastry</div><div class="cat-card-total">$78,407 · 4.1% of category</div></div></div>
      <table class="cat-table"><thead><tr><th>Brand</th><th>Sales</th><th>Share</th></tr></thead><tbody id="bakeryTable"></tbody></table>
    </div>
  </div>

  <div class="footnote">Period: July 2025 – June 2026 (12 months) &nbsp;·&nbsp; June 2026 partial month &nbsp;·&nbsp; Sales figures reflect platform sales &nbsp;·&nbsp; "Unbranded" denotes butter ordered without a specified brand &nbsp;·&nbsp; Prepared by Manufacturer Sales, FoodByUs</div>
</div>
</div>

<!-- ══════════════════════════════════════════════════════════ -->
<!-- TAB 2 — MARGARINE                                          -->
<!-- ══════════════════════════════════════════════════════════ -->
<div id="tab-marg" class="tab-panel">
<div class="page">

  <div class="section-label">Category overview</div>
  <div class="metrics">
    <div class="metric"><div class="metric-label">Total Sales</div><div class="metric-value">$159k</div><div class="metric-sub">12-month period</div></div>
    <div class="metric"><div class="metric-label">Monthly average</div><div class="metric-value">$13.3k</div><div class="metric-sub">Across 12 months</div></div>
    <div class="metric"><div class="metric-label">Active categories</div><div class="metric-value">4</div><div class="metric-sub">Margarine leads at 50%</div></div>
    <div class="metric"><div class="metric-label">Largest brand</div><div class="metric-value">Lurpak</div><div class="metric-sub">19.5% · $31k · blends</div></div>
    <div class="metric"><div class="metric-label">No. 2 brand</div><div class="metric-value">Miracle</div><div class="metric-sub">18.3% · $29k · margarine</div></div>
  </div>

  <div class="chart-row">
    <div class="chart-card">
      <div class="chart-title">Monthly Sales by spread type ($)</div>
      <div class="chart-wrap" style="height:240px"><canvas id="mTypeBar"></canvas></div>
      <div class="legend">
        <div class="legend-item"><span class="legend-swatch" style="background:var(--marg)"></span>Margarine</div>
        <div class="legend-item"><span class="legend-swatch" style="background:var(--blend)"></span>Blends</div>
        <div class="legend-item"><span class="legend-swatch" style="background:var(--plant)"></span>Plant-based spreads</div>
        <div class="legend-item"><span class="legend-swatch" style="background:var(--marg-pc)"></span>Portion control</div>
      </div>
    </div>
    <div class="chart-card">
      <div class="chart-title">Category mix — 12-month share</div>
      <div class="chart-wrap" style="height:240px"><canvas id="mDonut"></canvas></div>
    </div>
  </div>

  <div class="chart-card-full">
    <div class="chart-title">Monthly Sales by brand — top 6 ($)</div>
    <div class="chart-wrap" style="height:220px"><canvas id="mBrandBar"></canvas></div>
    <div class="legend">
      <div class="legend-item"><span class="legend-swatch" style="background:#1D4ED8"></span>Lurpak</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#E0A82E"></span>Miracle</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#D9A441"></span>Western Star</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#B4894A"></span>Sunlit Plains</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#9CA3AF"></span>Unbranded</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#639922"></span>Mrs McGregor's</div>
      <div class="legend-item"><span class="legend-swatch" style="background:#D1D5DB"></span>Other brands</div>
    </div>
  </div>

  <div class="section-label">Brand share by category</div>
  <div class="cat-grid-2">
    <div class="cat-card">
      <div class="cat-card-header"><div class="cat-colour-bar" style="background:var(--marg)"></div><div><div class="cat-card-title">Margarine</div><div class="cat-card-total">$78,918 · 49.5% of category</div></div></div>
      <table class="cat-table"><thead><tr><th>Brand</th><th>Sales</th><th>Share</th></tr></thead><tbody id="margTable"></tbody></table>
    </div>
    <div class="cat-card">
      <div class="cat-card-header"><div class="cat-colour-bar" style="background:var(--blend)"></div><div><div class="cat-card-title">Blends</div><div class="cat-card-total">$55,298 · 34.7% of category</div></div></div>
      <table class="cat-table"><thead><tr><th>Brand</th><th>Sales</th><th>Share</th></tr></thead><tbody id="mBlendTable"></tbody></table>
    </div>
  </div>
  <div class="cat-grid-2">
    <div class="cat-card">
      <div class="cat-card-header"><div class="cat-colour-bar" style="background:var(--plant)"></div><div><div class="cat-card-title">Plant-based spreads</div><div class="cat-card-total">$14,441 · 9.1% of category</div></div></div>
      <table class="cat-table"><thead><tr><th>Brand</th><th>Sales</th><th>Share</th></tr></thead><tbody id="plantTable"></tbody></table>
    </div>
    <div class="cat-card">
      <div class="cat-card-header"><div class="cat-colour-bar" style="background:var(--marg-pc)"></div><div><div class="cat-card-title">Portion control</div><div class="cat-card-total">$10,664 · 6.7% of category</div></div></div>
      <table class="cat-table"><thead><tr><th>Brand</th><th>Sales</th><th>Share</th></tr></thead><tbody id="mpcTable"></tbody></table>
    </div>
  </div>

  <div class="footnote">Period: July 2025 – June 2026 (12 months) &nbsp;·&nbsp; June 2026 partial month &nbsp;·&nbsp; Sales figures reflect platform sales &nbsp;·&nbsp; "Blends" are butter/oil spreadable products &nbsp;·&nbsp; "Unbranded" denotes product ordered without a specified brand &nbsp;·&nbsp; Prepared by Manufacturer Sales, FoodByUs</div>
</div>
</div>

<script>
// ── UTILITIES ──────────────────────────────────────────────────────────────
const months = ['Jul 25','Aug 25','Sep 25','Oct 25','Nov 25','Dec 25','Jan 26','Feb 26','Mar 26','Apr 26','May 26','Jun 26'];
const gridColor = 'rgba(0,0,0,0.06)';
const tickColor = '#9CA3AF';
const fmt  = v => '$' + Math.round(v).toLocaleString('en-AU');
const fmtK = v => '$' + (v/1000).toFixed(0) + 'k';

function buildTable(tbodyId, brands) {
  const total = brands.reduce((s,b) => s + b.gmv, 0);
  const tbody = document.getElementById(tbodyId);
  brands.forEach(b => {
    const share = (b.gmv / total * 100);
    const tr = document.createElement('tr');
    tr.innerHTML = `
      <td><span class="brand-dot" style="background:${b.color}"></span>${b.name}</td>
      <td>${fmt(b.gmv)}</td>
      <td><div class="share-bar-wrap"><span style="min-width:34px;text-align:right">${share.toFixed(1)}%</span><div class="share-bar-bg"><div class="share-bar-fill" style="width:${share}%;background:${b.color}"></div></div></div></td>`;
    tbody.appendChild(tr);
  });
}

function switchTab(id) {
  document.querySelectorAll('.tab-panel').forEach(p => p.classList.remove('active'));
  document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
  document.getElementById('tab-' + id).classList.add('active');
  event.target.classList.add('active');
}

const stackOpts = {
  responsive:true, maintainAspectRatio:false,
  plugins:{legend:{display:false}, tooltip:{callbacks:{label:ctx=>` ${ctx.dataset.label}: ${fmt(ctx.parsed.y)}`}}},
  scales:{
    x:{stacked:true, ticks:{color:tickColor,font:{size:11},autoSkip:false,maxRotation:45}, grid:{display:false}},
    y:{stacked:true, ticks:{color:tickColor,font:{size:11},callback:fmtK}, grid:{color:gridColor}}
  }
};

// ════════════ BUTTER ════════════
const unsalted = [96476.99,99578.80,102935.10,100230.00,105147.14,117307.83,94727.96,96563.99,110397.48,100692.00,116284.40,86933.01];
const pc       = [42509.77,35288.52,33201.60,36620.66,41317.99,40121.76,35703.73,31803.55,37650.54,31488.69,34495.72,22488.78];
const salted   = [11121.45,14354.96,12971.94,19726.20,18910.28,17105.18,18318.11,17464.82,18799.75,16942.30,14761.05,10661.13];
const bakery   = [6716.09,6535.62,5197.18,5315.77,7109.34,13582.96,11618.67,5773.81,5745.22,4621.43,3855.29,2335.16];

new Chart(document.getElementById('typeBar'), {
  type:'bar',
  data:{labels:months, datasets:[
    {label:'Unsalted',        data:unsalted, backgroundColor:'#D9A441', borderWidth:0},
    {label:'Portion control', data:pc,       backgroundColor:'#378ADD', borderWidth:0},
    {label:'Salted',          data:salted,   backgroundColor:'#1D9E75', borderWidth:0},
    {label:'Bakery / pastry', data:bakery,   backgroundColor:'#534AB7', borderWidth:0},
  ]},
  options: stackOpts
});

new Chart(document.getElementById('catDonut'), {
  type:'doughnut',
  data:{labels:['Unsalted 64%','Portion control 22%','Salted 10%','Bakery / pastry 4%'],
    datasets:[{data:[1227275,422691,191137,78407], backgroundColor:['#D9A441','#378ADD','#1D9E75','#534AB7'], borderWidth:3, borderColor:'#FFFFFF'}]},
  options:{responsive:true, maintainAspectRatio:false, cutout:'60%',
    plugins:{legend:{position:'right',labels:{color:'#6B7280',font:{size:11},boxWidth:10,padding:10}},
    tooltip:{callbacks:{label:ctx=>` ${fmt(ctx.parsed)}`}}}}
});

const butterBrandMonthly = {
  'Western Star':[35272.62,34974.67,34553.93,35091.50,39061.63,42491.17,34749.56,33247.83,36101.84,34744.56,41943.34,27294.84],
  'Devondale':   [26362.03,24020.78,22806.64,32195.71,32504.86,27115.34,27144.30,27085.50,31982.98,28404.54,31745.42,19367.78],
  'Unbranded':   [23254.64,28204.94,30191.04,27372.15,28190.10,26493.98,20341.69,20725.20,23714.00,21821.64,14803.08,18359.40],
  'Pauls':       [23909.06,18312.93,17648.55,18187.89,17741.15,24595.62,21879.63,22236.77,28149.04,23433.02,28073.56,17492.24],
  'Pepe Saya':   [8621.75,9158.07,10285.14,9675.12,14672.16,15283.58,12519.24,11119.98,12109.48,8746.71,9849.88,5895.98],
  'Anchor':      [7487.03,9181.47,9027.95,10212.54,9543.35,10191.06,6568.37,7799.48,6270.69,6494.36,6991.95,5511.23],
  'Other':       [31917.17,31905.04,29792.57,29157.72,30771.50,41946.98,37165.68,29391.41,34264.96,30099.59,35989.23,28496.61],
};
new Chart(document.getElementById('brandBar'), {
  type:'bar',
  data:{labels:months, datasets:Object.entries(butterBrandMonthly).map(([label,data],i)=>({label, data, backgroundColor:['#D9A441','#378ADD','#9CA3AF','#1D9E75','#534AB7','#D85A30','#D1D5DB'][i], borderWidth:0}))},
  options: stackOpts
});

buildTable('unsaltedTable', [
  {name:'Western Star', gmv:304556, color:'#D9A441'},
  {name:'Pauls',        gmv:244834, color:'#1D9E75'},
  {name:'Devondale',    gmv:225563, color:'#378ADD'},
  {name:'Unbranded',    gmv:192204, color:'#9CA3AF'},
  {name:'Anchor',       gmv:68518,  color:'#D85A30'},
  {name:'NZMP',         gmv:41123,  color:'#888780'},
  {name:'Other',        gmv:150477, color:'#D1D5DB'},
]);
buildTable('bpcTable', [
  {name:'Tatura',       gmv:93647, color:'#2563EB'},
  {name:'Pepe Saya',    gmv:91540, color:'#534AB7'},
  {name:'Western Star', gmv:64580, color:'#D9A441'},
  {name:'Devondale',    gmv:42787, color:'#378ADD'},
  {name:'Unbranded',    gmv:36413, color:'#9CA3AF'},
  {name:'Lescure',      gmv:31236, color:'#B4894A'},
  {name:'Other',        gmv:62488, color:'#D1D5DB'},
]);
buildTable('saltedTable', [
  {name:'Devondale',    gmv:62385, color:'#378ADD'},
  {name:'Western Star', gmv:60392, color:'#D9A441'},
  {name:'Unbranded',    gmv:48307, color:'#9CA3AF'},
  {name:'Pauls',        gmv:11837, color:'#1D9E75'},
  {name:'Westgold',     gmv:2874,  color:'#639922'},
  {name:'Burro Zanasi', gmv:1935,  color:'#BA7517'},
  {name:'Other',        gmv:3407,  color:'#D1D5DB'},
]);
buildTable('bakeryTable', [
  {name:'Fonterra',     gmv:28572, color:'#0891B2'},
  {name:'Lescure',      gmv:18425, color:'#B4894A'},
  {name:'Careme',       gmv:12011, color:'#7C3AED'},
  {name:'Anchor',       gmv:7468,  color:'#D85A30'},
  {name:'Unbranded',    gmv:6548,  color:'#9CA3AF'},
  {name:'Mainland',     gmv:2113,  color:'#D97706'},
  {name:'Other',        gmv:3270,  color:'#D1D5DB'},
]);

// ════════════ MARGARINE ════════════
const mMarg  = [6237.37,6206.95,6108.30,6672.97,5985.83,7806.70,6900.18,5858.20,7248.78,6531.10,7128.06,6234.04];
const mBlend = [5453.28,6552.14,5209.67,5602.57,4696.07,5822.15,4634.89,4021.52,4406.55,3383.41,3355.10,2161.05];
const mPlant = [738.55,710.14,1042.20,763.16,802.56,1039.21,1049.91,984.55,1404.25,1678.01,2039.78,2188.91];
const mPC    = [1245.79,1369.65,1211.64,1725.64,1399.05,1341.57,987.72,780.54,246.35,146.53,94.53,115.02];

new Chart(document.getElementById('mTypeBar'), {
  type:'bar',
  data:{labels:months, datasets:[
    {label:'Margarine',           data:mMarg,  backgroundColor:'#E0A82E', borderWidth:0},
    {label:'Blends',              data:mBlend, backgroundColor:'#D85A30', borderWidth:0},
    {label:'Plant-based spreads', data:mPlant, backgroundColor:'#1D9E75', borderWidth:0},
    {label:'Portion control',     data:mPC,    backgroundColor:'#378ADD', borderWidth:0},
  ]},
  options: stackOpts
});

new Chart(document.getElementById('mDonut'), {
  type:'doughnut',
  data:{labels:['Margarine 50%','Blends 35%','Plant-based 9%','Portion control 7%'],
    datasets:[{data:[78918,55298,14441,10664], backgroundColor:['#E0A82E','#D85A30','#1D9E75','#378ADD'], borderWidth:3, borderColor:'#FFFFFF'}]},
  options:{responsive:true, maintainAspectRatio:false, cutout:'60%',
    plugins:{legend:{position:'right',labels:{color:'#6B7280',font:{size:11},boxWidth:10,padding:10}},
    tooltip:{callbacks:{label:ctx=>` ${fmt(ctx.parsed)}`}}}}
});

const margBrandMonthly = {
  'Lurpak':         [2787.64,3797.56,3546.23,3649.68,2845.92,3738.96,2968.51,1795.44,2429.51,1409.02,1416.66,731.83],
  'Miracle':        [1051.77,1314.29,1244.69,1383.82,1082.38,1497.75,1163.07,1997.57,5006.87,4650.05,4778.71,3935.07],
  'Western Star':   [2665.64,2754.58,1663.44,1952.89,1850.15,2083.19,1633.63,2226.08,1977.04,1974.39,1938.44,1429.22],
  'Sunlit Plains':  [3717.30,3413.77,3556.10,3929.79,2391.31,2618.22,1905.99,973.92,0.00,0.00,0.00,0.00],
  'Unbranded':      [1299.95,1382.85,764.27,1018.25,1766.78,3649.48,3265.32,2045.47,397.45,362.69,550.10,708.12],
  "Mrs McGregor's": [765.30,778.36,925.04,1024.35,1158.58,772.98,1009.76,1197.79,1647.76,1581.08,1646.00,1440.41],
  'Other':          [1387.39,1397.47,1872.04,1805.56,1788.39,1649.05,1626.42,1408.54,1847.30,1761.82,2287.56,2454.37],
};
new Chart(document.getElementById('mBrandBar'), {
  type:'bar',
  data:{labels:months, datasets:Object.entries(margBrandMonthly).map(([label,data],i)=>({label, data, backgroundColor:['#1D4ED8','#E0A82E','#D9A441','#B4894A','#9CA3AF','#639922','#D1D5DB'][i], borderWidth:0}))},
  options: stackOpts
});

buildTable('margTable', [
  {name:'Miracle',         gmv:29106, color:'#E0A82E'},
  {name:'Sunlit Plains',   gmv:22506, color:'#B4894A'},
  {name:"Mrs McGregor's",  gmv:13947, color:'#639922'},
  {name:'Unbranded',       gmv:9644,  color:'#9CA3AF'},
  {name:'Meadow Lea',      gmv:1695,  color:'#534AB7'},
  {name:'Peerless Foods',  gmv:950,   color:'#888780'},
  {name:'Other',           gmv:1069,  color:'#D1D5DB'},
]);
buildTable('mBlendTable', [
  {name:'Lurpak',       gmv:31117, color:'#1D4ED8'},
  {name:'Western Star', gmv:24149, color:'#D9A441'},
  {name:'Ballantyne',   gmv:33,    color:'#B4B2A9'},
]);
buildTable('plantTable', [
  {name:'Nuttelex',     gmv:12702, color:'#1D9E75'},
  {name:'Golden Award', gmv:1735,  color:'#BA7517'},
  {name:'Tablelands',   gmv:5,     color:'#B4B2A9'},
]);
buildTable('mpcTable', [
  {name:'Unbranded',    gmv:7567,  color:'#9CA3AF'},
  {name:'Meadow Lea',   gmv:2963,  color:'#534AB7'},
  {name:'Flora',        gmv:135,   color:'#D85A30'},
]);
</script>
</body>
</html>
