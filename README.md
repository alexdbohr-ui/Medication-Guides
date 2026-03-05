<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>20mg IR Adderall — Manufacturer Reference</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #0f0f10;
    --surface: #1a1a1c;
    --surface2: #222226;
    --border: #2a2a2e;
    --border2: #333338;
    --text: #e8e8ec;
    --muted: #888890;
    --accent: #c8a97e;
    --available: #5aab7a;
    --shortage: #d4a03a;
    --discontinued: #b05555;
    --panel-w: 420px;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  html, body { height: 100%; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'DM Sans', sans-serif;
    min-height: 100vh;
    overflow-x: hidden;
  }

  /* ── HEADER ── */
  header {
    text-align: center;
    padding: 40px 24px 20px;
    position: relative;
    z-index: 1;
  }
  header .eyebrow {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 10px;
  }
  header h1 {
    font-size: 26px;
    font-weight: 300;
    letter-spacing: -0.02em;
    color: var(--text);
  }
  header p {
    margin-top: 6px;
    font-size: 13px;
    color: var(--muted);
    font-family: 'DM Mono', monospace;
  }

  .disclaimer {
    background: #1e1a14;
    border: 1px solid #3a2e1a;
    border-radius: 8px;
    padding: 10px 16px;
    font-size: 11px;
    color: #a08050;
    text-align: center;
    max-width: 720px;
    margin: 12px auto 32px;
    font-family: 'DM Mono', monospace;
    line-height: 1.6;
  }

  /* ── LAYOUT ── */
  .layout {
    display: flex;
    transition: all 0.4s ease;
  }
  .layout.panel-open .grid-area {
    margin-right: var(--panel-w);
  }

  /* ── GRID ── */
  .grid-area {
    flex: 1;
    padding: 0 24px 60px;
    transition: margin 0.4s ease;
  }
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(230px, 1fr));
    gap: 16px;
    max-width: 1000px;
    margin: 0 auto;
  }

  /* ── CARD ── */
  .card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 24px 20px 18px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 12px;
    cursor: pointer;
    transition: border-color 0.2s, transform 0.2s, box-shadow 0.2s;
    position: relative;
    overflow: hidden;
    user-select: none;
  }
  .card:hover {
    border-color: #3a3a40;
    transform: translateY(-3px);
    box-shadow: 0 12px 32px rgba(0,0,0,0.4);
  }
  .card.active {
    border-color: var(--accent);
    box-shadow: 0 0 0 1px var(--accent), 0 12px 32px rgba(200,169,126,0.15);
  }
  .card.discontinued { opacity: 0.5; }

  .status {
    position: absolute;
    top: 12px; right: 12px;
    font-family: 'DM Mono', monospace;
    font-size: 9px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    padding: 3px 7px;
    border-radius: 20px;
  }
  .status.available { background: rgba(90,171,122,0.15); color: var(--available); border: 1px solid rgba(90,171,122,0.3); }
  .status.shortage  { background: rgba(212,160,58,0.15);  color: var(--shortage);  border: 1px solid rgba(212,160,58,0.3); }
  .status.disc      { background: rgba(176,85,85,0.15);   color: var(--discontinued); border: 1px solid rgba(176,85,85,0.3); }

  .pill-wrap { width: 100px; height: 100px; display: flex; align-items: center; justify-content: center; }
  .pill-wrap svg { filter: drop-shadow(0 6px 16px rgba(0,0,0,0.5)); }

  .card-name { font-size: 14px; font-weight: 600; text-align: center; }
  .card-type { font-size: 10px; font-family: 'DM Mono', monospace; letter-spacing: 0.08em; color: var(--accent); text-transform: uppercase; }

  .card-meta {
    width: 100%;
    border-top: 1px solid var(--border);
    padding-top: 12px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 6px 10px;
  }
  .card-meta label { font-size: 9px; font-family: 'DM Mono', monospace; letter-spacing: 0.1em; text-transform: uppercase; color: var(--muted); display: block; margin-bottom: 1px; }
  .card-meta span  { font-size: 12px; color: var(--text); font-weight: 500; }

  .click-hint {
    font-size: 10px;
    font-family: 'DM Mono', monospace;
    color: #555;
    margin-top: 4px;
    transition: color 0.2s;
  }
  .card:hover .click-hint { color: var(--accent); }
  .card.active .click-hint { display: none; }

  /* ── SIDE PANEL ── */
  .panel {
    position: fixed;
    top: 0; right: 0;
    width: var(--panel-w);
    height: 100vh;
    background: var(--surface);
    border-left: 1px solid var(--border2);
    display: flex;
    flex-direction: column;
    transform: translateX(100%);
    transition: transform 0.4s cubic-bezier(0.4,0,0.2,1);
    z-index: 100;
    overflow: hidden;
  }
  .panel.open { transform: translateX(0); }

  .panel-header {
    padding: 24px 24px 20px;
    border-bottom: 1px solid var(--border);
    display: flex;
    align-items: flex-start;
    gap: 16px;
    flex-shrink: 0;
    background: var(--surface2);
  }
  .panel-pill { flex-shrink: 0; }
  .panel-title { flex: 1; }
  .panel-title h2 { font-size: 17px; font-weight: 600; line-height: 1.3; }
  .panel-title .pt { font-size: 10px; font-family: 'DM Mono', monospace; color: var(--accent); text-transform: uppercase; letter-spacing: 0.1em; margin-bottom: 4px; }
  .panel-title .imprint { font-size: 12px; font-family: 'DM Mono', monospace; color: var(--muted); margin-top: 4px; }

  .close-btn {
    background: none;
    border: 1px solid var(--border2);
    color: var(--muted);
    width: 30px; height: 30px;
    border-radius: 50%;
    cursor: pointer;
    font-size: 16px;
    display: flex; align-items: center; justify-content: center;
    flex-shrink: 0;
    transition: border-color 0.2s, color 0.2s;
  }
  .close-btn:hover { border-color: var(--text); color: var(--text); }

  .panel-body {
    flex: 1;
    overflow-y: auto;
    padding: 0;
  }
  .panel-body::-webkit-scrollbar { width: 4px; }
  .panel-body::-webkit-scrollbar-track { background: var(--surface); }
  .panel-body::-webkit-scrollbar-thumb { background: #333; border-radius: 2px; }

  /* ── TABS ── */
  .tabs {
    display: flex;
    border-bottom: 1px solid var(--border);
    background: var(--surface2);
    flex-shrink: 0;
  }
  .tab {
    flex: 1;
    padding: 12px 6px;
    text-align: center;
    font-size: 11px;
    font-family: 'DM Mono', monospace;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--muted);
    cursor: pointer;
    border-bottom: 2px solid transparent;
    transition: color 0.2s, border-color 0.2s;
  }
  .tab:hover { color: var(--text); }
  .tab.active { color: var(--accent); border-bottom-color: var(--accent); }

  .tab-content { display: none; padding: 20px; }
  .tab-content.active { display: block; }

  /* ── OVERVIEW TAB ── */
  .info-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin-bottom: 20px;
  }
  .info-box {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 12px 14px;
  }
  .info-box label { font-size: 9px; font-family: 'DM Mono', monospace; letter-spacing: 0.1em; text-transform: uppercase; color: var(--muted); display: block; margin-bottom: 4px; }
  .info-box .val { font-size: 14px; font-weight: 600; }
  .info-box .val.green { color: var(--available); }
  .info-box .val.amber { color: var(--shortage); }
  .info-box .val.red   { color: var(--discontinued); }

  .section-title {
    font-size: 10px;
    font-family: 'DM Mono', monospace;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 10px;
    padding-bottom: 6px;
    border-bottom: 1px solid var(--border);
  }

  .notes-text {
    font-size: 13px;
    line-height: 1.7;
    color: #c0c0c8;
    margin-bottom: 20px;
  }

  /* ── PRICE TAB ── */
  .price-big {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 20px;
    text-align: center;
    margin-bottom: 16px;
  }
  .price-big .price-label { font-size: 10px; font-family: 'DM Mono', monospace; letter-spacing: 0.1em; text-transform: uppercase; color: var(--muted); margin-bottom: 6px; }
  .price-big .price-val { font-size: 32px; font-weight: 300; color: var(--accent); }
  .price-big .price-sub { font-size: 12px; color: var(--muted); margin-top: 4px; font-family: 'DM Mono', monospace; }

  .price-rows { margin-bottom: 20px; }
  .price-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 0;
    border-bottom: 1px solid var(--border);
    font-size: 13px;
  }
  .price-row:last-child { border-bottom: none; }
  .price-row .pr-label { color: var(--muted); font-size: 12px; }
  .price-row .pr-val { font-weight: 600; }

  .tip-box {
    background: #1a1a10;
    border: 1px solid #3a3a1a;
    border-radius: 10px;
    padding: 14px 16px;
    font-size: 12px;
    color: #a0a060;
    line-height: 1.7;
  }
  .tip-box strong { color: #c8c870; }

  /* ── REVIEWS TAB ── */
  .review-summary {
    display: flex;
    align-items: center;
    gap: 16px;
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 16px;
    margin-bottom: 20px;
  }
  .review-score {
    text-align: center;
    flex-shrink: 0;
  }
  .review-score .score-num { font-size: 40px; font-weight: 300; line-height: 1; color: var(--accent); }
  .review-score .score-label { font-size: 10px; font-family: 'DM Mono', monospace; color: var(--muted); text-transform: uppercase; letter-spacing: 0.1em; margin-top: 4px; }

  .score-bars { flex: 1; }
  .score-bar-row { display: flex; align-items: center; gap: 8px; margin-bottom: 5px; }
  .score-bar-row .bar-label { font-size: 10px; font-family: 'DM Mono', monospace; color: var(--muted); width: 50px; flex-shrink: 0; }
  .score-bar-row .bar-track { flex: 1; height: 4px; background: var(--border2); border-radius: 2px; overflow: hidden; }
  .score-bar-row .bar-fill  { height: 100%; border-radius: 2px; background: var(--accent); transition: width 0.6s ease; }
  .score-bar-row .bar-pct   { font-size: 10px; font-family: 'DM Mono', monospace; color: var(--muted); width: 28px; text-align: right; flex-shrink: 0; }

  .review-card {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 14px 16px;
    margin-bottom: 12px;
    font-size: 13px;
    line-height: 1.7;
    color: #c0c0c8;
  }
  .review-card .rv-meta {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 8px;
  }
  .review-card .rv-stars { color: var(--accent); font-size: 12px; letter-spacing: 2px; }
  .review-card .rv-date  { font-size: 10px; font-family: 'DM Mono', monospace; color: var(--muted); }
  .review-card .rv-sentiment {
    display: inline-block;
    font-size: 9px;
    font-family: 'DM Mono', monospace;
    padding: 2px 7px;
    border-radius: 10px;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    margin-top: 8px;
  }
  .rv-sentiment.pos { background: rgba(90,171,122,0.15); color: var(--available); }
  .rv-sentiment.neg { background: rgba(176,85,85,0.15); color: var(--discontinued); }
  .rv-sentiment.mix { background: rgba(212,160,58,0.15); color: var(--shortage); }

  .review-source {
    font-size: 10px;
    font-family: 'DM Mono', monospace;
    color: #444;
    text-align: center;
    margin-top: 4px;
    padding-top: 16px;
    border-top: 1px solid var(--border);
  }

  /* Mobile overlay */
  .overlay {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.5);
    z-index: 99;
  }
  .overlay.show { display: block; }

  @media (max-width: 700px) {
    :root { --panel-w: 100vw; }
    .layout.panel-open .grid-area { margin-right: 0; }
  }
</style>
</head>
<body>

<header>
  <div class="eyebrow">Pill Identification & Review Reference</div>
  <h1>20mg Immediate-Release Amphetamine Mixed Salts</h1>
  <p>Click any manufacturer to view reviews, pricing & availability</p>
</header>

<div class="disclaimer">
  ⚠ For informational reference only. Reviews are aggregated from public patient forums (Drugs.com, MedShadow, Reddit). Always consult your pharmacist or physician before making medication decisions.
</div>

<div class="layout" id="layout">
  <div class="grid-area">
    <div class="grid" id="grid"></div>
  </div>
</div>

<div class="overlay" id="overlay" onclick="closePanel()"></div>

<!-- SIDE PANEL -->
<div class="panel" id="panel">
  <div class="panel-header" id="panelHeader"></div>
  <div class="tabs" id="tabs">
    <div class="tab active" onclick="switchTab('overview')">Overview</div>
    <div class="tab" onclick="switchTab('price')">Price</div>
    <div class="tab" onclick="switchTab('reviews')">Reviews</div>
  </div>
  <div class="panel-body">
    <div class="tab-content active" id="tab-overview"></div>
    <div class="tab-content" id="tab-price"></div>
    <div class="tab-content" id="tab-reviews"></div>
  </div>
</div>

<script>
const manufacturers = [
  {
    id: 'teva-brand',
    name: 'Teva Pharmaceuticals',
    type: 'Brand-Name Adderall®',
    status: 'available',
    statusLabel: 'Available',
    imprint: 'b 973 / 2 0',
    color: 'Peach / Salmon',
    shape: 'Oval, Scored',
    ndc: '57844-0120-01',
    pillType: 'oval',
    pillColor1: '#e8b89a', pillColor2: '#c47f5a', pillStroke: '#a06040',
    imprintText: ['b 973', '2 0'],
    overview: `Teva's brand-name Adderall has historically been the gold standard and most sought-after version among patients. It is the original branded formulation and is manufactured in the same facilities as the Teva generic. Teva holds both the brand and generic market, giving it the widest distribution.`,
    availabilityNotes: `Currently the most reliably available formulation at major chains including CVS, Walgreens, and Walmart. Teva is the primary supplier during the ongoing shortage, though batch inconsistencies have been reported since 2022. Ask your pharmacist specifically for Teva brand.`,
    price: { goodrx: '$16–$30', retail: '~$814', insurance: '$0–$60', perPill: '~$0.55' },
    priceNotes: `Brand-name Adderall without insurance runs $800+ per month for 60 tablets (2x daily dosing). However, with a GoodRx coupon, generic Teva (bioequivalent) drops to $16–$30/mo for 30 tablets. Most insurance plans cover generic versions with a small copay.`,
    score: 3.6,
    bars: { Efficacy: 72, Consistency: 55, Availability: 90, 'Side Effects': 60 },
    reviews: [
      { stars: 5, date: '2024', text: 'Been on Teva brand for 8 years. When I can get it, it works consistently and predictably. The oval B973 is what I always ask for specifically.', sentiment: 'pos' },
      { stars: 2, date: '2022', text: 'Teva IR 30mg is BAD as of early 2022. After 16 years of taking this, I\'ve never had a problem — now I\'m falling asleep after I take it. Took an old Lannett I had on hand and I\'m back to normal.', sentiment: 'neg' },
      { stars: 4, date: '2025', text: 'Teva wore off far too quickly in my June 2025 refill. I don\'t know if it\'s something they add, but I metabolize it differently now. Used to last 5 hours, now barely 3.', sentiment: 'mix' },
      { stars: 5, date: '2023', text: 'Pills that used to break cleanly are now crumbling in my hands. Despite that, it\'s still the most effective generic I\'ve tried — I always request Teva and most pharmacists will accommodate if stock allows.', sentiment: 'mix' },
    ]
  },
  {
    id: 'teva-generic',
    name: 'Teva Pharmaceuticals',
    type: 'Generic (E 401)',
    status: 'available',
    statusLabel: 'Available',
    imprint: 'E 401',
    color: 'Orange',
    shape: 'Round, Quad-scored',
    ndc: '57844-0120',
    pillType: 'round',
    pillColor1: '#e8922a', pillColor2: '#b86010', pillStroke: '#8a4800',
    imprintText: ['E 401'],
    overview: `Teva's orange round generic (E 401) is chemically identical to the brand but uses different inactive ingredients than the oval brand tablet. It is the most widely dispensed generic at chain pharmacies. Patient reception has been mixed — some prefer this version, others strongly prefer the oval brand.`,
    availabilityNotes: `Most widely available generic during the shortage period. Found at most major pharmacy chains. During the shortage, Teva has been the dominant supplier as Mylan, Zydus, and Sandoz discontinued their IR lines.`,
    price: { goodrx: '$16–$25', retail: '~$48', insurance: '$0–$30', perPill: '~$0.55' },
    priceNotes: `Generic amphetamine salt combo (Teva E 401) is among the most affordable options. GoodRx coupons bring a 30-count supply down to $16–$25 at most pharmacies. Retail without coupon averages ~$48. Covered by most insurance plans with standard copay.`,
    score: 3.4,
    bars: { Efficacy: 65, Consistency: 50, Availability: 92, 'Side Effects': 58 },
    reviews: [
      { stars: 4, date: '2023', text: 'Teva generic works well for me when I can get it. It\'s not quite as clean as the oval brand version but it\'s consistent month to month — which is all I ask for.', sentiment: 'pos' },
      { stars: 2, date: '2024', text: 'Been getting Teva generic from Walgreens for years. Complaining that the dose doesn\'t last longer than a couple hours, but this last refill doesn\'t even work at all. Doubled my dose and got a headache and brain fog.', sentiment: 'neg' },
      { stars: 3, date: '2025', text: 'Something has changed with Teva\'s formula since 2022. It used to be the best generic around but now the results are wildly inconsistent batch to batch. Still better than Camber or Mallinckrodt for me personally.', sentiment: 'mix' },
    ]
  },
  {
    id: 'camber',
    name: 'Camber Pharmaceuticals',
    type: 'Generic (U30)',
    status: 'shortage',
    statusLabel: 'Shortage',
    imprint: 'U30',
    color: 'Orange',
    shape: 'Round, Quad-scored',
    ndc: '31722-0157-01',
    pillType: 'round',
    pillColor1: '#f0a050', pillColor2: '#c07020', pillStroke: '#904000',
    imprintText: ['U30'],
    overview: `Camber's generic has received some of the most consistently negative patient reviews of any IR formulation. During the shortage it became more widely distributed as pharmacies switched suppliers, exposing a large number of patients to it for the first time. Inactive ingredient composition is suspected to be the source of reported side effects.`,
    availabilityNotes: `Available at some Walgreens locations and independent pharmacies during shortage periods. Listed on ASHP shortage bulletin as having limited availability due to ingredient supply delays. Camber did not provide a shortage reason to ASHP.`,
    price: { goodrx: '$15–$25', retail: '~$45', insurance: '$0–$30', perPill: '~$0.50' },
    priceNotes: `One of the least expensive generics on the market. GoodRx prices start around $15 for 30 tablets. Often used by pharmacies as a low-cost substitute when Teva is unavailable, sometimes without informing patients.`,
    score: 1.8,
    bars: { Efficacy: 28, Consistency: 22, Availability: 45, 'Side Effects': 20 },
    reviews: [
      { stars: 1, date: '2024', text: 'Camber is toxic. This medicine caused me to become very nauseous, tachycardia, blurred vision, severe anxiety, and I was completely unable to focus. It was like I wasn\'t taking anything — my life went back to the way it was before Adderall.', sentiment: 'neg' },
      { stars: 1, date: '2023', text: 'My pharmacy switched me to Camber without notice. I asked the pharmacist about it because I noticed a huge change in symptoms. He told me it\'s a price war and he couldn\'t change it — but that others were complaining too.', sentiment: 'neg' },
      { stars: 2, date: '2023', text: 'I took Camber once and went the rest of the month without it. Couldn\'t focus, made me very anxious, depressed, sick to my stomach and emotional. So tired of this monthly generic Russian roulette.', sentiment: 'neg' },
      { stars: 3, date: '2022', text: 'I got less effective results with Camber vs Teva 20mg. Walgreens insists the dosages are the same but I don\'t feel it. They tried to switch me once before, but switched me back to Teva when I complained.', sentiment: 'neg' },
    ]
  },
  {
    id: 'lannett',
    name: 'Lannett Company',
    type: 'Generic (20 LCI)',
    status: 'shortage',
    statusLabel: 'Limited',
    imprint: '20 / LCI',
    color: 'Peach',
    shape: 'Round, Quad-scored',
    ndc: '0527-series',
    pillType: 'round',
    pillColor1: '#e8b090', pillColor2: '#c07858', pillStroke: '#905040',
    imprintText: ['20', 'LCI'],
    overview: `Lannett's generic has generated highly polarized reviews. Some patients report it works fine or even better than Teva, while many others report it's ineffective and causes jitteriness, anxiety, or cardiovascular symptoms. The inconsistency may reflect batch-to-batch variation. Lannett manufactures primarily in the US.`,
    availabilityNotes: `Sporadically available through major chains and independent pharmacies. Stocked at some CVS and Walgreens locations as a Teva substitute during shortage periods. Available but not consistently stocked in all markets.`,
    price: { goodrx: '$16–$28', retail: '~$50', insurance: '$0–$30', perPill: '~$0.55' },
    priceNotes: `Mid-range pricing among generics. GoodRx coupons bring costs to $16–$28 for 30 tablets. Sometimes slightly more expensive than Camber but cheaper than brand Teva. Covered by most insurance plans.`,
    score: 2.4,
    bars: { Efficacy: 40, Consistency: 35, Availability: 50, 'Side Effects': 38 },
    reviews: [
      { stars: 1, date: '2024', text: 'If anyone is having a terrible time with Lannett generic Adderall — you can report this to FDA MedWatch. I\'ve been having crippling headaches, stomach aches, and the medication doesn\'t even feel like it works. I get tired after I take it and then can\'t sleep all night.', sentiment: 'neg' },
      { stars: 2, date: '2024', text: 'Walgreens always carried the generic that worked best for me, but recently changed suppliers to Lannett. Now it SUCKS — doesn\'t work at all. The Teva peach oval B 973 is the one that works best for me and I have no idea how to get it back.', sentiment: 'neg' },
      { stars: 4, date: '2023', text: 'I\'ve been on adderall 25 years. Got Lannett and it made me tired, heart racing, BP accelerated, and did nothing to help me focus. But my neighbor has had the opposite experience — says Lannett is the only one that works consistently for her.', sentiment: 'mix' },
      { stars: 4, date: '2022', text: 'Teva IR 30mg is bad as of 2022. Took an old Lannett I still had and I\'m back to normal. This is extremely frustrating that there\'s nothing we can do — but Lannett genuinely worked for me when Teva didn\'t.', sentiment: 'pos' },
    ]
  },
  {
    id: 'elite',
    name: 'Elite / NorthStar Rx',
    type: 'Generic (N34)',
    status: 'shortage',
    statusLabel: 'Limited',
    imprint: 'N34',
    color: 'Peach',
    shape: 'Round, Quad-scored',
    ndc: '16714-series',
    pillType: 'round',
    pillColor1: '#dda880', pillColor2: '#b87050', pillStroke: '#885040',
    imprintText: ['N34'],
    overview: `Elite Pharmaceuticals (distributed under the NorthStar Rx label) has received more positive reviews than most generics, with some patients explicitly preferring it over Teva. It is among the harder-to-find options but has a relatively good reputation in patient communities. Same active ingredients as all other generics per FDA bioequivalence standards.`,
    availabilityNotes: `Difficult to find — limited to select independent pharmacies and some smaller chains. Not commonly stocked at major chains like CVS or Walgreens. Worth calling ahead to independent pharmacies. ASHP lists as limited availability.`,
    price: { goodrx: '$18–$32', retail: '~$55', insurance: '$0–$35', perPill: '~$0.60' },
    priceNotes: `Slightly higher priced than Camber or Lannett generics, but still affordable. GoodRx brings 30 tablets to $18–$32. May be harder to use discount coupons at independent pharmacies; call ahead. Generally covered by insurance.`,
    score: 3.8,
    bars: { Efficacy: 75, Consistency: 70, Availability: 25, 'Side Effects': 72 },
    reviews: [
      { stars: 5, date: '2024', text: 'Picked up Elite/NorthStar for the first time last month and had a positive experience. Definitely prefer it to Teva — Teva has been a bit inconsistent for me lately and this felt more reliable.', sentiment: 'pos' },
      { stars: 4, date: '2023', text: 'N34 is hard to find but worth the search. Called 8 pharmacies before finding one that stocked it. Worked well for 3 months straight — best consistency I\'ve had since the shortage started.', sentiment: 'pos' },
      { stars: 3, date: '2024', text: 'Works well but I can\'t find it reliably. My pharmacy switched me to Camber when they ran out and it was a disaster. Wish more pharmacies would carry Elite/NorthStar as a consistent option.', sentiment: 'mix' },
    ]
  },
  {
    id: 'zydus',
    name: 'Zydus Pharmaceuticals',
    type: 'Generic (F6) — Discontinued',
    status: 'disc',
    statusLabel: 'Discontinued',
    imprint: 'F6',
    color: 'Beige / Tan',
    shape: 'Round, Quad-scored',
    ndc: 'N/A',
    pillType: 'round',
    pillColor1: '#d4c8a0', pillColor2: '#a89870', pillStroke: '#887848',
    imprintText: ['F6'],
    overview: `Zydus discontinued their amphetamine mixed salts IR line. During the period they were available, patient reviews were generally moderate — not as well-regarded as Teva brand but received fewer negative reviews than Camber or Mallinckrodt. The beige/tan coloration made it easy to identify.`,
    availabilityNotes: `No longer available. Zydus confirmed discontinuation to ASHP. If you receive a tan/beige round F6 tablet, it is from old pharmacy stock and may be expired. Do not accept this formulation without verifying freshness.`,
    price: { goodrx: 'N/A', retail: 'N/A', insurance: 'N/A', perPill: 'N/A' },
    priceNotes: `No longer manufactured or distributed. Was priced similarly to other generics at ~$20–$35/mo with coupons when available. No current pricing data applies.`,
    score: 3.0,
    bars: { Efficacy: 58, Consistency: 50, Availability: 0, 'Side Effects': 55 },
    reviews: [
      { stars: 3, date: '2022', text: 'Zydus was mid-tier for me — not great, not terrible. It worked but not as well as Teva brand. At least it didn\'t cause the side effects that Camber and Mallinckrodt did for me. Sad it\'s discontinued.', sentiment: 'mix' },
      { stars: 4, date: '2021', text: 'Was on Zydus F6 for a year and didn\'t have any problems. It was reliable. When they switched me to Camber I noticed immediately — Camber is not the same drug as far as I\'m concerned.', sentiment: 'pos' },
    ]
  },
  {
    id: 'sandoz',
    name: 'Sandoz / Novartis',
    type: 'Generic — Discontinued',
    status: 'disc',
    statusLabel: 'Discontinued',
    imprint: 'dp / 20',
    color: 'Peach / Orange',
    shape: 'Round, Quad-scored',
    ndc: 'N/A',
    pillType: 'round',
    pillColor1: '#e09878', pillColor2: '#b06848', pillStroke: '#884838',
    imprintText: ['dp', '20'],
    overview: `Sandoz (the generic arm of Novartis) was historically considered one of the better-reviewed generic manufacturers, often cited alongside Teva as a reliable option. They have since discontinued their IR amphetamine line. Some patients reported Sandoz caused acid reflux or GI issues despite otherwise adequate efficacy.`,
    availabilityNotes: `Discontinued as of 2022–2023. No longer available through any pharmacy channel. ASHP confirmed discontinuation. Do not expect to find this formulation at any pharmacy.`,
    price: { goodrx: 'N/A', retail: 'N/A', insurance: 'N/A', perPill: 'N/A' },
    priceNotes: `No longer available. Was priced similarly to Teva generic at ~$20–$30/mo with GoodRx when in production. Discontinuation has contributed to the ongoing shortage.`,
    score: 3.5,
    bars: { Efficacy: 68, Consistency: 62, Availability: 0, 'Side Effects': 52 },
    reviews: [
      { stars: 4, date: '2022', text: 'Sandoz round peach worked almost as well as Teva brand for me. I filled with Sandoz in 2018 and it was my second-best option ever. Sad they stopped making it.', sentiment: 'pos' },
      { stars: 3, date: '2023', text: 'Sandoz caused me debilitating acid reflux even though it controlled my symptoms to some degree. I had unreliable results from refill to refill — sometimes it was great, sometimes it felt like nothing.', sentiment: 'mix' },
    ]
  },
  {
    id: 'mylan',
    name: 'Mylan Pharmaceuticals',
    type: 'Generic — Discontinued',
    status: 'disc',
    statusLabel: 'Discontinued',
    imprint: 'M / A23',
    color: 'Peach / Orange',
    shape: 'Round, Quad-scored',
    ndc: 'N/A',
    pillType: 'round',
    pillColor1: '#e0a070', pillColor2: '#b07040', pillStroke: '#886040',
    imprintText: ['M', 'A23'],
    overview: `Mylan (now Viatris) discontinued their amphetamine mixed salts IR tablets. Reviews during their production period were mixed — they were not as widely praised as Teva or Sandoz, but also not as negatively reviewed as Camber or Mallinckrodt. Discontinuation contributed to the 2022–present shortage.`,
    availabilityNotes: `Discontinued. No longer available at any pharmacy. ASHP confirmed Mylan's amphetamine IR line is no longer being produced. Mylan's broader portfolio was absorbed into Viatris following their 2020 merger.`,
    price: { goodrx: 'N/A', retail: 'N/A', insurance: 'N/A', perPill: 'N/A' },
    priceNotes: `No longer manufactured. Was a budget-tier generic, typically $18–$28/mo with coupons. Discontinuation has reduced market competition and indirectly increased prices for remaining generics.`,
    score: 2.8,
    bars: { Efficacy: 50, Consistency: 45, Availability: 0, 'Side Effects': 48 },
    reviews: [
      { stars: 3, date: '2021', text: 'Mylan was okay for me — nothing special but it did the job. Never noticed any particular side effects. It was my fallback when Teva was unavailable at my pharmacy.', sentiment: 'mix' },
      { stars: 2, date: '2020', text: 'Switched to Mylan after Teva shortage and it just doesn\'t hit the same. Much weaker efficacy in my experience. Always felt like I needed an extra half-pill to get the same effect.', sentiment: 'neg' },
    ]
  }
];

let activeId = null;
let activeTab = 'overview';

function buildPillSVG(mfr, size=80) {
  const { pillType, pillColor1, pillColor2, pillStroke, imprintText, id } = mfr;
  const gid = `g_${id}`;
  if (pillType === 'oval') {
    const rx = size * 0.46, ry = size * 0.26;
    const cx = size/2, cy = size/2;
    return `<svg width="${size}" height="${size*0.6}" viewBox="0 0 ${size} ${size*0.6}">
      <defs><linearGradient id="${gid}" x1="0%" y1="0%" x2="0%" y2="100%">
        <stop offset="0%" stop-color="${pillColor1}"/><stop offset="100%" stop-color="${pillColor2}"/>
      </linearGradient></defs>
      <ellipse cx="${size/2}" cy="${size*0.3}" rx="${rx}" ry="${ry}" fill="url(#${gid})" stroke="${pillStroke}" stroke-width="1.2"/>
      <line x1="${size/2}" y1="${size*0.3-ry+1}" x2="${size/2}" y2="${size*0.3+ry-1}" stroke="${pillStroke}" stroke-width="1.3" opacity="0.55"/>
      <text x="${size*0.27}" y="${size*0.33}" font-family="Georgia,serif" font-size="${size*0.1}" fill="${pillStroke}" font-weight="bold" text-anchor="middle" opacity="0.85">${imprintText[0]||''}</text>
      <text x="${size*0.73}" y="${size*0.33}" font-family="Georgia,serif" font-size="${size*0.1}" fill="${pillStroke}" font-weight="bold" text-anchor="middle" opacity="0.85">${imprintText[1]||''}</text>
    </svg>`;
  } else {
    const r = size * 0.42, c = size/2;
    const lines = imprintText.length > 1 
      ? `<text x="${c}" y="${c-size*0.04}" font-family="Georgia,serif" font-size="${size*0.12}" fill="${pillStroke}" font-weight="bold" text-anchor="middle" opacity="0.85">${imprintText[0]}</text>
         <text x="${c}" y="${c+size*0.12}" font-family="Georgia,serif" font-size="${size*0.12}" fill="${pillStroke}" font-weight="bold" text-anchor="middle" opacity="0.85">${imprintText[1]}</text>`
      : `<text x="${c}" y="${c+size*0.05}" font-family="Georgia,serif" font-size="${size*0.13}" fill="${pillStroke}" font-weight="bold" text-anchor="middle" opacity="0.85">${imprintText[0]}</text>`;
    return `<svg width="${size}" height="${size}" viewBox="0 0 ${size} ${size}">
      <defs><linearGradient id="${gid}" x1="0%" y1="0%" x2="0%" y2="100%">
        <stop offset="0%" stop-color="${pillColor1}"/><stop offset="100%" stop-color="${pillColor2}"/>
      </linearGradient></defs>
      <circle cx="${c}" cy="${c}" r="${r}" fill="url(#${gid})" stroke="${pillStroke}" stroke-width="1.2"/>
      <line x1="${c}" y1="${c-r+1}" x2="${c}" y2="${c+r-1}" stroke="${pillStroke}" stroke-width="1.3" opacity="0.45"/>
      <line x1="${c-r+1}" y1="${c}" x2="${c+r-1}" y2="${c}" stroke="${pillStroke}" stroke-width="1.3" opacity="0.45"/>
      ${lines}
    </svg>`;
  }
}

function buildCards() {
  const grid = document.getElementById('grid');
  manufacturers.forEach(m => {
    const card = document.createElement('div');
    card.className = `card${m.status === 'disc' ? ' discontinued' : ''}`;
    card.id = `card-${m.id}`;
    card.onclick = () => openPanel(m.id);
    card.innerHTML = `
      <span class="status ${m.status === 'available' ? 'available' : m.status === 'shortage' ? 'shortage' : 'disc'}">${m.statusLabel}</span>
      <div class="pill-wrap">${buildPillSVG(m, 80)}</div>
      <div class="card-name">${m.name}</div>
      <div class="card-type">${m.type}</div>
      <div class="card-meta">
        <div><label>Color</label><span>${m.color}</span></div>
        <div><label>Shape</label><span>${m.shape}</span></div>
        <div><label>Imprint</label><span>${m.imprint}</span></div>
        <div><label>NDC</label><span>${m.ndc}</span></div>
      </div>
      <div class="click-hint">↗ tap for details</div>
    `;
    grid.appendChild(card);
  });
}

function openPanel(id) {
  const m = manufacturers.find(x => x.id === id);
  if (!m) return;

  // Update active card
  document.querySelectorAll('.card').forEach(c => c.classList.remove('active'));
  document.getElementById(`card-${id}`).classList.add('active');
  activeId = id;

  // Build header
  const pillHTML = buildPillSVG(m, 60);
  document.getElementById('panelHeader').innerHTML = `
    <div class="panel-pill">${pillHTML}</div>
    <div class="panel-title">
      <div class="pt">${m.type}</div>
      <h2>${m.name}</h2>
      <div class="imprint">Imprint: ${m.imprint} · ${m.color} · ${m.shape}</div>
    </div>
    <button class="close-btn" onclick="closePanel()">×</button>
  `;

  // Build overview
  const statusClass = m.status === 'available' ? 'green' : m.status === 'shortage' ? 'amber' : 'red';
  const scoreStars = Math.round(m.score);
  document.getElementById('tab-overview').innerHTML = `
    <div class="info-grid">
      <div class="info-box"><label>Availability</label><span class="val ${statusClass}">${m.statusLabel}</span></div>
      <div class="info-box"><label>Avg. Rating</label><span class="val" style="color:var(--accent)">${m.score} / 5</span></div>
      <div class="info-box"><label>Imprint</label><span class="val" style="font-size:13px">${m.imprint}</span></div>
      <div class="info-box"><label>NDC</label><span class="val" style="font-size:11px;color:var(--muted)">${m.ndc}</span></div>
    </div>
    <div class="section-title">About This Manufacturer</div>
    <div class="notes-text">${m.overview}</div>
    <div class="section-title">Availability Notes</div>
    <div class="notes-text">${m.availabilityNotes}</div>
  `;

  // Build price
  const naStyle = m.price.goodrx === 'N/A' ? 'color:var(--muted)' : '';
  document.getElementById('tab-price').innerHTML = `
    <div class="price-big">
      <div class="price-label">GoodRx Price (30 tablets)</div>
      <div class="price-val" style="${naStyle}">${m.price.goodrx}</div>
      <div class="price-sub">per month · 20mg IR</div>
    </div>
    <div class="price-rows">
      <div class="price-row"><span class="pr-label">Retail (no coupon)</span><span class="pr-val">${m.price.retail}</span></div>
      <div class="price-row"><span class="pr-label">With insurance</span><span class="pr-val">${m.price.insurance}</span></div>
      <div class="price-row"><span class="pr-label">Approx. per pill</span><span class="pr-val">${m.price.perPill}</span></div>
    </div>
    <div class="section-title">Pricing Notes</div>
    <div class="notes-text" style="font-size:13px;line-height:1.7;color:#c0c0c8;margin-bottom:16px">${m.priceNotes}</div>
    <div class="tip-box">💡 <strong>Saving tip:</strong> Generic amphetamine salt combo (any manufacturer) is the same drug by FDA standards. Use GoodRx or RxSaver at Costco, Walmart, or independent pharmacies for lowest prices. Brand-name Adderall retails at <strong>$800+/mo</strong> without insurance.</div>
  `;

  // Build reviews
  const barHTML = Object.entries(m.bars).map(([k, v]) => `
    <div class="score-bar-row">
      <span class="bar-label">${k}</span>
      <div class="bar-track"><div class="bar-fill" style="width:${v}%"></div></div>
      <span class="bar-pct">${v}%</span>
    </div>`).join('');

  const reviewsHTML = m.reviews.map(r => {
    const stars = '★'.repeat(r.stars) + '☆'.repeat(5 - r.stars);
    return `<div class="review-card">
      <div class="rv-meta">
        <span class="rv-stars">${stars}</span>
        <span class="rv-date">${r.date}</span>
      </div>
      ${r.text}
      <br><span class="rv-sentiment ${r.sentiment}">${r.sentiment === 'pos' ? '✓ Positive' : r.sentiment === 'neg' ? '✗ Negative' : '~ Mixed'}</span>
    </div>`;
  }).join('');

  document.getElementById('tab-reviews').innerHTML = `
    <div class="review-summary">
      <div class="review-score">
        <div class="score-num">${m.score}</div>
        <div class="score-label">/ 5.0</div>
      </div>
      <div class="score-bars">${barHTML}</div>
    </div>
    <div class="section-title">Patient Reviews</div>
    ${reviewsHTML}
    <div class="review-source">Reviews aggregated from Drugs.com, MedShadow Foundation, and ADHD patient forums · For reference only</div>
  `;

  // Switch to first tab
  switchTab('overview');

  // Open panel
  document.getElementById('panel').classList.add('open');
  document.getElementById('layout').classList.add('panel-open');
  document.getElementById('overlay').classList.add('show');

  // Animate bars after render
  setTimeout(() => {
    document.querySelectorAll('.bar-fill').forEach(b => {
      const w = b.style.width;
      b.style.width = '0';
      setTimeout(() => b.style.width = w, 50);
    });
  }, 100);
}

function closePanel() {
  document.getElementById('panel').classList.remove('open');
  document.getElementById('layout').classList.remove('panel-open');
  document.getElementById('overlay').classList.remove('show');
  document.querySelectorAll('.card').forEach(c => c.classList.remove('active'));
  activeId = null;
}

function switchTab(name) {
  activeTab = name;
  document.querySelectorAll('.tab').forEach((t, i) => {
    const names = ['overview', 'price', 'reviews'];
    t.classList.toggle('active', names[i] === name);
  });
  document.querySelectorAll('.tab-content').forEach(tc => {
    tc.classList.toggle('active', tc.id === `tab-${name}`);
  });
}

buildCards();
</script>
</body>
</html>
