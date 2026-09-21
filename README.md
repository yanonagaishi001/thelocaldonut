<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>The Local Donut | Got a Nice Ring to It | Scottsdale, AZ</title>
<meta name="description" content="The Local Donut in Scottsdale, Arizona. Scratch-made specialty and traditional donuts since 2016. Order ahead online or visit us at 3213 N Hayden Rd.">
<meta name="theme-color" content="#FA934E">
<link rel="icon" href="logo.png">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@600;700&family=Figtree:wght@400;500;600;700&display=swap">
<style>
/* ---------- Tokens: change the brand here ---------- */
:root {
  --bg: #FFFCF8;        /* warm white page background */
  --ink: #141210;       /* logo black */
  --soft: #5A524C;      /* body text */
  --line: #E9E1D8;      /* thin dividers */
  --tint: #FBF3EA;      /* photo placeholders, quiet panels */
  --orange: #FA934E;    /* logo ring */
  --pink: #EF4D90;      /* logo frosting: the ring in the headline */
  --pink-text: #C9246F; /* darker pink, readable for small labels */
  --peach: #FFE9D6;     /* soft orange tint for panels */
  --blush: #FDE3EE;     /* soft pink tint */
  --display: 'Josefin Sans', 'Century Gothic', Futura, sans-serif;
  --body: 'Figtree', Helvetica, Arial, sans-serif;
  --pad: clamp(20px, 6vw, 88px);
  --max: 1160px;
}

/* ---------- Base ---------- */
*, *::before, *::after { box-sizing: border-box; }
html { scroll-behavior: smooth; }
body { margin: 0; border-top: 6px solid var(--orange); font-family: var(--body); font-size: 17px; line-height: 1.6; background: var(--bg); color: var(--ink); -webkit-font-smoothing: antialiased; }
a { color: inherit; text-decoration: none; }
a:focus-visible { outline: 3px solid var(--orange); outline-offset: 3px; border-radius: 4px; }
h1, h2, h3, p { margin: 0; }
h1, h2, h3 { font-family: var(--display); font-weight: 700; letter-spacing: -0.01em; }
h2 { font-size: clamp(30px, 3.4vw, 44px); line-height: 1.1; }
p { color: var(--soft); }
.wrap { width: 100%; max-width: calc(var(--max) + var(--pad) * 2); margin: 0 auto; padding-left: var(--pad); padding-right: var(--pad); }
.eyebrow { font-weight: 700; font-size: 14px; letter-spacing: 2px; text-transform: uppercase; color: var(--pink-text); }
.link { font-weight: 600; border-bottom: 2px solid var(--orange); padding-bottom: 2px; }
.link:hover { border-color: var(--ink); }
.photo { display: flex; align-items: center; justify-content: center; text-align: center; padding: 24px; overflow: hidden; background: var(--tint); color: var(--soft); font-weight: 500; font-size: 14px; line-height: 1.5; }
.photo img { width: 100%; height: 100%; object-fit: cover; }

/* ---------- Buttons ---------- */
.btn { display: inline-flex; align-items: center; justify-content: center; min-height: 54px; padding: 0 30px; border-radius: 999px; border: 2px solid var(--ink); font-weight: 700; font-size: 16px; white-space: nowrap; transition: background .15s ease, color .15s ease; }
.btn-solid { background: var(--orange); border-color: var(--orange); color: var(--ink); }
.btn-solid:hover { background: var(--ink); border-color: var(--ink); color: #fff; }
.btn-line:hover { background: var(--ink); color: #fff; }
.btn-small { min-height: 46px; padding: 0 22px; font-size: 15px; }

/* ---------- Nav ---------- */
.nav { display: flex; align-items: center; justify-content: space-between; min-height: 84px; }
.brand { display: flex; align-items: center; gap: 12px; font-family: var(--display); font-weight: 700; font-size: 20px; }
.brand img { width: 52px; height: 52px; }
.nav-links { display: flex; align-items: center; gap: 36px; font-weight: 500; font-size: 16px; }
.nav-links a:not(.btn) { padding: 12px 0; }
.nav-links a:not(.btn):hover { color: var(--pink-text); }

/* ---------- Hero ---------- */
.hero { display: flex; flex-direction: column; align-items: center; text-align: center; gap: 26px; padding-top: clamp(40px, 7vw, 88px); padding-bottom: clamp(40px, 5vw, 64px); }
.hero h1 { font-size: clamp(44px, 7.4vw, 100px); line-height: 1.02; letter-spacing: -0.02em; }
/* The pink ring drawn around the word "ring" */
.ring { position: relative; display: inline-block; padding: 0 0.12em; }
.ring::after { content: ""; position: absolute; left: -0.1em; right: -0.1em; top: 0.02em; bottom: -0.1em; border: 0.055em solid var(--pink); border-radius: 50%; transform: rotate(-4deg); pointer-events: none; }
.hero p { max-width: 520px; font-size: clamp(17px, 1.4vw, 19px); }
.cta-row { display: flex; flex-wrap: wrap; justify-content: center; gap: 14px; }
.hero-photo { aspect-ratio: 16 / 7; border-radius: 24px; }

/* ---------- Info strip ---------- */
.info { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 32px; margin-top: clamp(24px, 3vw, 32px); padding: 32px clamp(20px, 3vw, 40px); border-radius: 24px; background: var(--peach); }
.info h3 { margin-bottom: 6px; color: var(--pink-text); font-family: var(--body); font-size: 14px; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; }
.info p { font-size: 16px; color: var(--ink); }
.info a { text-decoration: underline; text-underline-offset: 3px; }

/* ---------- Favorites ---------- */
.section { padding-top: clamp(64px, 8vw, 112px); }
.section-head { display: flex; flex-wrap: wrap; align-items: baseline; justify-content: space-between; gap: 12px 32px; margin-bottom: 40px; }
.faves { display: grid; grid-template-columns: repeat(4, minmax(0, 1fr)); gap: 32px; }
.fave .photo { width: 100%; aspect-ratio: 1; border-radius: 50%; margin-bottom: 18px; }
.fave:nth-child(odd) .photo { background: var(--peach); }
.fave:nth-child(even) .photo { background: var(--blush); }
.fave h3 { font-size: 22px; margin-bottom: 4px; }
.fave p { font-size: 15px; line-height: 1.5; }
.also { margin-top: 40px; font-size: 16px; }

/* ---------- Roots ---------- */
.roots { display: grid; grid-template-columns: minmax(0, 1fr) minmax(0, 1fr); gap: clamp(32px, 6vw, 88px); align-items: center; }
.roots .photo { aspect-ratio: 5 / 4; border-radius: 24px; }
.roots-copy { display: flex; flex-direction: column; gap: 18px; align-items: flex-start; }

/* ---------- Visit ---------- */
.visit { display: grid; grid-template-columns: minmax(0, 1fr) minmax(0, 1fr); gap: clamp(32px, 6vw, 88px); align-items: start; }
.visit-copy { display: flex; flex-direction: column; gap: 28px; align-items: flex-start; }
.details { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 24px 32px; margin: 0; width: 100%; font-size: 16px; }
.details dt { margin-bottom: 4px; color: var(--pink-text); font-size: 14px; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; }
.details dd { margin: 0; color: var(--soft); }
.details a { text-decoration: underline; text-underline-offset: 3px; }
.map { aspect-ratio: 5 / 4; border-radius: 24px; }

/* ---------- Footer ---------- */
.footer { margin-top: clamp(64px, 8vw, 112px); background: var(--peach); }
.footer-inner { display: flex; flex-wrap: wrap; align-items: center; justify-content: space-between; gap: 20px 32px; padding-top: 36px; padding-bottom: 36px; font-size: 15px; color: var(--ink); }
.footer-brand { display: flex; align-items: center; gap: 14px; }
.footer-brand img { width: 60px; height: 60px; }
.footer-brand strong { display: block; font-family: var(--display); font-size: 18px; color: var(--ink); }
.footer nav { display: flex; flex-wrap: wrap; gap: 4px 28px; font-weight: 500; }
.footer nav a { padding: 12px 0; }
.footer nav a:hover { color: var(--pink-text); }

/* ---------- Tablet and phone ---------- */
@media (max-width: 900px) {
  .nav-links a:not(.btn) { display: none; }
  .faves { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .roots, .visit { grid-template-columns: minmax(0, 1fr); }
}
@media (max-width: 600px) {
  body { font-size: 16px; }
  .nav { min-height: 68px; }
  .brand { font-size: 16px; gap: 8px; }
  .brand img { width: 44px; height: 44px; }
  .btn-small { min-height: 44px; padding: 0 16px; font-size: 14px; }
  .cta-row { width: 100%; }
  .cta-row .btn { width: 100%; }
  .hero-photo { aspect-ratio: 4 / 3; border-radius: 18px; }
  .info { grid-template-columns: minmax(0, 1fr); gap: 20px; }
  .faves { gap: 24px 20px; }
  .fave h3 { font-size: 19px; }
  .details { grid-template-columns: minmax(0, 1fr); }
}
@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }
  .btn { transition: none; }
}
</style>
</head>
<body id="top">

<header class="wrap nav">
  <a class="brand" href="#top">
    <img src="logo.png" alt="" width="52" height="52">
    The Local Donut
  </a>
  <nav class="nav-links" aria-label="Main">
    <a href="#favorites">Donuts</a>
    <a href="#roots">Our roots</a>
    <a href="#visit">Visit</a>
    <a class="btn btn-solid btn-small" href="https://the-local-donut.square.site">Order now</a>
  </nav>
</header>

<main>

<section class="wrap hero">
  <div class="eyebrow">Scottsdale, AZ · Est. 2016</div>
  <h1>Got a nice <span class="ring">ring</span> to it.</h1>
  <p>Scratch-made donuts, fresh every morning on Hayden Road. Order ahead and your box will be waiting.</p>
  <div class="cta-row">
    <a class="btn btn-solid" href="https://the-local-donut.square.site">Order ahead</a>
    <a class="btn btn-line" href="#favorites">See the donuts</a>
  </div>
</section>

<div class="wrap">
  <!-- Add a photo: <img src="images/hero.jpg" alt="A box of donuts from above"> inside this div -->
  <div class="photo hero-photo">[ PHOTO ]<br>One wide, bright shot of the donut case or a full box</div>

  <div class="info">
    <div>
      <h3>Hours</h3>
      <p>Mon to Thu: 6am to 12pm<br>Fri to Sun: 6am to 2pm</p>
    </div>
    <div>
      <h3>Find us</h3>
      <p>3213 N Hayden Rd<br>Scottsdale, AZ 85251</p>
    </div>
    <div>
      <h3>Come early</h3>
      <p>Favorites sell out. <a href="https://the-local-donut.square.site">Order ahead</a> to lock in your box.</p>
    </div>
  </div>
</div>

<section class="wrap section" id="favorites">
  <div class="section-head">
    <h2>A few favorites</h2>
    <a class="link" href="https://the-local-donut.square.site">See today's full lineup</a>
  </div>
  <div class="faves">
    <article class="fave">
      <div class="photo">[ PHOTO ]</div>
      <h3>Crème Brûlée</h3>
      <p>[One line: custard filling, torched sugar top.]</p>
    </article>
    <article class="fave">
      <div class="photo">[ PHOTO ]</div>
      <h3>PB&amp;J</h3>
      <p>[One line description.]</p>
    </article>
    <article class="fave">
      <div class="photo">[ PHOTO ]</div>
      <h3>The Princess</h3>
      <p>Strawberry and cream. [Confirm.]</p>
    </article>
    <article class="fave">
      <div class="photo">[ PHOTO ]</div>
      <h3>Old Fashioned</h3>
      <p>Maple, chocolate, or blueberry.</p>
    </article>
  </div>
  <p class="also">Also in the case: croissant donuts, fritters, mochi balls, vegan options, kolaches, breakfast croissants, and hot or iced coffee.</p>
</section>

<section class="wrap section roots" id="roots">
  <div class="photo">[ PHOTO ]<br>The crew, or the lobby on a busy morning</div>
  <div class="roots-copy">
    <h2>Our roots</h2>
    <p>We are a neighborhood shop first. The regulars have a usual, the kids get to pick the one with sprinkles, and nobody leaves empty-handed. We have been doing it on Hayden Road since 2016.</p>
    <p>[Add two or three sentences of the shop's story here.]</p>
  </div>
</section>

<section class="wrap section visit" id="visit">
  <div class="visit-copy">
    <h2>Come see us</h2>
    <dl class="details">
      <div><dt>Address</dt><dd>3213 N Hayden Rd<br>Scottsdale, AZ 85251</dd></div>
      <div><dt>Hours</dt><dd>Mon to Thu: 6am to 12pm<br>Fri to Sun: 6am to 2pm</dd></div>
      <div><dt>Parking</dt><dd>Free lot out front. No drive-thru.</dd></div>
      <div><dt>Call</dt><dd><a href="tel:+14805005236">(480) 500-5236</a></dd></div>
    </dl>
    <a class="btn btn-line" href="https://maps.google.com/?q=3213+N+Hayden+Rd+Scottsdale+AZ+85251">Get directions</a>
  </div>
  <!-- Replace this box with a Google Maps embed iframe when going live -->
  <div class="photo map">[ MAP ]</div>
</section>

</main>

<footer class="footer">
  <div class="wrap footer-inner">
    <div class="footer-brand">
      <img src="logo.png" alt="" width="60" height="60">
      <div><strong>The Local Donut</strong>Got a nice ring to it.</div>
    </div>
    <nav aria-label="Footer">
      <a href="https://the-local-donut.square.site">Order now</a>
      <a href="#visit">Location</a>
      <a href="tel:+14805005236">Contact</a>
      <a href="https://instagram.com/thelocaldonut">Instagram</a>
    </nav>
  </div>
</footer>

</body>
</html>
