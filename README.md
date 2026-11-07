<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>The Grill House | Premium Menu</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --gold: #d5ad65;
  --black: #10100e;
  --card: #1b1a17;
  --muted: #aaa49a;
}

body {
  background: var(--black);
  color: #f5f1e9;
  font-family: Georgia, serif;
}

/* HERO */

.hero {
  min-height: 340px;
  background:
    linear-gradient(
      rgba(0,0,0,.35),
      rgba(0,0,0,.85)
    ),
    url("https://images.unsplash.com/photo-1550547660-d9450f859349?w=1400&auto=format&fit=crop")
    center 52% / cover;

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 40px 20px;
}

.logo {
  color: var(--gold);
  font-size: 13px;
  letter-spacing: 6px;
  margin-bottom: 16px;
}

.hero h1 {
  font-size: clamp(36px, 7vw, 65px);
  letter-spacing: 5px;
}

.hero p {
  color: #ddd0b9;
  margin-top: 14px;
  font-size: 15px;
}

/* INTRO */

.intro {
  text-align: center;
  padding: 35px 20px 15px;
}

.intro h2 {
  color: var(--gold);
  font-size: 25px;
  font-weight: normal;
}

.intro p {
  color: var(--muted);
  margin-top: 10px;
  font-family: Arial, sans-serif;
  font-size: 13px;
}

/* MENU */

main {
  width: min(1100px, 92%);
  margin: 0 auto;
  padding: 25px 0 60px;
}

.section-title {
  color: var(--gold);
  font-size: 25px;
  font-weight: normal;
  letter-spacing: 3px;
  margin: 35px 0 20px;
  padding-bottom: 12px;
  border-bottom: 1px solid #4a3c27;
}

.menu-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 22px;
}

.card {
  background: var(--card);
  border: 1px solid #302a20;
  border-radius: 9px;
  overflow: hidden;
  transition: transform .2s, border-color .2s;
}

.card:hover {
  transform: translateY(-5px);
  border-color: var(--gold);
}

.card img {
  width: 100%;
  height: 190px;
  object-fit: cover;
  display: block;
}

.card-content {
  padding: 19px;
}

.card h3 {
  font-size: 18px;
  font-weight: normal;
  margin-bottom: 9px;
}

.description {
  color: var(--muted);
  font-family: Arial, sans-serif;
  font-size: 13px;
  line-height: 1.6;
  min-height: 42px;
}

.card-bottom {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 10px;
  margin-top: 17px;
}

.price {
  color: var(--gold);
  font-size: 19px;
  font-weight: bold;
}

.tag {
  color: var(--gold);
  font-size: 10px;
  letter-spacing: 1px;
  border: 1px solid #70562f;
  padding: 5px 8px;
  border-radius: 3px;
}

/* FOOTER */

footer {
  background: #191713;
  border-top: 1px solid #403421;
  text-align: center;
  padding: 35px 20px;
}

footer h2 {
  color: var(--gold);
  letter-spacing: 4px;
  font-size: 19px;
}

footer p {
  color: var(--muted);
  font-family: Arial, sans-serif;
  font-size: 12px;
  margin-top: 12px;
}

.footer-note {
  margin-top: 22px;
  font-size: 11px;
}

/* MOBILE */

@media (max-width: 750px) {
  .menu-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .card img {
    height: 155px;
  }
}

@media (max-width: 480px) {
  .menu-grid {
    grid-template-columns: 1fr;
  }

  .card img {
    height: 210px;
  }

  .hero {
    min-height: 280px;
  }
}
</style>
</head>

<body>

<header class="hero">
  <div class="logo">EST. 2026</div>
  <h1>THE GRILL HOUSE</h1>
  <p>Fresh food. Good company. Every day.</p>
</header>

<section class="intro">
  <h2>Our Signature Menu</h2>
  <p>PREPARED WITH PASSION. SERVED WITH PRIDE.</p>
</section>

<main>

  <h2 class="section-title">BURGERS</h2>

  <div class="menu-grid">

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?w=700&auto=format&fit=crop"
        alt="Classic cheeseburger"
      >
      <div class="card-content">
        <h3>Classic Burger</h3>
        <p class="description">
          Juicy beef patty, lettuce, tomato and house sauce.
        </p>
        <div class="card-bottom">
          <span class="price">$10.99</span>
          <span class="tag">CLASSIC</span>
        </div>
      </div>
    </article>

    <article class="card">
      <img
  src="images/double-cheeseburger.avif"
  alt="Double cheeseburger"
      >
      <div class="card-content">
        <h3>Double Cheeseburger</h3>
        <p class="description">
          Two beef patties, melted cheese and toasted buns.
        </p>
        <div class="card-bottom">
          <span class="price">$13.99</span>
          <span class="tag">POPULAR</span>
        </div>
      </div>
    </article>

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1550547660-d9450f859349?w=700&auto=format&fit=crop"
        alt="Gourmet BBQ burger"
      >
      <div class="card-content">
        <h3>BBQ Bacon Burger</h3>
        <p class="description">
          Bacon, cheddar cheese and smoky BBQ sauce.
        </p>
        <div class="card-bottom">
          <span class="price">$14.99</span>
          <span class="tag">SIGNATURE</span>
        </div>
      </div>
    </article>

  </div>

  <h2 class="section-title">SIDES</h2>

  <div class="menu-grid">

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1573080496219-bb080dd4f877?w=700&auto=format&fit=crop"
        alt="Golden French fries"
      >
      <div class="card-content">
        <h3>French Fries</h3>
        <p class="description">
          Golden crispy fries with house seasoning.
        </p>
        <div class="card-bottom">
          <span class="price">$4.49</span>
          <span class="tag">FAVORITE</span>
        </div>
      </div>
    </article>

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1639024471283-03518883512d?w=700&auto=format&fit=crop"
        alt="Onion rings"
      >
      <div class="card-content">
        <h3>Onion Rings</h3>
        <p class="description">
          Crispy golden battered onion rings.
        </p>
        <div class="card-bottom">
          <span class="price">$5.49</span>
          <span class="tag">SIDES</span>
        </div>
      </div>
    </article>

  </div>

  <h2 class="section-title">DRINKS</h2>

  <div class="menu-grid">

    <article class="card">
      <img
  src="images/lemonade.avif"
  alt="Fresh lemonade"
>
      <div class="card-content">
        <h3>Fresh Lemonade</h3>
        <p class="description">
          Refreshing lemonade served chilled.
        </p>
        <div class="card-bottom">
          <span class="price">$3.49</span>
          <span class="tag">FRESH</span>
        </div>
      </div>
    </article>

    <article class="card">
      <img
        src="https://images.unsplash.com/photo-1544145945-f90425340c7e?w=700&auto=format&fit=crop"
        alt="Cold refreshing drink"
      >
      <div class="card-content">
        <h3>Soft Drink</h3>
        <p class="description">
          Choose your favorite refreshing flavor.
        </p>
        <div class="card-bottom">
          <span class="price">$2.49</span>
          <span class="tag">DRINKS</span>
        </div>
      </div>
    </article>

  </div>

</main>

<footer>
  <h2>THE GRILL HOUSE</h2>
  <p>Fresh food. Good company. Every day.</p>
  <p>Thank you for visiting!</p>
  <p class="footer-note">
    DEMONSTRATION MENU • SAMPLE PRICES
  </p>
</footer>

</body>
</html>
