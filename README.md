<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  <title>CodePen - NFT Landing Page</title>
  <link rel="stylesheet" href="./style.css">

</head>
<body>
<!-- partial:index.partial.html -->
<!--! ------------------------------- Header -------------------------------- -->
<header>
  <div class="logo">LOGO</div>

  <div class="menu-items">
    <a href="#">Discover</a>
    <a href="#">Rarity</a>
    <a href="#">How It Works</a>
    <a href="#">Community</a>
    <a class="special" href="#">HostNFTs</a>
  </div>

  <div class="lang">
    <div class="lang-en">En</div>
  </div>
</header>

<!--! ---------------------------- Hero Section ----------------------------- -->
<!--# BG GIF -->
<div class="bg-gif"><video autoplay loop src="https://cdn.dribbble.com/users/2733/screenshots/15581498/media/55cb2ac35a15f1ffe8e2f1e9d979feed.mp4" alt="bg" /></div>

<!--# Hero ctr -->
<div class="ctr">
  <!--! left-ctr -->
  <div class="left-ctr">
    <div class="left-ctr-1">
      <span>
        <h1>Discover</h1>
      </span>
      <span>
        <h1>&amp; Collect</h1>
      </span>
      <span>
        <h1>Our new</h1>
      </span>
      <span>
        <h1>Holography</h1>
      </span>
      <span>
        <h1>Nft's</h1>
      </span>
    </div>
    <div class="left-ctr-2">
      <div class="left-ctr-2-1">
        <p>
          Holography are your ticket into the largest and fastest growing Online Casino Network on the Blockchain. With only 10,000 VIP members ever to be minted, Holo grant holders access to the new world
          of Defi Gambling. Holo grant proof of ownership on the Ethereum Blockchain.
        </p>
      </div>
      <div class="left-ctr-2-2">
        <span>
          <p>Twitter</p>
        </span>
        <span>
          <p>Instagram</p>
        </span>
        <span>
          <p>Discord</p>
        </span>
      </div>
    </div>
  </div>
  <div class="right-ctr">
    <div class="right-ctr-box">
      <div class="right-ctr-box-inner-1">
        <h1>Holographic Head</h1>
        <p>Last Bid</p>
      </div>
      <div class="right-ctr-box-inner-2">
        <p>#3D #holo #new</p>
        <h1>2.251ETH <img src="./ethlogo.png" width="15" alt="" /></h1>
      </div>
    </div>
  </div>
</div>
<!-- partial -->
  <script src='https://cdnjs.cloudflare.com/ajax/libs/gsap/3.11.5/gsap.min.js'></script><script  src="./script.js"></script>

</body>
</html>
<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  background-color: #020404;
  color: #eee;
  height: 100vh;
  font-family: "Poppins";
  padding-inline: clamp(1.5rem, 2vw, 2rem);
  overflow: hidden;
}
/*# Header */
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1rem;
  width: 100%;
  height: fit-content;
  position: relative;
  top: 0;
  font-size: 12px;
  padding-top: 30px;
}
header .logo {
  font-weight: bold;
}
header .menu-items {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 0.5rem;
}
header .menu-items a {
  color: #eee;
  text-decoration: none;
}
header .menu-items .special {
  background-color: #eee;
  color: #020404;
  padding: 3px 5px;
  border-radius: 0.3rem;
}
header .lang {
  display: flex;
}
/*# Hero Section */
/*? BG GIF */
.bg-gif video {
  position: absolute;
  z-index: -1;
  width: 100%;
  height: 100vh;
  object-fit: cover;
  object-position: 50% 85%;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

/*? Hero ctr */
.ctr {
  position: absolute;
  bottom: 2rem;
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
}

.left-ctr-1 h1 {
  margin: 10px 0px;
  line-height: 1.5rem;
  font-size: 50px;
  font-weight: 600;
  text-transform: uppercase;
}
.left-ctr-2 {
  display: flex;
  width: 100%;
  padding-top: 30px;
}
.left-ctr-2 .left-ctr-2-1 {
  width: 40%;
}
.left-ctr-2 .left-ctr-2-2 {
  margin: 0px 20px;
}
.left-ctr-2 .left-ctr-2-2 p {
  margin-bottom: 4px;
  text-decoration: underline;
}
.left-ctr-2 p {
  font-size: 10px;
  line-height: 170%;
  color: #a0a0a0;
}
.ctr .right-ctr {
  margin-right: 2rem;
  background-color: #eee;
  color: #020404;
  width: 500px;
  height: fit-content;
  font-size: 10px;
  padding: 15px 20px;
  border-radius: 10px;
}

.right-ctr-box {
  display: flex;
  align-items: center;
  width: 100%;
  flex-direction: column;
  height: fit-content;
}
.right-ctr-box .right-ctr-box-inner-1,
.right-ctr-box .right-ctr-box-inner-2 {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}
.right-ctr-box h1 {
  font-size: 15px;
}
.right-ctr-box p {
  font-size: 10px;
}
span {
  overflow: hidden;
  display: block;
}
</style>

<script>
const tl = gsap.timeline();
tl.from([".logo, .menu-items a, .lang"], {
  duration: 1,
  opacity: 0,
  y: 40,
  stagger: { amount: 0.4 }
})
  .from(
    ".left-ctr h1",
    { opacity: 0, duration: 1, y: 100, skewY: 10, stagger: { amount: 0.4 } },
    "-=1"
  )
  .from(
    [".left-ctr-2-1, .left-ctr-2-2"],
    { opacity: 0, duration: 1, y: 100, stagger: { amount: 0.4 } },
    "-=1"
  )
  .from(".right-ctr", { duration: 1, x: 500, skewX: 50 }, "-=1");
</script>
