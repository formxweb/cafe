
<!-- IRMAK CAFE · tek dosya. GitHub'da repoya index.html adıyla koyun. Bilgiler: aşağıdaki IRMAK_CONFIG bölümü. -->
<html lang="tr" class="is-loading">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>IRMAK CAFE</title>
<meta name="description" content="IRMAK CAFE — çay, kahve, kahvaltı ve tatlı. Menü, iletişim ve çalışma saatleri.">
<meta name="theme-color" content="#0F0D0C">
<link rel="canonical" href="" id="meta-canonical">
<meta property="og:type" content="website">
<meta property="og:site_name" content="IRMAK CAFE">
<meta property="og:title" content="IRMAK CAFE">
<meta property="og:description" content="Her ırmak bir çayla başlar.">
<meta property="og:locale" content="tr_TR">
<meta property="og:url" content="" id="meta-og-url">
<meta property="og:image" content="" id="meta-og-image">
<meta name="twitter:card" content="summary_large_image">
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns=%27http://www.w3.org/2000/svg%27 viewBox=%270 0 64 64%27%3E%3Crect width=%2764%27 height=%2764%27 fill=%27%230F0D0C%27/%3E%3Ctext x=%2732%27 y=%2745%27 font-family=%27Arial%27 font-weight=%27900%27 font-size=%2736%27 text-anchor=%27middle%27 fill=%27%23F3EEE6%27%3EI%3C/text%3E%3C/svg%3E">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Anybody:wdth,wght@50..150,100..900&family=Newsreader:ital,opsz,wght@0,6..72,300..600;1,6..72,300..500&display=swap">
<style>
/* =====================================================================
   IRMAK CAFE — premium · editoryal · sinematik
   Espresso siyahı, krema, tavşan kanı. Tipografi mimari bir obje gibi
   davranır; kaydırma zamanı, kamerayı ve görüntüyü yönetir.
   Hareket dili: tek eğri (--ease), üç süre (1.4s / .9s / .35s).
   ===================================================================== */
:root {
  --esp: #0F0D0C; --esp-2: #181412; --crema: #F3EEE6; --crema-2: #E7DFD3;
  --ink: #1B1714; --muted-l: #6A6059; --muted-d: #ADA296;
  --cay: #8A2214; --copper: #C9794A;
  --line-l: rgb(27 23 20 / .14); --line-d: rgb(243 238 230 / .14);
  --serif: "Newsreader", "Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif;
  --sans: "Anybody", "Helvetica Neue", Arial, sans-serif;
  --g: clamp(20px, 4vw, 60px);
  --ease: cubic-bezier(.19, 1, .22, 1);
  --t1: 1.4s; --t2: .9s; --t3: .35s;
  --hdr: 84px;
  color-scheme: dark;
}
*, *::before, *::after { box-sizing: border-box; }
html { -webkit-text-size-adjust: 100%; background: var(--esp); scroll-padding-top: 70px; }
body { margin: 0; background: var(--esp); color: var(--crema); font-family: var(--serif); font-size: 1.075rem; line-height: 1.7; -webkit-font-smoothing: antialiased; text-rendering: optimizeLegibility; overflow-x: clip; }
html.is-loading body { overflow: hidden; }
img, video { display: block; max-width: 100%; }
a { color: inherit; text-decoration: none; }
button { font: inherit; color: inherit; background: none; border: 0; padding: 0; cursor: pointer; }
h1, h2, h3, p, figure, ul, ol { margin: 0; padding: 0; }
ul, ol { list-style: none; }
::selection { background: var(--copper); color: var(--esp); }
:focus-visible { outline: 2px solid var(--copper); outline-offset: 3px; }
.sr { position: absolute; width: 1px; height: 1px; overflow: hidden; clip-path: inset(50%); white-space: nowrap; }
.skip { position: fixed; left: 16px; top: 12px; z-index: 300; padding: 10px 14px; background: var(--crema); color: var(--esp); font: 600 .8rem var(--sans); transform: translateY(-200%); }
.skip:focus { transform: none; }
.i { width: 18px; height: 18px; fill: none; stroke: currentColor; stroke-width: 1.6; stroke-linecap: round; stroke-linejoin: round; flex: none; }
.i .dot { fill: currentColor; stroke: none; }
.wrap { width: 100%; max-width: 1400px; margin-inline: auto; padding-inline: var(--g); }
@media (min-width: 1181px) { .wrap { padding-right: max(var(--g), 76px); } }
/* film greni: statik, tek katman */
body::after { content: ""; position: fixed; inset: 0; z-index: 90; pointer-events: none; opacity: .06; background-image: var(--grain, none); background-size: 200px; mix-blend-mode: overlay; }

/* ---------------------------------------------------------------- yazı sistemi */
.meta { display: inline-flex; align-items: center; gap: 14px; font-family: var(--sans); font-size: .7rem; font-variation-settings: "wdth" 115, "wght" 600; letter-spacing: .24em; text-transform: uppercase; }
.meta__no, .akis__no span { color: var(--copper); font-variant-numeric: tabular-nums; }
.h2 { font-family: var(--serif); font-weight: 300; font-size: clamp(2.7rem, 5.4vw, 5.6rem); line-height: 1; letter-spacing: -.03em; margin-top: 24px; }
.h2 em, .menu__title em, .ziyaret__title em, .hero__title em { font-style: italic; color: var(--copper); }
.mask { display: block; overflow: hidden; padding-bottom: .08em; margin-bottom: -.08em; }
.mask > span { display: block; transform: translate3d(0, 110%, 0); transition: transform var(--t1) var(--ease); }
.mask:nth-child(2) > span { transition-delay: .09s; } .mask:nth-child(3) > span { transition-delay: .18s; }
.is-in .mask > span, .mask.is-in > span { transform: none; }

/* ---------------------------------------------------------------- düğmeler */
.btn { position: relative; display: inline-flex; align-items: center; justify-content: center; gap: 10px; min-height: 54px; padding: 0 30px; font-family: var(--sans); font-size: .74rem; font-variation-settings: "wdth" 115, "wght" 620; letter-spacing: .2em; text-transform: uppercase; overflow: hidden; isolation: isolate; transition: color var(--t3) var(--ease), border-color var(--t3); }
.btn::before { content: ""; position: absolute; inset: 0; z-index: -1; transform: translateY(101%); transition: transform .6s var(--ease); }
.btn:hover::before { transform: none; }
.btn--light { background: var(--crema); color: var(--esp); }
.btn--light::before { background: var(--copper); }
.btn--line { border: 1px solid currentColor; }
.btn--line::before { background: currentColor; }
.btn--line:hover { color: var(--esp); }
.menu .btn--line:hover, .ziyaret .btn--line:hover { color: var(--crema); }
.btn--dark { background: var(--esp); color: var(--crema); }
.btn--dark::before { background: var(--cay); }

/* ---------------------------------------------------------------- perde */
.curtain { position: fixed; inset: 0; z-index: 200; background: var(--esp); display: grid; place-content: center; justify-items: center; gap: 18px; clip-path: inset(0 0 0 0); transition: clip-path 1.2s var(--ease); }
.curtain__w { display: flex; font-family: var(--sans); font-size: clamp(3.6rem, 13vw, 11rem); font-variation-settings: "wdth" 150, "wght" 780; line-height: .9; letter-spacing: .02em; overflow: hidden; }
.curtain__w span { display: block; transform: translateY(105%); animation: up 1s var(--ease) forwards; }
.curtain__w span:nth-child(2) { animation-delay: .07s; } .curtain__w span:nth-child(3) { animation-delay: .14s; } .curtain__w span:nth-child(4) { animation-delay: .21s; } .curtain__w span:nth-child(5) { animation-delay: .28s; }
.curtain__s { font-style: italic; color: var(--muted-d); opacity: 0; animation: fade .9s var(--ease) .5s forwards; }
@keyframes up { to { transform: none; } }
@keyframes fade { to { opacity: 1; } }
html.is-open .curtain { clip-path: inset(0 0 100% 0); }
html.is-done .curtain { display: none; }

/* ---------------------------------------------------------------- başlık, dizin */
.hdr { position: fixed; inset: 0 0 auto; z-index: 60; padding-top: env(safe-area-inset-top, 0px); transition: background-color .5s var(--ease), border-color .5s, transform .6s var(--ease); border-bottom: 1px solid transparent; }
.hdr__in { max-width: 1400px; margin-inline: auto; padding-inline: var(--g); height: var(--hdr); display: grid; grid-template-columns: 1fr auto 1fr; align-items: center; gap: 24px; transition: height .5s var(--ease); }
.hdr.is-scrolled { background: rgb(15 13 12 / .82); -webkit-backdrop-filter: blur(16px) saturate(1.2); backdrop-filter: blur(16px) saturate(1.2); border-bottom-color: var(--line-d); }
.hdr.is-scrolled .hdr__in { height: 66px; }
.hdr.is-hidden { transform: translateY(-100%); }
.logo { display: inline-flex; align-items: baseline; gap: 10px; justify-self: start; white-space: nowrap; }
.logo__w { font-family: var(--sans); font-size: 1.26rem; font-variation-settings: "wdth" 125, "wght" 720; letter-spacing: .16em; line-height: 1; }
.logo__c { font-style: italic; font-size: 1.06rem; color: var(--copper); }
.nav { display: flex; gap: 36px; }
.nav a, .hdr__tel { font-family: var(--sans); font-size: .72rem; font-variation-settings: "wdth" 115, "wght" 580; letter-spacing: .2em; text-transform: uppercase; position: relative; padding-block: 8px; }
.nav a::after { content: ""; position: absolute; left: 0; right: 0; bottom: 2px; height: 1px; background: var(--copper); transform: scaleX(0); transform-origin: right; transition: transform .5s var(--ease); }
.nav a:hover::after, .nav a.is-active::after { transform: scaleX(1); transform-origin: left; }
.hdr__act { justify-self: end; display: flex; align-items: center; gap: 20px; }
.hdr__tel { letter-spacing: .12em; }
.hdr__tel:hover, .hdr__ig:hover { color: var(--copper); }
.hdr__ig { display: inline-grid; place-items: center; width: 40px; height: 40px; border: 1px solid var(--line-d); border-radius: 50%; transition: color .3s, border-color .3s; }
.burger { display: none; width: 44px; height: 44px; position: relative; }
.burger span:not(.sr) { position: absolute; left: 10px; right: 10px; height: 1.5px; background: currentColor; }
.burger span:nth-child(1) { top: 17px; } .burger span:nth-child(2) { top: 26px; left: 18px; }

.rail { position: fixed; right: 16px; top: 50%; z-index: 55; transform: translateY(-50%); display: grid; gap: 12px; mix-blend-mode: difference; color: #fff; opacity: 0; pointer-events: none; transition: opacity .6s var(--ease); }
.rail.is-on { opacity: 1; pointer-events: auto; }
.rail a { display: flex; align-items: center; justify-content: flex-end; gap: 10px; min-height: 24px; font-family: var(--sans); font-size: .64rem; font-variation-settings: "wdth" 110, "wght" 600; letter-spacing: .2em; text-transform: uppercase; opacity: .45; transition: opacity .4s; }
.rail a em { font-style: normal; max-width: 0; overflow: hidden; white-space: nowrap; transition: max-width .6s var(--ease); }
.rail a.is-active em { max-width: 0; }
.rail a::after { content: ""; width: 14px; height: 1px; background: currentColor; transition: width .6s var(--ease); }
.rail a:hover, .rail a.is-active { opacity: 1; }
.rail a:hover em { max-width: 120px; }
.rail a.is-active::after { width: 34px; }

/* ---------------------------------------------------------------- giriş */
.hero { position: relative; height: 100svh; min-height: 640px; overflow: hidden; background: var(--esp); display: grid; grid-template-rows: auto 1fr auto; }
.hero__media { position: absolute; inset: 0; }
.hero__media img, .hero__media video { width: 100%; height: 100%; object-fit: cover; object-position: 60% 50%; transform: scale(calc(1.14 - var(--hz, 0) * .14)) translate3d(0, var(--hy, 0px), 0); transition: transform 2.6s var(--ease); will-change: transform; }
html.is-ready .hero__media img, html.is-ready .hero__media video { --hz: 1; }
.hero__shade { position: absolute; inset: 0; background: linear-gradient(90deg, rgb(15 13 12 / .88) 0%, rgb(15 13 12 / .5) 42%, rgb(15 13 12 / .1) 75%), linear-gradient(0deg, rgb(15 13 12 / .92) 0%, rgb(15 13 12 / .2) 38%, transparent 55%); }
.hero__top { position: relative; z-index: 2; display: flex; justify-content: space-between; gap: 20px; padding-top: calc(var(--hdr) + 26px); color: rgb(243 238 230 / .72); }
.hero__loc span:empty { display: none; }
.hero__mid { position: relative; z-index: 2; align-self: center; display: grid; justify-items: start; gap: 34px; padding-bottom: 16vw; }
.hero__title { font-family: var(--serif); font-weight: 300; font-size: clamp(3.2rem, 7.6vw, 8.2rem); line-height: .96; letter-spacing: -.035em; }
.hero__lead { font-size: clamp(1.05rem, 1.3vw, 1.25rem); color: rgb(243 238 230 / .82); max-width: 30em; }
.hero__cta { display: flex; flex-wrap: wrap; gap: 12px; margin-top: 30px; }
.hero__word { position: absolute; left: 0; right: 0; bottom: 0; z-index: 1; text-align: center; font-family: var(--sans); font-variation-settings: "wdth" 150, "wght" 800; font-size: 18.6vw; line-height: .74; letter-spacing: -.01em; color: var(--crema); transform: translate3d(0, calc(14% + var(--wy, 0px)), 0); white-space: nowrap; pointer-events: none; }
[data-rise] { opacity: 0; transform: translateY(20px); transition: opacity 1.2s var(--ease), transform 1.2s var(--ease); }
html.is-ready [data-rise] { opacity: 1; transform: none; }
html.is-ready .hero__side[data-rise] { transition-delay: .35s; }
html.is-ready .hero .mask > span { transform: none; }

/* ---------------------------------------------------------------- akış */
.akis { background: var(--esp); padding-block: clamp(120px, 18vw, 260px); }
.akis__in { max-width: 1180px; }
.akis__no { margin-bottom: 44px; gap: 18px; }
.akis__text { font-family: var(--serif); font-weight: 300; font-size: clamp(1.9rem, 3.7vw, 3.9rem); line-height: 1.22; letter-spacing: -.02em; }
.akis__text .w { opacity: var(--o, .14); transition: opacity .25s linear; }
.akis__sub { margin-top: 48px; max-width: 32em; margin-left: auto; color: var(--muted-d); font-size: 1.15rem; font-style: italic; }

/* ---------------------------------------------------------------- açılan kare */
.acilim { position: relative; height: 260vh; background: var(--esp); }
.acilim__stick { position: sticky; top: 0; height: 100svh; overflow: hidden; }
.acilim__fig { position: absolute; inset: 0; clip-path: inset(var(--it, 28%) var(--il, 34%) var(--it, 28%) var(--il, 34%)); will-change: clip-path; }
.acilim__fig img { width: 100%; height: 100%; object-fit: cover; transform: scale(var(--is, 1.3)); will-change: transform; }
.acilim__fig::after { content: ""; position: absolute; inset: 0; background: rgb(15 13 12 / var(--ish, 0)); }
.acilim__text { position: absolute; inset: 0; display: grid; place-content: center; justify-items: center; gap: 22px; text-align: center; padding: var(--g); opacity: var(--to, 0); transform: translateY(calc((1 - var(--to, 0)) * 30px)); }
.acilim__q { font-family: var(--serif); font-style: italic; font-weight: 300; font-size: clamp(2.4rem, 6vw, 6.2rem); line-height: 1.02; letter-spacing: -.025em; }

/* ---------------------------------------------------------------- imza */
.imza { background: var(--esp-2); }
.imza__grid { display: grid; grid-template-columns: 1fr 1fr; }
.imza__media { position: sticky; top: 0; height: 100svh; overflow: hidden; }
.imza__img { position: absolute; inset: 0; clip-path: inset(100% 0 0 0); transition: clip-path 1.2s var(--ease); }
.imza__img img { width: 100%; height: 100%; object-fit: cover; transform: scale(1.12); transition: transform 1.8s var(--ease); }
.imza__img.is-on { clip-path: inset(0); z-index: 2; }
.imza__img.is-on img { transform: none; }
.imza__img.was { clip-path: inset(0); z-index: 1; }
.imza__count { position: absolute; left: 28px; bottom: 24px; z-index: 3; color: var(--crema); mix-blend-mode: difference; }
.imza__list { padding-inline: clamp(28px, 6vw, 110px); }
.imza__head { padding-top: clamp(110px, 16vh, 180px); }
.dish { min-height: 100svh; display: flex; flex-direction: column; justify-content: center; gap: 22px; padding-block: 60px; }
.dish__img { display: none; }
.dish__k { color: var(--copper); }
.dish__name { font-family: var(--sans); font-variation-settings: "wdth" 125, "wght" 720; font-size: clamp(2.8rem, 5.4vw, 5.6rem); line-height: .9; letter-spacing: -.01em; text-transform: uppercase; }
.dish__desc { font-size: clamp(1.15rem, 1.5vw, 1.4rem); line-height: 1.5; color: rgb(243 238 230 / .82); max-width: 24em; }
.dish__foot { display: flex; align-items: center; gap: 28px; padding-top: 22px; border-top: 1px solid var(--line-d); max-width: 30em; }
.dish__price { font-family: var(--sans); font-variation-settings: "wdth" 110, "wght" 600; font-size: 1.3rem; letter-spacing: .04em; font-variant-numeric: tabular-nums; }
.dish__link { font-family: var(--sans); font-size: .72rem; font-variation-settings: "wdth" 115, "wght" 600; letter-spacing: .2em; text-transform: uppercase; color: var(--muted-d); display: inline-flex; gap: 10px; align-items: center; min-height: 44px; }
.dish__link:hover { color: var(--crema); }
.dish__tag { margin-left: auto; font-family: var(--sans); font-size: .64rem; letter-spacing: .2em; text-transform: uppercase; color: var(--muted-d); font-variation-settings: "wdth" 110, "wght" 560; }

/* ---------------------------------------------------------------- tipografi bandı */
.band { background: var(--esp); padding-block: clamp(70px, 9vw, 130px); overflow: hidden; }
.band__row { white-space: nowrap; font-family: var(--serif); font-style: italic; font-weight: 300; font-size: clamp(4rem, 11vw, 11.5rem); line-height: 1.02; letter-spacing: -.03em; transform: translate3d(var(--bx, 0px), 0, 0); will-change: transform; }
.band__row--o { font-family: var(--sans); font-style: normal; font-variation-settings: "wdth" 150, "wght" 700; letter-spacing: .01em; text-transform: uppercase; color: transparent; -webkit-text-stroke: 1px rgb(243 238 230 / .42); font-size: clamp(3.4rem, 9vw, 9.5rem); margin-top: 1vw; }

/* ---------------------------------------------------------------- menü */
.menu { background: var(--crema); color: var(--ink); color-scheme: light; padding-block: clamp(110px, 13vw, 190px); position: relative; }
.menu .meta__no { color: var(--cay); }
.menu__head { display: grid; justify-items: start; margin-bottom: clamp(40px, 5vw, 70px); }
.menu__title { font-family: var(--serif); font-weight: 300; font-size: clamp(4.4rem, 14vw, 14rem); line-height: .86; letter-spacing: -.045em; margin-top: 12px; }
.menu__note { margin-top: 18px; font-style: italic; color: var(--muted-l); font-size: .95rem; }
.menu__bar { display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: 18px 32px; padding-bottom: 20px; border-bottom: 1px solid var(--line-l); margin-bottom: clamp(36px, 5vw, 64px); }
.tabs { display: flex; flex-wrap: wrap; gap: 6px 34px; }
.tab { position: relative; min-height: 44px; font-family: var(--sans); font-size: .76rem; font-variation-settings: "wdth" 115, "wght" 620; letter-spacing: .2em; text-transform: uppercase; color: var(--muted-l); transition: color .3s; }
.tab sup { font-size: .6em; margin-left: 4px; color: var(--muted-l); letter-spacing: .08em; }
.tab::after { content: ""; position: absolute; left: 0; right: 0; bottom: 4px; height: 2px; background: var(--cay); transform: scaleX(0); transform-origin: left; transition: transform .6s var(--ease); }
.tab[aria-selected="true"] { color: var(--ink); }
.tab[aria-selected="true"]::after { transform: scaleX(1); }
.tab:hover { color: var(--ink); }
.search { display: flex; align-items: center; gap: 10px; border-bottom: 1px solid var(--line-l); min-width: 240px; color: var(--muted-l); }
.search input { flex: 1; min-width: 0; min-height: 44px; border: 0; background: transparent; font: italic 1.02rem var(--serif); color: var(--ink); outline: none; }
.search input::placeholder { color: var(--muted-l); }
.search:focus-within { border-color: var(--ink); color: var(--ink); }
.search input::-webkit-search-cancel-button { -webkit-appearance: none; }
.menu__grid { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 34px clamp(48px, 7vw, 120px); transition: opacity .45s var(--ease), transform .45s var(--ease); }
.menu__list.is-swap .menu__grid { opacity: 0; transform: translateY(14px); }
.menu__cat { grid-column: 1 / -1; font-family: var(--sans); font-size: .68rem; font-variation-settings: "wdth" 115, "wght" 620; letter-spacing: .22em; text-transform: uppercase; color: var(--cay); padding-top: 10px; }
.item { display: grid; grid-template-columns: minmax(0, 1fr); gap: 4px; position: relative; }
.item__row { display: flex; align-items: baseline; gap: 12px; }
.item__no { font-family: var(--sans); font-size: .64rem; font-variation-settings: "wdth" 110, "wght" 600; letter-spacing: .16em; color: var(--muted-l); min-width: 2.2em; font-variant-numeric: tabular-nums; }
.item__name { font-family: var(--serif); font-weight: 400; font-size: clamp(1.3rem, 1.7vw, 1.6rem); line-height: 1.2; letter-spacing: -.01em; transition: color .35s, transform .6s var(--ease); }
.item[data-img] .item__name::after { content: " ◦"; color: var(--cay); font-size: .7em; vertical-align: .15em; }
.item:hover .item__name { color: var(--cay); transform: translateX(6px); }
.item__dots { flex: 1; min-width: 24px; border-bottom: 1px dotted rgb(27 23 20 / .32); transform: translateY(-6px); }
.price { font-family: var(--sans); font-variation-settings: "wdth" 105, "wght" 580; font-variant-numeric: tabular-nums; letter-spacing: .04em; white-space: nowrap; }
.item__desc { color: var(--muted-l); font-size: .96rem; font-style: italic; line-height: 1.5; padding-left: calc(2.2em * .64 / .96 + 12px); }
.item__thumb { display: none; }
.menu__empty { font-style: italic; color: var(--muted-l); font-size: 1.2rem; }
.float { position: fixed; left: 0; top: 0; z-index: 40; width: 240px; aspect-ratio: 4 / 5; overflow: hidden; pointer-events: none; opacity: 0; transform: translate3d(var(--fx, 0px), var(--fy, 0px), 0) scale(.9) rotate(var(--fr, 0deg)); transition: opacity .35s var(--ease), transform .35s var(--ease); box-shadow: 0 30px 60px rgb(0 0 0 / .25); }
.float.is-on { opacity: 1; transform: translate3d(var(--fx, 0px), var(--fy, 0px), 0) scale(1) rotate(var(--fr, 0deg)); }
.float img { width: 100%; height: 100%; object-fit: cover; }

/* ---------------------------------------------------------------- galeri */
.gallery { background: var(--esp); padding-block: clamp(110px, 13vw, 190px); }
.gallery__head { display: grid; grid-template-columns: 1fr auto; align-items: end; gap: 24px; margin-bottom: clamp(60px, 8vw, 120px); }
.gallery__head .meta, .gallery__head .h2 { grid-column: 1; }
.gallery__head .btn { grid-column: 2; grid-row: 2; }
.gal { display: grid; grid-template-columns: repeat(12, minmax(0, 1fr)); column-gap: clamp(14px, 2vw, 28px); row-gap: clamp(40px, 6vw, 90px); align-items: start; }
.shot { position: relative; display: block; text-align: left; cursor: zoom-in; width: 100%; }
.shot__img { overflow: hidden; background: var(--esp-2); }
.shot__img img { width: 100%; height: auto; transform: translate3d(0, var(--py, 0px), 0) scale(1.12); transition: transform .2s linear; will-change: transform; }
.shot__cap { display: flex; justify-content: space-between; margin-top: 14px; font-family: var(--sans); font-size: .66rem; font-variation-settings: "wdth" 110, "wght" 600; letter-spacing: .2em; text-transform: uppercase; color: var(--muted-d); }
.shot:hover .shot__cap { color: var(--crema); }
.shot:nth-child(1) { grid-column: 1 / 8; }
.shot:nth-child(2) { grid-column: 9 / 13; margin-top: 18vh; }
.shot:nth-child(3) { grid-column: 2 / 6; margin-top: -6vh; }
.shot:nth-child(4) { grid-column: 7 / 12; margin-top: 8vh; }
.shot:nth-child(5) { grid-column: 1 / 5; }
.shot:nth-child(6) { grid-column: 6 / 13; margin-top: 14vh; }

/* ---------------------------------------------------------------- ziyaret */
.ziyaret { background: var(--crema); color: var(--ink); color-scheme: light; padding-block: clamp(110px, 13vw, 190px); }
.ziyaret .meta__no { color: var(--cay); }
.ziyaret .h2 em, .ziyaret__title em { color: var(--cay); }
.ziyaret__title { font-family: var(--serif); font-weight: 300; font-size: clamp(3rem, 7.4vw, 7.6rem); line-height: .96; letter-spacing: -.035em; margin-top: 24px; }
.ziyaret__phone { display: inline-block; margin-top: clamp(40px, 6vw, 80px); font-family: var(--sans); font-variation-settings: "wdth" 125, "wght" 700; font-size: clamp(2.3rem, 7.4vw, 7.8rem); line-height: 1; letter-spacing: -.01em; font-variant-numeric: tabular-nums; background: linear-gradient(var(--cay), var(--cay)) 0 100% / 0 3px no-repeat; transition: background-size .8s var(--ease), color .4s; padding-bottom: 8px; white-space: nowrap; }
.ziyaret__phone:hover { background-size: 100% 3px; color: var(--cay); }
.ziyaret__phone:empty { display: none; }
.ziyaret__grid { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 40px clamp(28px, 4vw, 64px); margin-top: clamp(56px, 7vw, 100px); padding-top: 32px; border-top: 1px solid var(--line-l); }
.info { display: grid; gap: 10px; align-content: start; }
.info__k { font-family: var(--sans); font-size: .68rem; font-variation-settings: "wdth" 115, "wght" 620; letter-spacing: .22em; text-transform: uppercase; color: var(--muted-l); }
.info__v { font-size: 1.35rem; line-height: 1.35; }
.info__v small { display: block; font-size: .95rem; font-style: italic; color: var(--muted-l); margin-top: 4px; }
.info .btn { justify-self: start; margin-top: 8px; min-height: 46px; padding: 0 22px; }
.hours { width: 100%; border-collapse: collapse; font-size: 1rem; }
.hours th, .hours td { padding: 3px 0; text-align: left; font-weight: 400; }
.hours td { text-align: right; font-family: var(--sans); font-variation-settings: "wdth" 105, "wght" 520; font-variant-numeric: tabular-nums; }
.hours tr.is-today { color: var(--cay); }

/* ---------------------------------------------------------------- alt bilgi */
.foot { background: var(--esp); padding-top: clamp(80px, 9vw, 130px); overflow: hidden; }
.foot__top { display: grid; grid-template-columns: 1.4fr 1fr 1fr; gap: 40px; }
.foot__tag { font-family: var(--serif); font-style: italic; font-weight: 300; font-size: clamp(1.8rem, 2.8vw, 2.6rem); line-height: 1.1; max-width: 12ch; }
.foot__nav, .foot__contact { display: grid; gap: 10px; align-content: start; }
.foot__nav { font-family: var(--sans); font-size: .72rem; font-variation-settings: "wdth" 115, "wght" 580; letter-spacing: .2em; text-transform: uppercase; }
.foot__nav a:hover, .foot__contact a:hover { color: var(--copper); }
.foot__contact { color: var(--muted-d); }
.foot__contact a { color: var(--crema); }
.foot__word { font-family: var(--sans); font-variation-settings: "wdth" 150, "wght" 800; font-size: 18.6vw; line-height: .74; text-align: center; letter-spacing: -.01em; color: var(--crema); margin-top: clamp(50px, 7vw, 100px); transform: translateY(8%); }
.foot__base { display: flex; flex-wrap: wrap; justify-content: space-between; gap: 12px; padding-block: 22px calc(22px + env(safe-area-inset-bottom, 0px)); border-top: 1px solid var(--line-d); font-family: var(--sans); font-size: .66rem; font-variation-settings: "wdth" 110, "wght" 520; letter-spacing: .16em; text-transform: uppercase; color: var(--muted-d); position: relative; background: var(--esp); }

/* ---------------------------------------------------------------- mobil gezinme, fab, ışık kutusu */
.fab { display: none; }
.mnav, .lb { width: 100%; height: 100%; max-width: none; max-height: none; margin: 0; border: 0; padding: 0; background: var(--esp); color: var(--crema); }
.mnav::backdrop, .lb::backdrop { background: rgb(15 13 12 / .92); }
.mnav__in { min-height: 100%; display: grid; grid-template-rows: auto 1fr auto; padding: calc(env(safe-area-inset-top, 0px) + 18px) var(--g) calc(env(safe-area-inset-bottom, 0px) + 28px); }
.mnav__top { display: flex; justify-content: space-between; align-items: center; min-height: 48px; }
.mnav__close { font-family: var(--sans); font-size: .72rem; font-variation-settings: "wdth" 115, "wght" 600; letter-spacing: .2em; text-transform: uppercase; min-height: 44px; }
.mnav__links { align-self: center; display: grid; gap: 4px; }
.mnav__links a { display: flex; align-items: baseline; gap: 16px; font-family: var(--serif); font-weight: 300; font-size: clamp(2.6rem, 11vw, 3.8rem); line-height: 1.15; letter-spacing: -.02em; }
.mnav__links span { font-family: var(--sans); font-size: .7rem; letter-spacing: .2em; color: var(--copper); font-variation-settings: "wdth" 110, "wght" 600; }
.mnav__foot { display: grid; gap: 12px; }
.lb[open] { display: grid; grid-template-rows: auto 1fr auto; padding: calc(env(safe-area-inset-top, 0px) + 12px) var(--g) calc(env(safe-area-inset-bottom, 0px) + 16px); }
.lb__close { justify-self: end; min-height: 44px; font-family: var(--sans); font-size: .72rem; letter-spacing: .2em; text-transform: uppercase; font-variation-settings: "wdth" 115, "wght" 600; }
.lb__fig { min-height: 0; display: grid; grid-template-rows: 1fr auto; place-items: center; gap: 12px; }
.lb__fig img { max-width: 100%; max-height: 100%; object-fit: contain; }
.lb__fig figcaption { font-style: italic; color: var(--muted-d); }
.lb__nav { display: flex; justify-content: center; gap: 12px; }
.lb__nav button { width: 52px; height: 52px; border: 1px solid var(--line-d); border-radius: 50%; }
.lb__nav button:hover { border-color: var(--copper); color: var(--copper); }

/* ---------------------------------------------------------------- görünüm */
.pre[data-reveal] { opacity: 0; transform: translateY(30px); }
.in[data-reveal] { opacity: 1; transform: none; transition: opacity 1.2s var(--ease) var(--d, 0s), transform 1.2s var(--ease) var(--d, 0s); }

@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after { animation-duration: 1ms !important; animation-delay: 0s !important; transition-duration: 1ms !important; transition-delay: 0s !important; }
  .mask > span, [data-rise] { transform: none !important; opacity: 1 !important; }
  .curtain { display: none; }
}

/* ---------------------------------------------------------------- orta ekran */
@media (max-width: 1180px) { .rail { display: none; } .nav { gap: 24px; } .hdr__tel { display: none; } }
/* ---------------------------------------------------------------- mobil */
@media (max-width: 860px) {
  :root { --hdr: 66px; }
  .nav { display: none; }
  .hdr__in { grid-template-columns: 1fr auto; }
  .hdr__act { gap: 6px; }
  .burger { display: block; }
  .hero { grid-template-rows: auto 1fr; }
  .hero__top .hero__loc { display: none; }
  .hero__shade { background: linear-gradient(0deg, rgb(15 13 12 / .96) 0%, rgb(15 13 12 / .7) 40%, rgb(15 13 12 / .15) 70%, rgb(15 13 12 / .5) 100%); }
  .hero__mid { grid-template-columns: 1fr; align-self: end; gap: 26px; padding-bottom: calc(22vw + 30px); }
  .hero__title { font-size: clamp(3rem, 14vw, 4.4rem); }
  .hero__cta .btn { flex: 1 1 auto; }
  .akis__sub { margin-left: 0; }
  .acilim { height: 220vh; }
  .imza__grid { display: block; }
  .imza__media { display: none; }
  .imza__list { padding-inline: var(--g); padding-bottom: 80px; }
  .imza__head { padding-top: 110px; padding-bottom: 20px; }
  .dish { min-height: 0; padding-block: 44px; }
  .dish__img { display: block; aspect-ratio: 4 / 5; overflow: hidden; margin-bottom: 8px; }
  .dish__img img { width: 100%; height: 100%; object-fit: cover; }
  .dish__name { font-size: clamp(2.4rem, 11vw, 3.4rem); }
  .band__row { font-size: 17vw; }
  .band__row--o { font-size: 14vw; }
  .menu__bar { display: grid; justify-content: stretch; }
  .tabs { flex-wrap: nowrap; overflow-x: auto; gap: 26px; scrollbar-width: none; margin-inline: calc(var(--g) * -1); padding-inline: var(--g); }
  .tabs::-webkit-scrollbar { display: none; }
  .tab { flex: none; }
  .search { min-width: 0; }
  .menu__grid { grid-template-columns: 1fr; gap: 26px; }
  .item[data-img] { grid-template-columns: minmax(0, 1fr) 64px; column-gap: 14px; }
  .item[data-img] .item__thumb { display: block; grid-column: 2; grid-row: 1 / span 2; width: 64px; aspect-ratio: 1; object-fit: cover; }
  .item[data-img] .item__name::after { content: none; }
  .float { display: none; }
  .gallery__head { grid-template-columns: 1fr; }
  .gallery__head .btn { grid-column: 1; grid-row: auto; justify-self: start; }
  .gal { grid-template-columns: repeat(2, minmax(0, 1fr)); row-gap: 28px; }
  .shot:nth-child(n) { grid-column: auto; margin-top: 0; }
  .shot:nth-child(1), .shot:nth-child(6) { grid-column: 1 / -1; }
  .shot:nth-child(3), .shot:nth-child(5) { margin-top: 40px; }
  .ziyaret__grid { grid-template-columns: 1fr; }
  .foot__top { grid-template-columns: 1fr; }
  .fab { position: fixed; right: 18px; bottom: calc(18px + env(safe-area-inset-bottom, 0px)); z-index: 45; display: grid; place-items: center; width: 58px; height: 58px; border-radius: 50%; background: var(--copper); color: var(--esp); box-shadow: 0 10px 30px rgb(0 0 0 / .35); transition: transform .5s var(--ease), opacity .5s; }
  .fab .i { width: 22px; height: 22px; stroke-width: 1.8; }
  .fab.is-hidden { transform: translateY(90px); opacity: 0; }
}

/* stok fotoğraflara ortak sıcak ton */
main img, .float img, .lb img { filter: saturate(.9) sepia(.08) contrast(1.03); }
</style>
<script type="application/ld+json" id="ld-json">{}</script>
</head>
<body>
<a class="skip" href="#menu">Menüye geç</a>

<!-- AÇILIŞ PERDESİ -->
<div class="curtain" aria-hidden="true" data-curtain>
  <p class="curtain__w"><span>I</span><span>R</span><span>M</span><span>A</span><span>K</span></p>
  <p class="curtain__s">Her ırmak bir çayla başlar</p>
</div>

<header class="hdr" data-hdr>
  <div class="hdr__in">
    <a class="logo" href="#top" aria-label="IRMAK CAFE, sayfanın başı"><span class="logo__w">IRMAK</span><span class="logo__c">Cafe</span></a>
    <nav class="nav" aria-label="Ana menü">
      <a href="#hikaye">Hikâye</a><a href="#imza">İmza</a><a href="#menu">Menü</a><a href="#galeri">Galeri</a><a href="#ziyaret">Ziyaret</a>
    </nav>
    <div class="hdr__act">
      <a class="hdr__tel" data-tel href="#ziyaret"><span data-phone-text>Ara</span></a>
      <a class="hdr__ig" data-ig href="#" target="_blank" rel="noopener" aria-label="Instagram"><svg class="i" viewBox="0 0 24 24" aria-hidden="true"><rect x="3" y="3" width="18" height="18" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.5" cy="6.5" r="1" class="dot"/></svg></a>
      <button class="burger" type="button" aria-haspopup="dialog" aria-controls="mnav" data-open-nav><span></span><span></span><span class="sr">Menüyü aç</span></button>
    </div>
  </div>
</header>

<!-- YÜZEN DİZİN -->
<nav class="rail" aria-label="Bölümler" data-rail>
  <a href="#hikaye" data-rail-for="hikaye"><span>01</span><em>Hikâye</em></a>
  <a href="#imza" data-rail-for="imza"><span>02</span><em>İmza</em></a>
  <a href="#menu" data-rail-for="menu-bolum"><span>03</span><em>Menü</em></a>
  <a href="#galeri" data-rail-for="galeri"><span>04</span><em>Galeri</em></a>
  <a href="#ziyaret" data-rail-for="ziyaret"><span>05</span><em>Ziyaret</em></a>
</nav>

<main id="top">

  <!-- GİRİŞ -->
  <section class="hero" aria-labelledby="hero-title" data-hero>
    <div class="hero__media" data-hero-media aria-hidden="true">
      <picture><source media="(max-width: 860px)" srcset="https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/bg_1.jpg" data-hero-m><img src="https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/bg_1.jpg" alt="" data-hero-img decoding="async"></picture>
    </div>
    <div class="hero__shade" aria-hidden="true"></div>
    <div class="hero__top wrap">
      <p class="meta" data-rise>Çay · Kahve · Kahvaltı · Tatlı</p>
      <p class="meta hero__loc" data-rise><span data-status-line></span></p>
    </div>
    <div class="hero__mid wrap">
      <h1 class="hero__title" id="hero-title"><span class="mask"><span>Her ırmak</span></span><span class="mask"><span>bir <em>çayla</em> başlar.</span></span></h1>
      <div class="hero__side" data-rise>
        <p class="hero__lead" data-copy="heroLead">Demli çay, özenle hazırlanmış kahve ve acele etmeyen sohbetler.</p>
        <div class="hero__cta">
          <a class="btn btn--light" href="#menu">Menüyü incele</a>
          <a class="btn btn--line" data-tel href="#ziyaret">Bizi arayın</a>
        </div>
      </div>
    </div>
    <p class="hero__word" aria-hidden="true" data-hero-word>IRMAK</p>
  </section>

  <!-- AKIŞ: kaydırdıkça beliren anlatı -->
  <section class="akis" id="hikaye" aria-labelledby="akis-title">
    <div class="wrap akis__in">
      <p class="meta akis__no"><span>01</span>Hikâye</p>
      <h2 class="sr" id="akis-title">Hikâyemiz</h2>
      <p class="akis__text" data-words>Irmak aynı yatakta akar ama suyu hiçbir zaman aynı değildir. Burada da masa aynı masa, fincan aynı fincan; değişen, her gelişte başka türlü akan zamandır.</p>
      <p class="akis__sub" data-reveal>Kimi gün bir kahve kadar kısa, kimi gün bir sohbet kadar uzun. Saatler, derler ya, burada su gibi akar.</p>
    </div>
  </section>

  <!-- AÇILAN KARE -->
  <section class="acilim" aria-label="Aynı ırmağa iki kez girilmez" data-acilim>
    <div class="acilim__stick">
      <figure class="acilim__fig" data-acilim-fig>
        <picture><source media="(max-width: 860px)" srcset="https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/carousel-1.jpg" data-reveal-m><img src="https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/carousel-1.jpg" alt="" loading="lazy" decoding="async" data-reveal-img></picture>
      </figure>
      <div class="acilim__text" data-acilim-text>
        <p class="acilim__q">“Aynı ırmağa<br>iki kez girilmez.”</p>
        <p class="meta">Herakleitos · Efes</p>
      </div>
    </div>
  </section>

  <!-- İMZA: her ürün küçük bir kampanya sahnesi -->
  <section class="imza" id="imza" aria-labelledby="imza-title">
    <div class="imza__grid">
      <div class="imza__media" data-imza-media aria-hidden="true"></div>
      <div class="imza__list">
        <header class="imza__head">
          <p class="meta"><span class="meta__no">02</span>İmza lezzetler</p>
          <h2 class="h2" id="imza-title"><span class="mask"><span>Masanın</span></span><span class="mask"><span><em>yıldızları</em></span></span></h2>
        </header>
        <div data-signatures></div>
      </div>
    </div>
  </section>

  <!-- TİPOGRAFİ BANDI -->
  <section class="band" aria-hidden="true" data-band>
    <p class="band__row" data-band-row="1">Çay · Kahve · Kahvaltı · Tatlı · Çay · Kahve · Kahvaltı · Tatlı ·</p>
    <p class="band__row band__row--o" data-band-row="-1">Sohbet · Mola · Sabah · Akşam · Sohbet · Mola · Sabah · Akşam ·</p>
  </section>

  <!-- MENÜ -->
  <section class="menu" id="menu-bolum" aria-labelledby="menu">
    <div class="wrap">
      <div class="menu__head">
        <p class="meta"><span class="meta__no">03</span>Menü</p>
        <h2 class="menu__title" id="menu" tabindex="-1"><span class="mask"><span>Menü</span></span></h2>
        <p class="menu__note" data-sample-note hidden>Örnek menü · ürün, fiyat ve fotoğraflar temsilidir</p>
      </div>
      <div class="menu__bar">
        <div class="tabs" role="tablist" aria-label="Menü kategorileri" data-tabs></div>
        <label class="search" for="menu-search"><span class="sr">Menüde ara</span>
          <svg class="i" viewBox="0 0 24 24" aria-hidden="true"><circle cx="11" cy="11" r="6"/><path d="m20 20-4.5-4.5"/></svg>
          <input type="search" id="menu-search" name="menu-search" placeholder="Menüde ara" autocomplete="off" data-search>
        </label>
      </div>
      <div class="menu__list" data-list aria-live="polite"></div>
    </div>
    <figure class="float" data-float aria-hidden="true"><img alt="" data-float-img></figure>
  </section>

  <!-- GALERİ -->
  <section class="gallery" id="galeri" aria-labelledby="gal-title">
    <div class="wrap">
      <div class="gallery__head">
        <p class="meta"><span class="meta__no">04</span>Galeri</p>
        <h2 class="h2" id="gal-title"><span class="mask"><span>Fincandan</span></span><span class="mask"><span><em>kareler</em></span></span></h2>
        <a class="btn btn--line" data-ig href="#" target="_blank" rel="noopener"><span data-ig-text>Instagram</span></a>
      </div>
      <div class="gal" data-gallery></div>
    </div>
  </section>

  <!-- ZİYARET -->
  <section class="ziyaret" id="ziyaret" aria-labelledby="ziyaret-title">
    <div class="wrap">
      <p class="meta"><span class="meta__no">05</span>Ziyaret</p>
      <h2 class="ziyaret__title" id="ziyaret-title"><span class="mask"><span>Bir çay</span></span><span class="mask"><span><em>içmeye</em> gelin.</span></span></h2>
      <a class="ziyaret__phone" data-tel href="#ziyaret" data-phone-big></a>
      <div class="ziyaret__grid" data-contact></div>
    </div>
  </section>
</main>

<footer class="foot">
  <div class="wrap foot__top">
    <p class="foot__tag">Her ırmak bir çayla başlar.</p>
    <nav class="foot__nav" aria-label="Alt menü"><a href="#hikaye">Hikâye</a><a href="#imza">İmza</a><a href="#menu">Menü</a><a href="#galeri">Galeri</a><a href="#ziyaret">Ziyaret</a></nav>
    <div class="foot__contact" data-foot-contact></div>
  </div>
  <p class="foot__word" aria-hidden="true">IRMAK</p>
  <div class="wrap foot__base"><p data-copyright>© IRMAK CAFE</p><a href="#top">Başa dön ↑</a></div>
</footer>

<a class="fab" data-tel href="#ziyaret" aria-label="Telefonla arayın"><svg class="i" viewBox="0 0 24 24" aria-hidden="true"><path d="M5 4h3l2 5-2.5 1.5a11 11 0 0 0 6 6L15 14l5 2v3a2 2 0 0 1-2 2A16 16 0 0 1 3 6a2 2 0 0 1 2-2"/></svg></a>

<dialog class="mnav" id="mnav" aria-label="Menü">
  <div class="mnav__in">
    <div class="mnav__top"><p class="logo"><span class="logo__w">IRMAK</span><span class="logo__c">Cafe</span></p><button class="mnav__close" type="button" data-close-nav>Kapat</button></div>
    <nav class="mnav__links" aria-label="Mobil menü">
      <a href="#hikaye"><span>01</span>Hikâye</a><a href="#imza"><span>02</span>İmza</a><a href="#menu"><span>03</span>Menü</a><a href="#galeri"><span>04</span>Galeri</a><a href="#ziyaret"><span>05</span>Ziyaret</a>
    </nav>
    <div class="mnav__foot"><a class="btn btn--light" data-tel href="#ziyaret"><span data-phone-text>Ara</span></a><a class="btn btn--line" data-ig href="#" target="_blank" rel="noopener"><span data-ig-text>Instagram</span></a></div>
  </div>
</dialog>

<dialog class="lb" id="lb" aria-label="Fotoğraf">
  <button class="lb__close" type="button" data-lb-close>Kapat</button>
  <figure class="lb__fig"><img alt="" data-lb-img><figcaption data-lb-cap></figcaption></figure>
  <div class="lb__nav"><button type="button" data-lb-prev aria-label="Önceki fotoğraf">←</button><button type="button" data-lb-next aria-label="Sonraki fotoğraf">→</button></div>
</dialog>

<noscript><p class="noscript">IRMAK CAFE · Menü ve iletişim bilgileri için JavaScript gereklidir.</p></noscript>
<script>
/*
 * IRMAK CAFE — MERKEZİ AYARLAR
 * ---------------------------------------------------------------
 * Sitedeki bütün işletme bilgisi buradan gelir. Boş bırakılan alan
 * sitede görünmez. Menü ve fotoğraflar şu an ÖRNEKTİR (menu.sample).
 */
window.IRMAK_CONFIG = {
  site: {
    url: "",                        // örn. "https://irmakcafe.com"
    title: "IRMAK CAFE",
    description: "IRMAK CAFE — çay, kahve, kahvaltı ve tatlı. Menü, iletişim ve çalışma saatleri.",
    ogImage: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/bg_1.jpg"
  },

  business: {
    name: "IRMAK CAFE",
    schemaType: "CafeOrCoffeeShop",
    priceRange: "₺₺",
    servesCuisine: ["Kahve", "Çay", "Kahvaltı", "Tatlı"]
  },

  contact: {
    phone: "0554 127 08 58",
    whatsapp: "",                   // WhatsApp hattı (aynı numaraysa buraya da yazın)
    whatsappMessage: "Merhaba IRMAK CAFE,",
    email: ""
  },

  location: {
    street: "", district: "", city: "", postalCode: "", country: "TR",
    lat: null, lng: null,
    mapsUrl: "",                    // Google Maps paylaşım linki
    directionsNote: ""
  },

  /* "HH:MM" biçiminde; gece yarısını geçen kapanış olur (["09:00","01:00"]).
     Kapalı gün: []. Bilinmiyorsa null bırakın. */
  hours: {
    timezone: "Europe/Istanbul",
    week: { mon: null, tue: null, wed: null, thu: null, fri: null, sat: null, sun: null },
    note: ""
  },

  social: {
    instagram: "irmakcafe58",
    googleBusiness: ""
  },

  /* Görseller: şu an ücretsiz stok fotoğraflardır (IRMAK'a ait değildir) ve
     jsDelivr üzerinden yüklenir. Kendi fotoğraflarınızı repoya yükleyip
     linkleri "img/hero.jpg" gibi dosya yollarıyla değiştirin. */
  media: {
    hero: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/bg_1.jpg",
    heroMobile: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/bg_1.jpg",
    heroVideo: "",                  // resmî reel web'e hazırlanınca: "assets/video/irmak-9x16.mp4"
    heroVideoWebm: "",
    reveal: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/carousel-1.jpg",        // kaydırdıkça ekranı dolduran görsel
    revealMobile: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/carousel-1.jpg",
    reel: "https://www.instagram.com/reel/Dc_QLodtUZn/?stkn=NGhmemgxdzVmNWUy"
  },

  /* Galeri: 6 kare, sabit bir kompozisyona yerleşir (sıra önemlidir). */
  gallery: [
    { src: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/carousel-2.jpg", alt: "Kahve çekirdekleri üstünde beyaz kupa", cap: "Sade" },
    { src: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/drink-9.jpg", alt: "Üç bardak milkshake", cap: "Soğuk" },
    { src: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/menu-4.jpg", alt: "Siyah fincanda latte", cap: "Latte" },
    { src: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/dessert-4.jpg", alt: "Yaban mersinli cheesecake dilimi", cap: "Tatlı" },
    { src: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/drink-6.jpg", alt: "Çilekli limonata", cap: "Limonata" },
    { src: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/dessert-3.jpg", alt: "Meyveli tart", cap: "Tart" }
  ],

  /* MENÜ — ÖRNEK (sample: true). Fiyatlar temsilidir. */
  menu: {
    sample: true,
    note: "",
    signature: [
      { name: "Irmak Latte", kicker: "Evin kahvesi", desc: "Çift shot espresso, kadife süt ve bir tutam tarçın. Ağır, sıcak, acelesiz.", price: 140, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/menu-1.jpg", imageAlt: "Latte, köpüğünde süt deseni" },
      { name: "Buzlu Latte", kicker: "Bardakta bir ırmak", desc: "Espresso buzun üstünden soğuk süte akar; iki renk yavaşça birbirine karışır.", price: 135, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/menu-3.jpg", imageAlt: "Uzun bardakta buzlu latte" },
      { name: "Pazar Pankeki", kicker: "Uzun kahvaltılar için", desc: "Kat kat pankek, taze meyve ve akçaağaç şurubu. Yanına bir demlik çay.", price: 220, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/dessert-2.jpg", imageAlt: "Meyveli pankek" }
    ],
    categories: [
      { id: "sicak", name: "Çay & Sıcak", items: [
        { name: "Çay", desc: "Demli, ince belli bardakta.", price: 25 },
        { name: "Demlik çay", desc: "İki kişilik; masaya demlikle.", price: 110 },
        { name: "Türk kahvesi", desc: "Bol köpüklü, yanında su ve lokum.", price: 85 },
        { name: "Dibek kahvesi", desc: "Taşta dövülmüş, yumuşak içim.", price: 95 },
        { name: "Menengiç kahvesi", desc: "Sütlü, hafif fıstıksı.", price: 95 },
        { name: "Salep", desc: "Tarçınla; kış akşamlarına.", price: 120 },
        { name: "Sıcak çikolata", desc: "Koyu ve kadifemsi.", price: 130 } ] },
      { id: "kahve", name: "Kahve", items: [
        { name: "Espresso", desc: "Tek ya da çift shot.", price: 75, image: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/service-2.jpg" },
        { name: "Americano", desc: "Espresso ve sıcak su; sade, uzun.", price: 100, image: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/menu-1.jpg" },
        { name: "Latte", desc: "Espresso, buharda ısıtılmış süt.", price: 125, image: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/menu-2.jpg" },
        { name: "Cappuccino", desc: "Eşit ölçü espresso, süt ve köpük.", price: 125, image: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/menu-3.jpg" },
        { name: "Flat white", desc: "Çift shot, ince köpük.", price: 135, image: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/service-3.jpg" },
        { name: "Filtre kahve", desc: "Günün çekirdeği, elde demleme.", price: 110, image: "https://cdn.jsdelivr.net/gh/themewagon/Koppee@main/img/service-1.jpg" },
        { name: "Mocha", desc: "Espresso, çikolata, süt.", price: 140 } ] },
      { id: "soguk", name: "Soğuk", items: [
        { name: "Buzlu latte", desc: "Espresso, soğuk süt, buz.", price: 135, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/menu-3.jpg" },
        { name: "Soğuk demleme", desc: "Uzun saatler soğukta demlenir.", price: 130 },
        { name: "Limonata", desc: "Taze sıkım limon, nane.", price: 90, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/drink-6.jpg" },
        { name: "Taze portakal suyu", desc: "Sıkma, katkısız.", price: 110, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/drink-1.jpg" },
        { name: "Milkshake", desc: "Çilek, çikolata ya da vanilya.", price: 145, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/drink-9.jpg" } ] },
      { id: "kahvalti", name: "Kahvaltı", items: [
        { name: "Serpme kahvaltı", desc: "İki kişilik: peynirler, zeytin, reçeller, yumurta, sınırsız çay.", price: 950, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/image_4.jpg" },
        { name: "Menemen", desc: "Soğanlı ya da soğansız; karar sizin.", price: 210 },
        { name: "Sucuklu yumurta", desc: "Sahanda, yanında köy ekmeği.", price: 250 },
        { name: "Kaşarlı tost", desc: "Ekşi mayalı ekmekte.", price: 170 },
        { name: "Pankek", desc: "Meyve ve akçaağaç şurubu.", price: 220, image: "https://cdn.jsdelivr.net/gh/themewagon/klassy-cafe@main/assets/images/menu-item-02.jpg" } ] },
      { id: "tatli", name: "Tatlı", items: [
        { name: "Frambuaz soslu cheesecake", desc: "Yoğun, serin; üstünde sıcak sos.", price: 210, image: "https://cdn.jsdelivr.net/gh/themewagon/klassy-cafe@main/assets/images/menu-item-04.jpg" },
        { name: "Yaban mersinli cheesecake", desc: "Taze nane ile.", price: 210, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/dessert-4.jpg" },
        { name: "Brownie", desc: "Sıcak servis, isteğe dondurmalı.", price: 170, image: "https://cdn.jsdelivr.net/gh/themewagon/klassy-cafe@main/assets/images/menu-item-01.jpg" },
        { name: "Meyveli tart", desc: "Mevsim meyveleri, vanilyalı krema.", price: 180, image: "https://cdn.jsdelivr.net/gh/themewagon/coffee1@master/images/dessert-3.jpg" },
        { name: "Muffin", desc: "Günün çeşidi.", price: 120, image: "https://cdn.jsdelivr.net/gh/themewagon/klassy-cafe@main/assets/images/menu-item-05.jpg" },
        { name: "Fırın sütlaç", desc: "Soğuk servis, tarçınlı.", price: 130 } ] }
    ]
  },

  copy: {
    heroLead: "Demli çay, özenle hazırlanmış kahve ve acele etmeyen sohbetler.",
    story: [
      "Irmak aynı yatakta akar ama suyu hiçbir zaman aynı değildir. Burada da masa aynı masa, fincan aynı fincan; değişen, her gelişte başka türlü akan zamandır.",
      "Kimi gün bir kahve kadar kısa, kimi gün bir sohbet kadar uzun. Saatler, derler ya, burada su gibi akar."
    ]
  }
};
</script>
<script>
/* IRMAK CAFE — schema.org yapılandırılmış veri (tarayıcı + Node build ortak)
   Yalnızca config.js'te GERÇEKTEN dolu olan alanlardan üretir. */
(function (root, factory) {
  if (typeof module === "object" && module.exports) module.exports = factory();
  else root.IRMAK_SCHEMA = factory();
})(typeof self !== "undefined" ? self : this, function () {
  "use strict";
  const has = (v) => v !== undefined && v !== null && !(typeof v === "string" && v.trim() === "") && !(Array.isArray(v) && v.length === 0);
  const clean = (o) => Object.fromEntries(Object.entries(o).filter(([, v]) => has(v)));
  const httpUrl = (u) => (has(u) && /^https?:\/\//i.test(String(u).trim()) ? String(u).trim() : "");
  const DAYS = ["mon", "tue", "wed", "thu", "fri", "sat", "sun"];
  const EN = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"];
  function e164(raw) {
    if (!has(raw)) return "";
    let d = String(raw).replace(/\D/g, "");
    if (d.startsWith("90") && d.length === 12) d = d.slice(2);
    if (d.startsWith("0") && d.length === 11) d = d.slice(1);
    return d.length === 10 ? "+90" + d : "+" + d;
  }
  return function buildSchema(C) {
    C = C || {};
    const site = C.site || {}, B = C.business || {}, CT = C.contact || {}, L = C.location || {}, S = C.social || {}, H = C.hours || {}, M = C.menu || {};
    const base = httpUrl(site.url).replace(/\/+$/, "");
    const ld = { "@context": "https://schema.org", "@type": B.schemaType || "CafeOrCoffeeShop", name: B.name || "IRMAK CAFE" };
    if (base) ld.url = base + "/";
    if (has(CT.phone)) ld.telephone = e164(CT.phone);
    if (has(CT.email) && /^[^@\s]+@[^@\s]+\.[^@\s]+$/.test(CT.email)) ld.email = CT.email;
    if (has(B.priceRange)) ld.priceRange = B.priceRange;
    if (Array.isArray(B.servesCuisine) && B.servesCuisine.length) ld.servesCuisine = B.servesCuisine;
    if (has(B.foundingYear)) ld.foundingDate = String(B.foundingYear);
    if (base && has(site.ogImage)) ld.image = /^https?:/.test(site.ogImage) ? site.ogImage : base + "/" + String(site.ogImage).replace(/^\//, "");
    if (has(L.street) || has(L.city)) ld.address = clean({ "@type": "PostalAddress", streetAddress: [L.street, L.district].filter(has).join(", "), addressLocality: L.district || L.city, addressRegion: L.city, postalCode: L.postalCode, addressCountry: L.country });
    if (typeof L.lat === "number" && typeof L.lng === "number") ld.geo = { "@type": "GeoCoordinates", latitude: L.lat, longitude: L.lng };
    if (httpUrl(L.mapsUrl)) ld.hasMap = httpUrl(L.mapsUrl);
    const ig = has(S.instagram) ? `https://www.instagram.com/${String(S.instagram).replace(/^@/, "").replace(/[^A-Za-z0-9._]/g, "")}/` : "";
    const same = [ig, httpUrl(S.googleBusiness), has(S.tiktok) ? `https://www.tiktok.com/@${String(S.tiktok).replace(/^@/, "")}` : ""].filter(Boolean);
    if (same.length) ld.sameAs = same;
    const week = H.week || {};
    const spec = [];
    DAYS.forEach((d, i) => (Array.isArray(week[d]) ? week[d] : []).forEach((s) => {
      if (Array.isArray(s) && /^\d{2}:\d{2}$/.test(s[0]) && /^\d{2}:\d{2}$/.test(s[1])) spec.push({ "@type": "OpeningHoursSpecification", dayOfWeek: "https://schema.org/" + EN[i], opens: s[0], closes: s[1] });
    }));
    if (spec.length) ld.openingHoursSpecification = spec;
    const cats = (Array.isArray(M.categories) ? M.categories : []).filter((c) => c && has(c.name) && Array.isArray(c.items) && c.items.length);
    if (cats.length) {
      ld.hasMenu = clean({ "@type": "Menu", url: base ? base + "/#menu" : "", hasMenuSection: cats.map((c) => ({ "@type": "MenuSection", name: c.name,
        hasMenuItem: c.items.filter((it) => it && has(it.name)).map((it) => clean({ "@type": "MenuItem", name: it.name, description: it.desc,
          offers: it.price !== null && it.price !== undefined && it.price !== "" && !isNaN(Number(it.price)) ? { "@type": "Offer", price: String(Number(it.price)), priceCurrency: "TRY" } : null })) })) });
    }
    return ld;
  };
});
</script>
<script>
/* =====================================================================
   IRMAK CAFE — davranış (premium · editoryal)
   İşletme verisi yalnızca config.js'ten gelir; DOM'a yalnızca
   textContent / setAttribute ile yazılır. Kaydırma yerel kalır
   (kaydırma kaçırma yok); efektler yalnızca transform / clip-path.
   ===================================================================== */
(() => {
  "use strict";
  const C = window.IRMAK_CONFIG || {};
  const doc = document.documentElement;
  const $ = (s, r = document) => r.querySelector(s);
  const $$ = (s, r = document) => Array.from(r.querySelectorAll(s));
  const mqMobile = matchMedia("(max-width: 860px)");
  const fine = matchMedia("(hover: hover) and (pointer: fine)").matches;
  const reduced = matchMedia("(prefers-reduced-motion: reduce)").matches;
  const clamp = (v, a, b) => Math.min(b, Math.max(a, v));
  const ease = (t) => 1 - Math.pow(1 - t, 3);

  function h(tag, attrs, ...kids) {
    const el = document.createElement(tag);
    if (attrs) for (const [k, v] of Object.entries(attrs)) {
      if (v === null || v === undefined || v === false) continue;
      if (k === "class") el.className = v;
      else if (k.startsWith("on") && typeof v === "function") el.addEventListener(k.slice(2), v);
      else el.setAttribute(k, v === true ? "" : String(v));
    }
    for (const kid of kids.flat(Infinity)) {
      if (kid === null || kid === undefined || kid === false || kid === "") continue;
      el.append(kid.nodeType ? kid : document.createTextNode(String(kid)));
    }
    return el;
  }
  const has = (v) => v !== undefined && v !== null && !(typeof v === "string" && v.trim() === "") && !(Array.isArray(v) && v.length === 0);
  const fill = (el, ...kids) => el.replaceChildren(...kids.flat(Infinity).filter((k) => k !== null && k !== undefined && k !== false && k !== ""));
  function safeUrl(u) {
    if (!has(u)) return "";
    const s = String(u).trim();
    if (/^data:(video|image)\/[a-z0-9.+-]+;base64,/i.test(s)) return s;
    if (/^(https?:)?\/\//i.test(s) || /^(tel|mailto):/i.test(s)) return s;
    if (/^[#./a-z0-9_-]/i.test(s) && !/^[a-z][a-z0-9+.-]*:/i.test(s)) return s;
    return "";
  }
  const pad = (n) => String(n).padStart(2, "0");

  /* ------------------------------------------------------------ iletişim verisi */
  const CT = C.contact || {}, L = C.location || {}, S = C.social || {}, MD = C.media || {};
  function phoneParts(raw) {
    if (!has(raw)) return null;
    let d = String(raw).replace(/\D/g, "");
    if (d.startsWith("90") && d.length === 12) d = d.slice(2);
    if (d.startsWith("0") && d.length === 11) d = d.slice(1);
    if (d.length === 10) return { e164: "+90" + d, wa: "90" + d, text: `0${d.slice(0, 3)} ${d.slice(3, 6)} ${d.slice(6, 8)} ${d.slice(8)}` };
    return { e164: "+" + d, wa: d, text: String(raw).trim() };
  }
  const phone = phoneParts(CT.phone), wa = phoneParts(CT.whatsapp);
  const igHandle = has(S.instagram) ? String(S.instagram).replace(/^@/, "").replace(/[^A-Za-z0-9._]/g, "") : "";
  const igHref = igHandle ? `https://www.instagram.com/${igHandle}/` : "";
  const addrLine = [L.street, L.district].filter(has).join(", "), addrCity = [L.postalCode, L.city].filter(has).join(" ");
  const mapsHref = safeUrl(L.mapsUrl) || ((typeof L.lat === "number" && typeof L.lng === "number") ? `https://www.google.com/maps/search/?api=1&query=${L.lat},${L.lng}` :
    (addrLine || addrCity) ? `https://www.google.com/maps/search/?api=1&query=${encodeURIComponent(["IRMAK CAFE", addrLine, addrCity].filter(has).join(", "))}` : "");

  /* ------------------------------------------------------------ saatler (Türkçe ekler) */
  const UNITS = ["", "bir", "iki", "üç", "dört", "beş", "altı", "yedi", "sekiz", "dokuz"], TENS = ["", "on", "yirmi", "otuz", "kırk", "elli"];
  const spoken = (n) => (n === 0 ? "sıfır" : n % 10 ? UNITS[n % 10] : TENS[Math.floor(n / 10)]);
  function suffix(x, kind) {
    const [hh, mm] = x.split(":").map(Number), w = spoken(mm ? mm : hh), v = w.match(/[aeıioöuü]/g) || ["e"], back = /[aıou]/.test(v[v.length - 1]);
    return kind === "dat" ? (/[aeıioöuü]$/.test(w) ? "y" : "") + (back ? "a" : "e") : (/[çfhkpsşt]$/.test(w) ? "t" : "d") + (back ? "a" : "e");
  }
  const fmtT = (x) => x.replace(":", "."), toMin = (x) => { const [a, b] = x.split(":").map(Number); return a * 60 + b; };
  const DAYS = ["mon", "tue", "wed", "thu", "fri", "sat", "sun"];
  const DAY_TR = { mon: "Pazartesi", tue: "Salı", wed: "Çarşamba", thu: "Perşembe", fri: "Cuma", sat: "Cumartesi", sun: "Pazar" };
  const H = C.hours || {}, week = H.week || {}, TZ = H.timezone || "Europe/Istanbul";
  const valid = (s) => Array.isArray(s) && s.length === 2 && /^\d{2}:\d{2}$/.test(s[0]) && /^\d{2}:\d{2}$/.test(s[1]);
  const spans = (d) => (Array.isArray(week[d]) ? week[d] : null);
  const hoursKnown = DAYS.some((d) => Array.isArray(week[d]));
  function now() {
    const map = { Mon: 0, Tue: 1, Wed: 2, Thu: 3, Fri: 4, Sat: 5, Sun: 6 };
    try { const p = Object.fromEntries(new Intl.DateTimeFormat("en-GB", { timeZone: TZ, weekday: "short", hour: "2-digit", minute: "2-digit", hourCycle: "h23" }).formatToParts(new Date()).map((x) => [x.type, x.value])); return { day: map[p.weekday], min: +p.hour * 60 + +p.minute }; }
    catch (e) { const d = new Date(); return { day: (d.getDay() + 6) % 7, min: d.getHours() * 60 + d.getMinutes() }; }
  }
  function status() {
    if (!hoursKnown) return null;
    const n = now(), today = DAYS[n.day], yest = DAYS[(n.day + 6) % 7];
    for (const s of (spans(yest) || []).filter(valid)) { const o = toMin(s[0]), c = toMin(s[1]); if (c <= o && n.min < c) return { open: true, text: `Şu an açık · ${fmtT(s[1])}’${suffix(s[1], "dat")} kadar` }; }
    for (const s of (spans(today) || []).filter(valid)) { const o = toMin(s[0]), c = toMin(s[1]); if ((c > o && n.min >= o && n.min < c) || (c <= o && n.min >= o)) return { open: true, text: `Şu an açık · ${fmtT(s[1])}’${suffix(s[1], "dat")} kadar` }; }
    for (let k = 0; k < 7; k++) { const d = DAYS[(n.day + k) % 7];
      for (const s of (spans(d) || []).filter(valid).sort((a, b) => toMin(a[0]) - toMin(b[0]))) { if (k === 0 && toMin(s[0]) <= n.min) continue;
        return { open: false, text: `Şu an kapalı · ${k === 0 ? "bugün" : k === 1 ? "yarın" : DAY_TR[d]} ${fmtT(s[0])}’${suffix(s[0], "loc")} açılıyor` }; } }
    return { open: false, text: "Şu an kapalı" };
  }
  const spanText = (d) => { const s = spans(d); if (s === null) return "—"; const v = s.filter(valid); return v.length ? v.map((x) => `${fmtT(x[0])}–${fmtT(x[1])}`).join(", ") : "Kapalı"; };

  /* ------------------------------------------------------------ temel bağlantılar */
  function wire() {
    $$("[data-tel]").forEach((a) => { if (phone) a.href = "tel:" + phone.e164; });
    $$("[data-phone-text]").forEach((s) => { s.textContent = phone ? phone.text : "İletişim"; });
    const big = $("[data-phone-big]"); if (big) big.textContent = phone ? phone.text : "";
    $$("[data-ig]").forEach((a) => { if (igHref) a.href = igHref; else a.hidden = true; });
    $$("[data-ig-text]").forEach((s) => { s.textContent = igHandle ? "@" + igHandle : "Instagram"; });
    tickStatus();
    const cr = $("[data-copyright]"); if (cr) cr.textContent = `© ${new Date().getFullYear()} ${C.business?.name || "IRMAK CAFE"}`;
    const lead = $('[data-copy="heroLead"]'); if (lead && has(C.copy?.heroLead)) lead.textContent = C.copy.heroLead;
    const img = $("[data-hero-img]"), m = $("[data-hero-m]");
    if (img && safeUrl(MD.hero)) img.src = safeUrl(MD.hero);
    if (m && safeUrl(MD.heroMobile)) m.srcset = safeUrl(MD.heroMobile);
    const ri = $("[data-reveal-img]"), rm = $("[data-reveal-m]");
    if (ri && safeUrl(MD.reveal)) ri.src = safeUrl(MD.reveal);
    if (rm && safeUrl(MD.revealMobile)) rm.srcset = safeUrl(MD.revealMobile);
    const mp4 = safeUrl(MD.heroVideo), webm = safeUrl(MD.heroVideoWebm);
    if (mp4 || webm) {
      const v = h("video", { muted: true, autoplay: !reduced, loop: true, playsinline: true, preload: "metadata", poster: safeUrl(MD.hero) || null, "aria-hidden": "true" });
      v.muted = true; if (webm) v.append(h("source", { src: webm, type: "video/webm" })); if (mp4) v.append(h("source", { src: mp4, type: "video/mp4" }));
      $("[data-hero-media]").replaceChildren(v);
    }
  }
  function tickStatus() { const st = status(), line = $("[data-status-line]"); if (line) line.textContent = st ? st.text : (igHandle ? "@" + igHandle : ""); }
  function grain() {
    try {
      const c = document.createElement("canvas"); c.width = c.height = 200;
      const x = c.getContext("2d"), d = x.createImageData(200, 200);
      for (let i = 0; i < d.data.length; i += 4) { const v = Math.random() * 255; d.data[i] = d.data[i + 1] = d.data[i + 2] = v; d.data[i + 3] = 255; }
      x.putImageData(d, 0, 0); doc.style.setProperty("--grain", `url(${c.toDataURL("image/png")})`);
    } catch (e) { /* */ }
  }

  /* ------------------------------------------------------------ açılış perdesi */
  function curtain() {
    const done = () => { doc.classList.remove("is-loading"); doc.classList.add("is-open", "is-ready", "is-done"); };
    if (reduced || !$("[data-curtain]")) { done(); return; }
    const ready = document.fonts?.ready ? Promise.race([document.fonts.ready, new Promise((r) => setTimeout(r, 800))]) : Promise.resolve();
    ready.then(() => setTimeout(() => {
      doc.classList.add("is-open"); doc.classList.remove("is-loading");
      setTimeout(() => doc.classList.add("is-ready"), 180);
      setTimeout(() => doc.classList.add("is-done"), 1300);
    }, 1050));
  }

  /* ------------------------------------------------------------ akış: kelime kelime beliren anlatı */
  function splitWords() {
    const el = $("[data-words]"); if (!el) return [];
    const words = el.textContent.trim().split(/\s+/);
    fill(el, words.map((w, i) => [h("span", { class: "w" }, w), i < words.length - 1 ? " " : ""]));
    return $$(".w", el);
  }

  /* ------------------------------------------------------------ imza sahneleri */
  const M = C.menu || {};
  const fmtPrice = (p) => {
    if (p === null || p === undefined || p === "" || isNaN(Number(p))) return "";
    const n = Number(p);
    return (Number.isInteger(n) ? n.toLocaleString("tr-TR") : n.toLocaleString("tr-TR", { minimumFractionDigits: 2, maximumFractionDigits: 2 })) + " ₺";
  };
  const sigs = (Array.isArray(M.signature) ? M.signature : []).filter((s) => s && has(s.name));
  function renderSignatures() {
    if (!sigs.length) { $("#imza").hidden = true; return; }
    const media = $("[data-imza-media]");
    fill(media, sigs.map((s, i) => h("figure", { class: "imza__img" + (i === 0 ? " is-on" : ""), "data-i": String(i) }, safeUrl(s.image) ? h("img", { src: safeUrl(s.image), alt: "", loading: i ? "lazy" : null, decoding: "async" }) : null)),
      h("p", { class: "meta imza__count" }, h("span", { "data-imza-no": true }, "01"), ` / ${pad(sigs.length)}`));
    fill($("[data-signatures]"), sigs.map((s, i) => h("article", { class: "dish", "data-dish": String(i) },
      safeUrl(s.image) ? h("figure", { class: "dish__img" }, h("img", { src: safeUrl(s.image), alt: s.imageAlt || s.name, loading: "lazy", decoding: "async" })) : null,
      h("p", { class: "meta dish__k" }, `${pad(i + 1)} · ${s.kicker || "İmza"}`),
      h("h3", { class: "dish__name" }, s.name),
      has(s.desc) ? h("p", { class: "dish__desc" }, s.desc) : null,
      h("div", { class: "dish__foot" }, fmtPrice(s.price) ? h("span", { class: "dish__price" }, fmtPrice(s.price)) : null,
        h("a", { class: "dish__link", href: "#menu" }, "Menüde gör →"), M.sample ? h("span", { class: "dish__tag" }, "Örnek") : null))));
    const io = new IntersectionObserver((es) => es.forEach((e) => {
      if (!e.isIntersecting) return;
      const i = e.target.dataset.dish;
      $$(".imza__img", media).forEach((f) => { f.classList.toggle("was", f.classList.contains("is-on") && f.dataset.i !== i); f.classList.toggle("is-on", f.dataset.i === i); });
      const no = $("[data-imza-no]"); if (no) no.textContent = pad(+i + 1);
    }), { rootMargin: "-45% 0px -45% 0px" });
    $$("[data-dish]").forEach((d) => io.observe(d));
  }

  /* ------------------------------------------------------------ menü */
  const norm = (s) => String(s || "").toLocaleLowerCase("tr").normalize("NFD").replace(/[̀-ͯ]/g, "").replace(/ı/g, "i");
  const cats = (Array.isArray(M.categories) ? M.categories : []).filter((c) => c && has(c.name) && Array.isArray(c.items))
    .map((c, i) => ({ id: (has(c.id) ? String(c.id).replace(/[^a-z0-9-]/gi, "") : "") || "k" + i, name: c.name, items: c.items.filter((it) => it && has(it.name)) }));
  let active = cats[0]?.id, query = "";
  const listEl = $("[data-list]");
  function itemEl(it, i) {
    const img = safeUrl(it.image), price = fmtPrice(it.price);
    return h("article", { class: "item", "data-img": img || null },
      img ? h("img", { class: "item__thumb", src: img, alt: "", loading: "lazy", decoding: "async" }) : null,
      h("div", { class: "item__row" }, h("span", { class: "item__no", "aria-hidden": "true" }, pad(i + 1)), h("h3", { class: "item__name" }, it.name),
        price ? h("span", { class: "item__dots", "aria-hidden": "true" }) : null, price ? h("span", { class: "price" }, price) : null),
      has(it.desc) ? h("p", { class: "item__desc" }, it.desc) : null);
  }
  function listContent() {
    if (!cats.length) return h("p", { class: "menu__empty" }, "Menümüz çok yakında burada.");
    const grid = h("div", { class: "menu__grid" });
    if (query) {
      const q = norm(query); let n = 0;
      cats.forEach((c) => { const hits = c.items.filter((it) => norm(it.name + " " + (it.desc || "")).includes(q)); if (!hits.length) return;
        grid.append(h("p", { class: "menu__cat" }, c.name)); hits.forEach((it, i) => grid.append(itemEl(it, i))); n += hits.length; });
      return n ? grid : h("p", { class: "menu__empty" }, `“${query}” için bir sonuç bulunamadı.`);
    }
    const c = cats.find((x) => x.id === active) || cats[0];
    c.items.forEach((it, i) => grid.append(itemEl(it, i)));
    return grid;
  }
  let swapT;
  function renderList(animate) {
    clearTimeout(swapT);
    if (!animate || reduced) { fill(listEl, listContent()); return; }
    listEl.classList.add("is-swap");
    swapT = setTimeout(() => { fill(listEl, listContent()); requestAnimationFrame(() => listEl.classList.remove("is-swap")); }, 280);
  }
  function select(id) {
    if (id === active && !query) return;
    active = id; const s = $("[data-search]"); if (query && s) { s.value = ""; query = ""; }
    $$(".tab").forEach((t) => { const on = t.dataset.cat === id; t.setAttribute("aria-selected", String(on)); t.tabIndex = on ? 0 : -1; if (on && mqMobile.matches) t.scrollIntoView({ block: "nearest", inline: "center" }); });
    listEl.setAttribute("aria-labelledby", "tab-" + id); renderList(true);
  }
  function renderMenu() {
    const tabs = $("[data-tabs]");
    if (M.sample) $("[data-sample-note]").hidden = false;
    if (!cats.length) { tabs.hidden = true; $(".search").hidden = true; renderList(false); return; }
    fill(tabs, cats.map((c) => h("button", { class: "tab", type: "button", role: "tab", id: "tab-" + c.id, "aria-controls": "menu-panel", "aria-selected": String(c.id === active), tabindex: c.id === active ? "0" : "-1", "data-cat": c.id }, c.name, h("sup", null, pad(c.items.length)))));
    listEl.id = "menu-panel"; listEl.setAttribute("role", "tabpanel"); listEl.setAttribute("aria-labelledby", "tab-" + active);
    tabs.addEventListener("click", (e) => { const b = e.target.closest(".tab"); if (b) select(b.dataset.cat); });
    tabs.addEventListener("keydown", (e) => {
      const all = $$(".tab", tabs), i = all.indexOf(document.activeElement); if (i < 0) return;
      let j = null; if (e.key === "ArrowRight") j = (i + 1) % all.length; if (e.key === "ArrowLeft") j = (i - 1 + all.length) % all.length; if (e.key === "Home") j = 0; if (e.key === "End") j = all.length - 1;
      if (j !== null) { e.preventDefault(); all[j].focus(); select(all[j].dataset.cat); }
    });
    const s = $("[data-search]"); let t;
    s.addEventListener("input", () => { clearTimeout(t); t = setTimeout(() => { query = s.value.trim().slice(0, 60); $$(".tab").forEach((b) => b.setAttribute("aria-selected", String(!query && b.dataset.cat === active))); renderList(false); }, 100); });
    renderList(false);
  }
  /* masaüstü: ürünün fotoğrafı imleci izleyen bir pencerede belirir */
  function floatPreview() {
    if (!fine || reduced) return;
    const f = $("[data-float]"), im = $("[data-float-img]");
    let tx = 0, ty = 0, x = 0, y = 0, on = false, raf = 0, lastX = 0;
    const loop = () => {
      x += (tx - x) * 0.16; y += (ty - y) * 0.16;
      const r = clamp((tx - lastX) * 0.4, -8, 8); lastX = tx;
      f.style.setProperty("--fx", `${x.toFixed(1)}px`); f.style.setProperty("--fy", `${y.toFixed(1)}px`); f.style.setProperty("--fr", `${r.toFixed(2)}deg`);
      raf = on || Math.abs(tx - x) > .5 ? requestAnimationFrame(loop) : 0;
    };
    listEl.addEventListener("pointermove", (e) => {
      const it = e.target.closest(".item[data-img]");
      tx = e.clientX + 28; ty = e.clientY - 150;
      if (it) { if (im.getAttribute("src") !== it.dataset.img) im.src = it.dataset.img; if (!on) { x = tx; y = ty; } on = true; f.classList.add("is-on"); }
      else { on = false; f.classList.remove("is-on"); }
      if (!raf) raf = requestAnimationFrame(loop);
    });
    listEl.addEventListener("pointerleave", () => { on = false; f.classList.remove("is-on"); });
  }

  /* ------------------------------------------------------------ galeri */
  const gallery = (Array.isArray(C.gallery) ? C.gallery : []).filter((g) => g && safeUrl(g.src));
  let lbI = 0;
  function renderGallery() {
    if (!gallery.length) { $("#galeri").hidden = true; return; }
    fill($("[data-gallery]"), gallery.map((g, i) => h("button", { class: "shot", type: "button", "data-lb": String(i), "aria-label": `Fotoğrafı büyüt: ${g.alt || ""}`, "data-reveal": true },
      h("span", { class: "shot__img" }, h("img", { src: safeUrl(g.src), alt: g.alt || "", loading: "lazy", decoding: "async" })),
      h("span", { class: "shot__cap" }, h("span", null, `${pad(i + 1)} — ${g.cap || ""}`), h("span", null, "Büyüt")))));
  }
  function showLb(i) { lbI = (i + gallery.length) % gallery.length; const g = gallery[lbI]; const im = $("[data-lb-img]"); im.src = safeUrl(g.src); im.alt = g.alt || ""; $("[data-lb-cap]").textContent = g.alt || ""; }

  /* ------------------------------------------------------------ ziyaret */
  function renderVisit() {
    const cells = [];
    if (igHref) cells.push(h("div", { class: "info" }, h("p", { class: "info__k" }, "Instagram"), h("p", { class: "info__v" }, "@" + igHandle, h("small", null, "Duyurular ve günün lezzetleri")), h("a", { class: "btn btn--line", href: igHref, target: "_blank", rel: "noopener" }, "Takip et")));
    if (wa) cells.push(h("div", { class: "info" }, h("p", { class: "info__k" }, "WhatsApp"), h("p", { class: "info__v" }, wa.text), h("a", { class: "btn btn--line", href: `https://wa.me/${wa.wa}?text=${encodeURIComponent(CT.whatsappMessage || "Merhaba")}`, target: "_blank", rel: "noopener" }, "Mesaj yaz")));
    if (addrLine || addrCity) cells.push(h("div", { class: "info" }, h("p", { class: "info__k" }, "Adres"), h("p", { class: "info__v" }, addrLine, addrLine && addrCity ? h("br") : null, addrCity, has(L.directionsNote) ? h("small", null, L.directionsNote) : null), mapsHref ? h("a", { class: "btn btn--line", href: mapsHref, target: "_blank", rel: "noopener" }, "Yol tarifi") : null));
    const n = now();
    cells.push(h("div", { class: "info" }, h("p", { class: "info__k" }, "Saatler"),
      hoursKnown ? h("table", { class: "hours" }, h("caption", { class: "sr" }, "Haftalık çalışma saatleri"), h("tbody", null, DAYS.map((d, i) => h("tr", { class: i === n.day ? "is-today" : null }, h("th", { scope: "row" }, DAY_TR[d]), h("td", null, spanText(d))))))
        : h("p", { class: "info__v" }, "Çalışma saatleri için", h("small", null, phone ? `bizi arayın: ${phone.text}` : "Instagram hesabımıza bakın."))));
    if (phone) cells.push(h("div", { class: "info" }, h("p", { class: "info__k" }, "Telefon"), h("p", { class: "info__v" }, phone.text, h("small", null, "Sipariş ve bilgi için")), h("a", { class: "btn btn--dark", href: "tel:" + phone.e164 }, "Hemen ara")));
    fill($("[data-contact]"), cells);
    fill($("[data-foot-contact]"), phone ? h("a", { href: "tel:" + phone.e164 }, phone.text) : null, igHref ? h("a", { href: igHref, target: "_blank", rel: "noopener" }, "@" + igHandle) : null, (addrLine || addrCity) ? h("span", null, [addrLine, addrCity].filter(has).join(", ")) : null);
  }

  /* ------------------------------------------------------------ SEO */
  function seo() {
    const site = C.site || {}, base = /^https?:\/\//.test(site.url || "") ? site.url.replace(/\/+$/, "") : "";
    const canon = $("#meta-canonical"), ogu = $("#meta-og-url"), ogi = $("#meta-og-image");
    if (base) { canon.href = base + "/"; ogu.content = base + "/"; } else { canon?.remove(); ogu?.remove(); }
    if (base && has(site.ogImage)) ogi.content = base + "/" + String(site.ogImage).replace(/^\//, ""); else ogi?.remove();
    if (has(site.description)) $('meta[name="description"]').content = site.description;
    const tag = $("#ld-json"), ld = window.IRMAK_SCHEMA ? window.IRMAK_SCHEMA(C) : null;
    if (tag && ld && tag.textContent.trim() === "{}") tag.textContent = JSON.stringify(ld);
  }

  /* ------------------------------------------------------------ kaydırma sahnesi (tek döngü) */
  function scrollScenes(words) {
    const hero = $("[data-hero]"), heroImg = () => $("[data-hero-media] img, [data-hero-media] video"), word = $("[data-hero-word]");
    const ac = $("[data-acilim]"), fig = $("[data-acilim-fig]"), txt = $("[data-acilim-text]");
    const akis = $("[data-words]"), band = $("[data-band]"), rows = $$("[data-band-row]");
    const shots = () => $$(".shot__img img");
    const hdr = $("[data-hdr]"), rail = $("[data-rail]"), fab = $(".fab"), visit = $("#ziyaret");
    let lastY = scrollY, raf = 0;
    const frame = () => {
      raf = 0;
      const y = scrollY, vh = innerHeight, mob = mqMobile.matches;
      /* başlık: aşağı kaydırınca saklanır, yukarıda görünür */
      hdr.classList.toggle("is-scrolled", y > 40);
      hdr.classList.toggle("is-hidden", y > vh && y > lastY + 2 && !$("#mnav").open);
      if (y < lastY - 2) hdr.classList.remove("is-hidden");
      lastY = y;
      rail?.classList.toggle("is-on", y > vh * 0.8);
      if (fab) { const r = visit.getBoundingClientRect(); fab.classList.toggle("is-hidden", y < vh * 0.6 || (r.top < vh && r.bottom > 0)); }
      if (reduced) return;
      /* giriş: fotoğraf ve dev yazı farklı derinlikte */
      if (y < hero.offsetHeight * 1.1) {
        const im = heroImg(); if (im) im.style.setProperty("--hy", `${(y * 0.28).toFixed(1)}px`);
        word.style.setProperty("--wy", `${(-y * 0.18).toFixed(1)}px`);
      }
      /* akış: kelimeler okundukça belirir */
      if (words.length) {
        const r = akis.getBoundingClientRect();
        if (r.top < vh && r.bottom > 0) {
          const p = clamp((vh * 0.82 - r.top) / (r.height + vh * 0.25), 0, 1), N = words.length;
          words.forEach((w, i) => w.style.setProperty("--o", (0.14 + 0.86 * clamp(p * N * 1.15 - i, 0, 1)).toFixed(3)));
        }
      }
      /* açılan kare: küçük pencere ekranı doldurur */
      const ar = ac.getBoundingClientRect();
      if (ar.top < vh && ar.bottom > 0) {
        const q = clamp(-ar.top / (ar.height - vh), 0, 1), e = ease(clamp(q / 0.62, 0, 1));
        const t0 = mob ? 20 : 27, l0 = mob ? 14 : 33;
        fig.style.setProperty("--it", `${(t0 * (1 - e)).toFixed(2)}%`); fig.style.setProperty("--il", `${(l0 * (1 - e)).toFixed(2)}%`);
        fig.style.setProperty("--is", (1.3 - 0.3 * e).toFixed(3)); fig.style.setProperty("--ish", (0.5 * clamp((q - 0.55) / 0.25, 0, 1)).toFixed(3));
        txt.style.setProperty("--to", clamp((q - 0.6) / 0.2, 0, 1).toFixed(3));
      }
      /* bant: iki satır zıt yönde akar */
      const br = band.getBoundingClientRect();
      if (br.top < vh && br.bottom > 0) { const d = (vh - br.top) * 0.45; rows.forEach((r) => r.style.setProperty("--bx", `${(-(+r.dataset.bandRow) * d - (+r.dataset.bandRow < 0 ? innerWidth * 0.6 : 0)).toFixed(1)}px`)); }
      /* galeri: hafif derinlik */
      if (!mob) shots().forEach((im) => { const r = im.parentElement.getBoundingClientRect(); if (r.top < vh && r.bottom > 0) im.style.setProperty("--py", `${(((r.top + r.height / 2) - vh / 2) * -0.06).toFixed(1)}px`); });
    };
    addEventListener("scroll", () => { if (!raf) raf = requestAnimationFrame(frame); }, { passive: true });
    addEventListener("resize", () => { if (!raf) raf = requestAnimationFrame(frame); }, { passive: true });
    frame();
  }

  /* ------------------------------------------------------------ görünme, dizin, gezinme */
  function reveals() {
    const masks = $$(".h2, .menu__title, .ziyaret__title").filter((el) => el.querySelector(".mask"));
    const io = new IntersectionObserver((es) => es.forEach((e) => { if (e.isIntersecting) { e.target.classList.add("is-in", "in"); io.unobserve(e.target); } }), { rootMargin: "0px 0px -8% 0px", threshold: 0.01 });
    if (reduced) { masks.forEach((m) => m.classList.add("is-in")); return; }
    masks.forEach((m) => io.observe(m));
    const groups = new Map();
    $$("[data-reveal]").forEach((el) => {
      if (el.getBoundingClientRect().top < innerHeight * 0.95) return;
      const p = el.parentElement, k = groups.get(p) || 0; groups.set(p, k + 1);
      el.style.setProperty("--d", `${Math.min(k, 5) * 0.08}s`); el.classList.add("pre"); io.observe(el);
    });
  }
  function sections() {
    const links = $$("[data-rail-for]"), navs = $$(".nav a");
    const io = new IntersectionObserver((es) => es.forEach((e) => {
      if (!e.isIntersecting) return;
      const id = e.target.id;
      links.forEach((a) => a.classList.toggle("is-active", a.dataset.railFor === id));
      navs.forEach((a) => a.classList.toggle("is-active", a.getAttribute("href") === "#" + (id === "menu-bolum" ? "menu" : id)));
    }), { rootMargin: "-45% 0px -50% 0px" });
    ["hikaye", "imza", "menu-bolum", "galeri", "ziyaret"].forEach((id) => { const el = document.getElementById(id); if (el) io.observe(el); });
  }
  function bind() {
    const mnav = $("#mnav"), lb = $("#lb");
    document.addEventListener("click", (e) => {
      const t = e.target.closest("a, button"); if (!t) return;
      if (t.matches("[data-open-nav]")) { mnav.showModal(); return; }
      if (t.matches("[data-close-nav]")) { mnav.close(); return; }
      if (t.matches("[data-lb]")) { showLb(+t.dataset.lb); lb.showModal(); return; }
      if (t.matches("[data-lb-close]")) { lb.close(); return; }
      if (t.matches("[data-lb-next]")) { showLb(lbI + 1); return; }
      if (t.matches("[data-lb-prev]")) { showLb(lbI - 1); return; }
      const href = t.getAttribute("href") || "";
      if (href.startsWith("#") && href.length > 1) {
        const target = document.getElementById(href.slice(1)); if (!target) return;
        e.preventDefault(); if (mnav.open) mnav.close();
        const top = target.getBoundingClientRect().top + scrollY - (target.id === "menu" ? 90 : 0);
        scrollTo({ top, behavior: reduced ? "auto" : "smooth" });
        const f = target.matches("h1,h2") ? target : target.querySelector("h1,h2"); if (f) { if (!f.hasAttribute("tabindex")) f.setAttribute("tabindex", "-1"); setTimeout(() => f.focus({ preventScroll: true }), 700); }
      }
    });
    lb.addEventListener("keydown", (e) => { if (e.key === "ArrowRight") showLb(lbI + 1); if (e.key === "ArrowLeft") showLb(lbI - 1); });
  }

  function init() {
    grain(); wire(); curtain();
    const words = splitWords();
    renderSignatures(); renderMenu(); renderGallery(); renderVisit(); seo();
    reveals(); sections(); bind(); floatPreview();
    scrollScenes(words);
    setInterval(tickStatus, 60000);
  }
  if (document.readyState === "loading") document.addEventListener("DOMContentLoaded", init); else init();
})();
</script>
</body>
</html>
