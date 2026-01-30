<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Amber Smith - Blog</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;600&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet">

<style>
:root{
  --green:#7b846a;
  --light-green:#a9b39a;
  --beige:#e8cfae;
  --cream:#f5f1e8;
  --text:#4b4b4b;
}

*{margin:0;padding:0;box-sizing:border-box;}

body{
  font-family:'Montserrat', sans-serif;
  color:var(--text);
  background:#c9d0bf;
}

h1,h2,h3{font-family:'Playfair Display', serif;}
a{text-decoration:none;color:inherit;}

.container{
  width:90%;
  max-width:1100px;
  margin:auto;
}

/* HEADER */
header{
  background:white;
  padding:20px 0;
}
.nav{
  display:flex;
  justify-content:space-between;
  align-items:center;
}
.logo h1{font-size:28px;}
.logo span{font-size:12px;letter-spacing:2px;color:var(--green);}
nav ul{display:flex;gap:30px;list-style:none;font-size:13px;letter-spacing:1px;}

/* HERO */
.hero{
  background:url("https://images.unsplash.com/photo-1501004318641-b39e6451bec6") center/cover no-repeat;
  padding:120px 0;
}
.hero-box{
  background:rgba(245,241,232,0.9);
  padding:40px;
  max-width:500px;
  margin:auto;
  text-align:center;
  border:1px solid #ddd;
}
.hero-box h2{font-size:28px;margin-bottom:15px;}

.btn{
  display:inline-block;
  margin-top:15px;
  padding:10px 25px;
  background:var(--green);
  color:white;
  font-size:12px;
  letter-spacing:1px;
}

/* CATEGORY CARDS */
.categories{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
  margin:70px auto;
}
.cat{
  height:140px;
  background-size:cover;
  background-position:center;
  display:flex;
  align-items:center;
  justify-content:center;
  color:white;
  font-family:'Playfair Display';
  font-size:22px;
}

/* SUBSCRIBE STRIP */
.subscribe-strip{
  background:var(--beige);
  padding:50px 0;
  text-align:center;
}
.subscribe-strip input{
  padding:12px;
  border:none;
  margin:10px;
  width:220px;
}
.subscribe-strip button{
  padding:12px 25px;
  border:none;
  background:var(--green);
  color:white;
}

/* FEATURE SECTIONS UPGRADED */
.feature{
  display:flex;
  align-items:center;
  justify-content:center;
  gap:60px;
  margin:110px auto;
  max-width:1100px;
  padding:0 20px;
}
.feature img{
  width:50%;
  height:420px;
  object-fit:cover;
  border-radius:6px;
}
.feature-text{
  width:45%;
  background:var(--cream);
  padding:50px;
  text-align:center;
  box-shadow:0 15px 40px rgba(0,0,0,0.08);
  position:relative;
  z-index:2;
}
.feature.reverse{flex-direction:row-reverse;}
.feature:not(.reverse) .feature-text{margin-left:-60px;}
.feature.reverse .feature-text{margin-right:-60px;}

/* POPULAR POSTS */
.popular{
  background:var(--green);
  padding:70px 0;
  color:white;
  text-align:center;
}
.popular-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:30px;
  margin-top:30px;
}
.post-card{
  background:white;
  color:var(--text);
  padding-bottom:20px;
}
.post-card img{
  width:100%;
  height:200px;
  object-fit:cover;
}

/* FOOTER SUB */
.footer-sub{
  background:var(--beige);
  padding:60px 0;
  text-align:center;
}

/* SCROLL ANIMATIONS */
.fade-in{
  opacity:0;
  transform:translateY(60px);
  transition:opacity 1s ease, transform 1s ease;
}
.fade-in.show{
  opacity:1;
  transform:translateY(0);
}
.fade-left{transform:translateX(-60px);}
.fade-right{transform:translateX(60px);}

/* MOBILE */
@media(max-width:900px){
  .categories{grid-template-columns:1fr;}
  .feature{flex-direction:column;gap:30px;margin:70px auto;}
  .feature.reverse{flex-direction:column;}
  .feature img,.feature-text{width:100%;}
  .feature-text{margin:0 !important;padding:35px 25px;}
  .popular-grid{grid-template-columns:1fr;}
}
</style>
</head>

<body>

<header class="fade-in">
  <div class="container nav">
    <div class="logo">
      <h1>Amber Smith</h1>
      <span>BEAUTY • TRAVEL • LIFESTYLE</span>
    </div>
    <nav>
      <ul>
        <li>HOME</li>
        <li>ABOUT ME</li>
        <li>SHOP MY INSTA</li>
        <li>CONTACT</li>
      </ul>
    </nav>
  </div>
</header>

<section class="hero fade-in">
  <div class="hero-box">
    <h2>Introduction Goes Here</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    <a href="#" class="btn">READ MORE</a>
  </div>
</section>

<section class="container categories fade-in">
  <div class="cat" style="background-image:url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e')">Travel</div>
  <div class="cat" style="background-image:url('https://images.unsplash.com/photo-1500530855697-b586d89ba3ee')">Lifestyle</div>
  <div class="cat" style="background-image:url('https://images.unsplash.com/photo-1492724441997-5dc865305da7')">Home</div>
</section>

<section class="subscribe-strip fade-in">
  <h2>Download My Monthly Planner</h2>
  <input type="text" placeholder="Full Name">
  <input type="email" placeholder="Email Address">
  <button>SUBSCRIBE</button>
</section>

<section class="feature fade-in fade-right">
  <img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6"/>
  <div class="feature-text">
    <h3>Lorem ipsum dolor sit amet</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    <a href="#" class="btn">READ MORE</a>
  </div>
</section>

<section class="feature reverse fade-in fade-left">
  <img src="https://images.unsplash.com/photo-1500534623283-312aade485b7"/>
  <div class="feature-text">
    <h3>Lorem ipsum dolor sit amet</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    <a href="#" class="btn">READ MORE</a>
  </div>
</section>

<section class="popular fade-in">
  <div class="container">
    <h2>Popular Posts</h2>
    <div class="popular-grid">
      <div class="post-card">
        <img src="https://images.unsplash.com/photo-1492724441997-5dc865305da7"/>
        <h3>Lorem ipsum dolor</h3>
        <a class="btn">READ MORE</a>
      </div>
      <div class="post-card">
        <img src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f"/>
        <h3>Lorem ipsum dolor</h3>
        <a class="btn">READ MORE</a>
      </div>
    </div>
  </div>
</section>

<section class="footer-sub fade-in">
  <h2>Get The Latest</h2>
  <input type="text" placeholder="Full Name">
  <input type="email" placeholder="Email Address">
  <button>SUBSCRIBE</button>
</section>

<script>
const faders = document.querySelectorAll('.fade-in');

const appearOptions = {
  threshold: 0.2,
  rootMargin: "0px 0px -50px 0px"
};

const appearOnScroll = new IntersectionObserver(function(entries, observer) {
  entries.forEach(entry => {
    if (!entry.isIntersecting) return;
    entry.target.classList.add("show");
    observer.unobserve(entry.target);
  });
}, appearOptions);

faders.forEach(fader => {
  appearOnScroll.observe(fader);
});
</script>

</body>
</html>
