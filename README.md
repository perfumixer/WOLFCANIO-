<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>WOLFCANIO Perfume House</title>
<meta name="description" content="WOLFCANIO is a Dubai perfume house. Every scent starts with oil.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,500;0,600;1,500&amp;family=Manrope:wght@400;600;700&amp;display=swap" rel="stylesheet">
<style>
/* Plan: ink pages with gold accents, a serif display over a plain sans body, one column rhythm that stacks on phones. */
:root {
  --ink: #0D0B09;
  --ink-2: #15110D;
  --ink-3: #1E1914;
  --gold: #C9A96A;
  --gold-hi: #E8D3A0;
  --gold-dk: #8A6E3F;
  --sand: #EDE4D3;
  --mist: #A39A8C;
  --line: rgba(237, 228, 211, 0.12);
  --line-2: rgba(237, 228, 211, 0.22);
  --serif: "Cormorant Garamond", Georgia, "Times New Roman", serif;
  --sans: Manrope, Arial, Helvetica, sans-serif;
  --gutter: clamp(20px, 4.4vw, 64px);
  color-scheme: dark;
}
* { box-sizing: border-box; }
html { background: var(--ink); scroll-behavior: smooth; }
body { margin: 0; background: var(--ink); color: var(--sand); font-family: var(--sans); font-size: 16px; line-height: 1.55; -webkit-font-smoothing: antialiased; }
a { color: inherit; text-decoration: none; }
button, input, select { font: inherit; color: inherit; }
button { cursor: pointer; }
img { display: block; max-width: 100%; height: auto; }
p { margin: 0; }
h1, h2, h3, h4 { font-family: var(--serif); font-weight: 500; margin: 0; line-height: 1.05; text-wrap: balance; }
:focus-visible { outline: 2px solid var(--gold-hi); outline-offset: 3px; }
section[id] { scroll-margin-top: 110px; }

/* Layout helpers */
.wrap { padding-left: var(--gutter); padding-right: var(--gutter); }
.section { padding: 112px var(--gutter); }
.section.first { padding-top: 72px; }
.page-head { padding: 72px var(--gutter) 0; }
.page-head h1 { font-size: clamp(48px, 7vw, 84px); margin-top: 14px; }
.page-head + .section { padding-top: 40px; }
.section h2 { font-size: clamp(40px, 5vw, 60px); margin-top: 14px; }
.head { display: flex; justify-content: space-between; align-items: flex-end; gap: 32px; flex-wrap: wrap; margin-bottom: 48px; }
.eyebrow { margin: 0; font-size: 12px; letter-spacing: 0.3em; text-transform: uppercase; color: var(--gold); }
.lead { margin-top: 18px; font-size: 18px; line-height: 1.7; color: var(--mist); max-width: 56ch; }
.view { display: none; }
.view.on { display: block; }

/* Buttons */
.btn { display: inline-flex; align-items: center; justify-content: center; height: 52px; padding: 0 26px; border-radius: 999px; border: 1px solid var(--gold); background: var(--gold); color: var(--ink); font-weight: 700; font-size: 13px; letter-spacing: 0.1em; text-transform: uppercase; text-align: center; }
.btn:hover { background: var(--gold-hi); border-color: var(--gold-hi); }
.btn.ghost { background: transparent; color: var(--sand); border-color: var(--line-2); }
.btn.ghost:hover { background: transparent; color: var(--gold-hi); border-color: var(--gold-hi); }
.btn:disabled, .btn:disabled:hover { opacity: 0.4; cursor: default; background: var(--gold); border-color: var(--gold); }
.btn.wide { width: 100%; margin-top: 24px; }
.drawer-foot .btn.wide { margin-top: 0; }
.add { height: 44px; padding: 0 18px; border-radius: 999px; border: 1px solid var(--gold); background: var(--gold); color: var(--ink); font-weight: 700; font-size: 12px; letter-spacing: 0.1em; text-transform: uppercase; }
.add:hover { background: var(--gold-hi); border-color: var(--gold-hi); }

/* Header */
.site-header { position: sticky; top: 0; z-index: 50; background: rgba(13, 11, 9, 0.94); -webkit-backdrop-filter: blur(10px); backdrop-filter: blur(10px); border-bottom: 1px solid var(--line); }
.bar { min-height: 96px; display: flex; align-items: center; justify-content: space-between; gap: 24px; padding: 0 var(--gutter); }
.brand { flex: none; display: block; }
.brand img { height: 64px; width: auto; }
.nav { display: flex; align-items: center; gap: 32px; font-size: 13px; letter-spacing: 0.14em; text-transform: uppercase; color: var(--mist); }
.nav a { padding: 6px 0; }
.nav a:hover { color: var(--gold-hi); }
.nav a[aria-current="page"] { color: var(--gold-hi); }
.bag-btn { height: 42px; display: inline-flex; align-items: center; gap: 10px; padding: 0 8px 0 18px; border: 1px solid var(--line-2); border-radius: 999px; background: none; font-size: 13px; letter-spacing: 0.12em; text-transform: uppercase; }
.bag-btn:hover { border-color: var(--gold); }
.count { display: inline-flex; align-items: center; justify-content: center; min-width: 26px; height: 26px; padding: 0 7px; border-radius: 999px; background: var(--gold); color: var(--ink); font-weight: 700; font-size: 12px; }

/* Home */
.hero { position: relative; overflow: hidden; padding: 104px var(--gutter) 96px; }
.topo { position: absolute; inset: 0; opacity: 0.22; pointer-events: none; }
.topo svg { width: 100%; height: 100%; display: block; }
.hero-inner { position: relative; }
.hero-logo { height: 120px; width: auto; margin-bottom: 40px; }
.hero h1 { font-size: clamp(52px, 9vw, 116px); max-width: 11ch; margin-top: 20px; }
.hero .lead { margin-top: 28px; }
.ctas { display: flex; gap: 12px; flex-wrap: wrap; margin-top: 40px; }
.ticker { overflow: hidden; border-top: 1px solid var(--line); border-bottom: 1px solid var(--line); }
.ticker-track { display: flex; width: max-content; padding: 18px 0; animation: tick 42s linear infinite; }
.ticker-track p { flex: none; padding-right: 48px; font-size: 13px; letter-spacing: 0.24em; text-transform: uppercase; color: var(--mist); white-space: nowrap; }
@keyframes tick { to { transform: translateX(-50%); } }
.lines { display: grid; grid-template-columns: repeat(4, minmax(0, 1fr)); gap: 24px; }
.line { display: flex; flex-direction: column; min-height: 300px; padding: 28px; text-align: left; background: var(--ink-2); border: 1px solid var(--line); border-radius: 14px; }
.line:hover { border-color: var(--gold-dk); }
.num { font-family: var(--serif); font-size: 44px; line-height: 1; color: var(--gold); }
.line h3 { font-size: 30px; margin-top: auto; padding-top: 28px; }
.line p { margin-top: 12px; font-size: 14px; line-height: 1.6; color: var(--mist); }
.line .more { margin-top: 20px; font-size: 12px; letter-spacing: 0.14em; text-transform: uppercase; color: var(--gold-hi); }

/* Product cards */
.grid { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 32px; }
.card { display: flex; flex-direction: column; padding: 24px; background: var(--ink-2); border: 1px solid var(--line); border-radius: 14px; }
.art { height: 230px; display: flex; align-items: center; justify-content: center; background: var(--ink-3); border-radius: 10px; }
.art svg { width: 118px; height: 158px; }
.kicker { margin-top: 22px; font-size: 12px; letter-spacing: 0.14em; text-transform: uppercase; color: var(--gold); }
.card h3 { font-size: 30px; margin-top: 8px; }
.notes { margin-top: 10px; font-size: 14px; line-height: 1.6; color: var(--mist); }
.card .foot { margin-top: auto; padding-top: 24px; display: flex; justify-content: space-between; align-items: center; gap: 12px; }
.price { font-family: var(--serif); font-size: 26px; color: var(--gold-hi); font-variant-numeric: tabular-nums; }
.price small { font-family: var(--sans); font-size: 12px; color: var(--mist); }
.empty { grid-column: 1 / -1; padding: 48px 0; text-align: center; color: var(--mist); }

/* Collection */
.tools { display: flex; justify-content: space-between; align-items: center; gap: 20px; flex-wrap: wrap; margin-bottom: 36px; }
.chips { display: flex; gap: 8px; flex-wrap: wrap; }
.chip { height: 44px; padding: 0 20px; border-radius: 999px; border: 1px solid var(--line-2); background: transparent; font-weight: 500; font-size: 13px; letter-spacing: 0.04em; }
.chip:hover { border-color: var(--gold); }
.chip[aria-pressed="true"] { background: var(--gold); border-color: var(--gold); color: var(--ink); font-weight: 700; }
.tools-right { display: flex; align-items: center; gap: 16px; flex-wrap: wrap; justify-content: flex-end; }
.search { width: min(360px, 100%); height: 52px; padding: 0 22px; border-radius: 999px; border: 1px solid var(--line-2); background: var(--ink-2); font-size: 15px; -webkit-appearance: none; appearance: none; }
.search::placeholder { color: var(--mist); }
.count-label { font-size: 14px; color: var(--mist); white-space: nowrap; }

/* Builder */
.build { display: grid; grid-template-columns: minmax(0, 1.1fr) minmax(0, 0.9fr); gap: 32px; align-items: start; }
.panel { padding: clamp(24px, 3vw, 40px); background: var(--ink-2); border: 1px solid var(--line); border-radius: 14px; }
.opt { margin-bottom: 32px; }
.opt:last-child { margin-bottom: 0; }
.label { display: block; margin-bottom: 12px; font-size: 12px; letter-spacing: 0.22em; text-transform: uppercase; color: var(--gold); }
.accords { display: grid; grid-template-columns: repeat(5, minmax(0, 1fr)); gap: 8px; }
.accord { min-height: 84px; padding: 14px; text-align: left; border-radius: 10px; border: 1px solid var(--line); background: var(--ink); }
.accord:hover { border-color: var(--gold-dk); }
.accord[aria-pressed="true"] { border-color: var(--gold); box-shadow: inset 0 0 0 1px var(--gold); }
.accord b { display: block; font-family: var(--serif); font-weight: 600; font-size: 19px; line-height: 1.1; }
.accord span { display: block; margin-top: 6px; font-size: 12px; line-height: 1.4; color: var(--mist); }
.field { width: 100%; height: 52px; padding: 0 16px; border-radius: 10px; border: 1px solid var(--line); background: var(--ink); font-size: 16px; -webkit-appearance: none; appearance: none; }
select.field { padding-right: 40px; background-image: linear-gradient(45deg, transparent 50%, var(--gold) 50%), linear-gradient(135deg, var(--gold) 50%, transparent 50%); background-position: calc(100% - 22px) 50%, calc(100% - 16px) 50%; background-size: 6px 6px; background-repeat: no-repeat; }
input[type="range"] { width: 100%; margin: 0; accent-color: var(--gold); }
.oil-row { display: flex; justify-content: space-between; margin-top: 10px; font-size: 14px; }
.oil-row span:first-child { color: var(--sand); }
.oil-row span:last-child { color: var(--gold-hi); }
.pills { display: flex; gap: 8px; flex-wrap: wrap; }
.pill { height: 44px; padding: 0 20px; border-radius: 999px; border: 1px solid var(--line-2); background: transparent; font-weight: 500; font-size: 13px; letter-spacing: 0.04em; }
.pill:hover { border-color: var(--gold); }
.pill[aria-pressed="true"] { background: var(--gold); border-color: var(--gold); color: var(--ink); font-weight: 700; }
.preview { position: sticky; top: 120px; }
.stage { height: 380px; display: flex; align-items: center; justify-content: center; background: var(--ink); border-radius: 12px; }
.stage svg { width: 190px; height: 253px; }
.spec { margin-top: 24px; padding-top: 16px; border-top: 1px solid var(--line); }
.row { display: flex; justify-content: space-between; align-items: center; gap: 16px; min-height: 36px; font-size: 15px; }
.row span:first-child { color: var(--mist); }
.row.total { margin-top: 6px; padding-top: 8px; border-top: 1px solid var(--line); min-height: 52px; }
.row.total .price { font-size: 28px; }

/* Method and about */
.steps { display: grid; grid-template-columns: repeat(4, minmax(0, 1fr)); gap: 32px; }
.step { padding-top: 32px; border-top: 1px solid var(--line); }
.step .num { display: block; font-size: 56px; }
.step h3 { font-size: 28px; margin-top: 18px; }
.step p { margin-top: 10px; font-size: 15px; line-height: 1.6; color: var(--mist); }
.about { display: grid; grid-template-columns: minmax(0, 1fr) minmax(0, 1fr); gap: 64px; align-items: start; }
.about p { font-size: 18px; line-height: 1.7; color: var(--mist); max-width: 60ch; }
.about p + p { margin-top: 16px; }

/* Footer */
.site-footer { border-top: 1px solid var(--line); padding: 56px var(--gutter) 64px; }
.foot-row { display: flex; justify-content: space-between; align-items: flex-start; gap: 32px; flex-wrap: wrap; }
.foot-logo img { height: 48px; width: auto; }
.foot-row address { font-style: normal; font-size: 14px; line-height: 1.8; color: var(--mist); }
.foot-nav { display: flex; gap: 26px; flex-wrap: wrap; font-size: 12px; letter-spacing: 0.14em; text-transform: uppercase; color: var(--mist); }
.foot-nav a:hover { color: var(--gold-hi); }

/* Bag */
.scrim { position: fixed; inset: 0; z-index: 60; background: rgba(0, 0, 0, 0.55); opacity: 0; pointer-events: none; transition: opacity 0.25s ease; }
.scrim.on { opacity: 1; pointer-events: auto; }
.drawer { position: fixed; top: 0; right: 0; bottom: 0; z-index: 70; width: min(420px, 100%); display: flex; flex-direction: column; background: var(--ink-2); border-left: 1px solid var(--line); transform: translateX(102%); visibility: hidden; transition: transform 0.3s ease, visibility 0.3s; }
.drawer.on { transform: none; visibility: visible; }
.drawer-head { display: flex; justify-content: space-between; align-items: center; padding: 24px; border-bottom: 1px solid var(--line); }
.drawer-head h2 { font-size: 32px; margin: 0; }
.ghost-btn { height: 40px; padding: 0 16px; border-radius: 999px; border: 1px solid var(--line-2); background: none; font-size: 12px; letter-spacing: 0.12em; text-transform: uppercase; }
.ghost-btn:hover { border-color: var(--gold); }
.items { flex: 1; overflow: auto; padding: 8px 24px; }
.item { display: flex; justify-content: space-between; align-items: flex-start; gap: 16px; padding: 20px 0; border-bottom: 1px solid var(--line); }
.item h4 { font-size: 22px; line-height: 1.2; }
.item small { display: block; margin-top: 4px; font-size: 13px; color: var(--mist); }
.item .side { flex: none; text-align: right; }
.item .side .price { font-size: 22px; }
.link-btn { margin-top: 8px; padding: 0; background: none; border: 0; font-size: 13px; color: var(--mist); text-decoration: underline; text-underline-offset: 3px; }
.link-btn:hover { color: var(--gold-hi); }
.drawer-foot { padding: 24px; border-top: 1px solid var(--line); }
.subtotal { display: flex; justify-content: space-between; align-items: center; margin-bottom: 16px; font-size: 15px; color: var(--mist); }
.toast { position: fixed; left: 50%; bottom: 28px; z-index: 80; transform: translate(-50%, 200%); padding: 14px 22px; border-radius: 999px; background: var(--gold); color: var(--ink); font-weight: 700; font-size: 14px; letter-spacing: 0.03em; white-space: nowrap; transition: transform 0.3s ease; }
.toast.on { transform: translate(-50%, 0); }

/* Responsive */
@media (max-width: 1100px) {
  .lines { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .steps { grid-template-columns: repeat(2, minmax(0, 1fr)); row-gap: 48px; }
}
@media (max-width: 900px) {
  .grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .build { grid-template-columns: minmax(0, 1fr); }
  .preview { position: static; }
  .about { grid-template-columns: minmax(0, 1fr); gap: 32px; }
}
@media (max-width: 640px) {
  .bar { flex-wrap: wrap; min-height: 0; padding-top: 14px; padding-bottom: 12px; row-gap: 12px; }
  .brand img { height: 44px; }
  .bag-btn { order: 2; }
  .nav { order: 3; width: 100%; gap: 24px; font-size: 12px; overflow-x: auto; white-space: nowrap; padding-bottom: 2px; }
  .grid, .lines, .steps { grid-template-columns: minmax(0, 1fr); }
  .accords { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .hero { padding-top: 72px; padding-bottom: 64px; }
  .hero-logo { height: 88px; margin-bottom: 28px; }
  .section { padding-top: 80px; padding-bottom: 80px; }
  .section.first { padding-top: 56px; }
  .head { margin-bottom: 32px; }
  .tools-right { width: 100%; justify-content: flex-start; }
  .search { width: 100%; }
  .stage { height: 320px; }
  .panel { padding: 22px; }
}
@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }
  .ticker-track { animation: none; }
  *, *::before, *::after { transition-duration: 0.01ms !important; }
}
</style>
</head>
<body>

<header class="site-header">
  <div class="bar">
    <a class="brand" href="#home" data-go="home" aria-label="WOLFCANIO home"><img data-logo alt="WOLFCANIO"></a>
    <nav class="nav" aria-label="Main">
      <a href="#home" data-go="home" data-anchor="lines">Lines</a>
      <a href="#shop" data-go="shop" data-nav="shop">Shop</a>
      <a href="#create" data-go="create" data-nav="create">Create</a>
      <a href="#method" data-go="method" data-nav="method">Method</a>
      <a href="#about" data-go="about" data-nav="about">About</a>
    </nav>
    <button class="bag-btn" type="button" data-bag>Bag <span class="count" data-count>0</span></button>
  </div>
</header>

<main>

  <section class="view on" id="view-home">
    <div class="hero">
      <div class="topo" id="topo" aria-hidden="true"></div>
      <div class="hero-inner">
        <img class="hero-logo" data-logo alt="WOLFCANIO">
        <p class="eyebrow">Dubai · Perfume House</p>
        <h1>Perfume, poured from oil.</h1>
        <p class="lead">Every WOLFCANIO scent starts with oil, at a 50% concentration by default. Choose one of four lines, or compose your own.</p>
        <div class="ctas">
          <a class="btn" href="#shop" data-go="shop">Shop the collection</a>
          <a class="btn ghost" href="#create" data-go="create">Create your own</a>
        </div>
      </div>
    </div>

    <div class="ticker" aria-label="Highlights">
      <div class="ticker-track">
        <p>Oil-based perfume · 50% oil by default · Dubai-based · Niche · Arabic oud · Design brand · Create your own</p>
        <p aria-hidden="true">Oil-based perfume · 50% oil by default · Dubai-based · Niche · Arabic oud · Design brand · Create your own</p>
      </div>
    </div>

    <section class="section" id="lines">
      <div class="head">
        <div>
          <p class="eyebrow">The lines</p>
          <h2>Four ways to wear it.</h2>
        </div>
      </div>
      <div class="lines">
        <button class="line" type="button" data-go="shop" data-filter="niche">
          <span class="num">01</span>
          <h3>Niche</h3>
          <p>Compositions built around one clear idea.</p>
          <span class="more">Shop niche</span>
        </button>
        <button class="line" type="button" data-go="shop" data-filter="oud">
          <span class="num">02</span>
          <h3>Arabic Oud</h3>
          <p>Resinous, deep oud compositions.</p>
          <span class="more">Shop Arabic oud</span>
        </button>
        <button class="line" type="button" data-go="shop" data-filter="design">
          <span class="num">03</span>
          <h3>Design Brand</h3>
          <p>Original compositions in the spirit of designer houses.</p>
          <span class="more">Shop design brand</span>
        </button>
        <button class="line" type="button" data-go="create">
          <span class="num">04</span>
          <h3>Create Your Own</h3>
          <p>Pick an accord, a top note and the oil strength, then name it.</p>
          <span class="more">Start composing</span>
        </button>
      </div>
    </section>

    <section class="section" id="featured">
      <div class="head">
        <div>
          <p class="eyebrow">Featured</p>
          <h2>Start with three.</h2>
        </div>
        <a class="btn ghost" href="#shop" data-go="shop">See the collection</a>
      </div>
      <div class="grid" id="featured-grid"></div>
    </section>
  </section>

  <section class="view" id="view-shop">
    <div class="page-head">
      <p class="eyebrow">All brand perfume</p>
      <h1>The collection</h1>
    </div>
    <div class="section">
      <div class="tools">
        <div class="chips" role="group" aria-label="Filter by line">
          <button class="chip" type="button" data-filter="all" aria-pressed="true">All</button>
          <button class=