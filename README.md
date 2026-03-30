<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Prasanna ❤️ Mani Wedding</title>

<style>
body {
    margin: 0;
    font-family: 'Georgia', serif;
    background: linear-gradient(to right, #fff8f0, #ffe6e6);
    color: #5a0f2e;
}

/* HERO */
.hero {
    background: linear-gradient(rgba(90,15,46,0.8), rgba(90,15,46,0.8)),
    url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?w=1600');
    background-size: cover;
    text-align: center;
    color: gold;
    padding: 120px 20px;
}

.hero h1 {
    font-size: 3.5rem;
    letter-spacing: 2px;
}

.hero h2 {
    font-size: 1.5rem;
}

/* COUNTDOWN */
#countdown {
    margin-top: 20px;
    font-size: 1.4rem;
    font-weight: bold;
}

/* SECTION */
section {
    padding: 60px 20px;
    text-align: center;
}

/* COUPLE IMAGE */
.couple img {
    width: 300px;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.3);
    margin-top: 20px;
}

/* MESSAGE */
.message {
    background: white;
    padding: 30px;
    border-radius: 20px;
    max-width: 750px;
    margin: auto;
    line-height: 1.8;
    box-shadow: 0 5px 20px rgba(0,0,0,0.1);
}

/* GALLERY */
.gallery img {
    width: 250px;
    margin: 10px;
    border-radius: 15px;
    transition: 0.3s;
}

.gallery img:hover {
    transform: scale(1.05);
}

/* FLOWERS */
.flower {
    position: fixed;
    top: -10px;
    font-size: 24px;
    animation: fall linear infinite;
}

@keyframes fall {
    to {
        transform: translateY(100vh);
    }
}

/* FOOTER */
footer {
    background: maroon;
    color: gold;
    padding: 15px;
}
</style>
</head>

<body>

<!-- MUSIC -->
<audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-romantic.mp3" type="audio/mpeg">
</audio>

<!-- HERO -->
<div class="hero">
    <h1>Prasanna ❤️ Mani</h1>
    <h2>A Royal Wedding Celebration</h2>
    <p id="countdown"></p>
</div>

<!-- COUPLE IMAGE -->
<section class="couple">
    <h2>💑 Made For Each Other</h2>
    <img src="https://images.unsplash.com/photo-1522673607200-164d1b6ce486?w=500" alt="Couple Image">
</section>

<!-- MESSAGE -->
<section>
    <h2>💌 My Heartfelt Wishes</h2>

    <div class="message">
        <p>Dear Akka Prasanna & Bava Mani,</p>

        <p>
        From my childhood till today, you have always been my strength, my guide,
        and my best friend, Akka. Seeing you step into this beautiful new journey
        fills my heart with happiness and pride.
        </p>

        <p>
        Bava, thank you for coming into our family and for taking such loving care
        of my Akka. You both truly complete each other.
        </p>

        <p>
        I wish you both endless love, happiness, success, and laughter.
        May your life together be filled with unforgettable memories
        and a bond that grows stronger every single day.
        </p>

        <p><b>❤️ Forever with love ❤️</b><br>
        — Anneda Raghu Vardhan Reddy</p>
    </div>
</section>

<!-- GALLERY -->
<section>
    <h2>📸 Beautiful Moments</h2>

    <div class="gallery">
        <img src="https://images.unsplash.com/photo-1519741497674-611481863552?w=500">
        <img src="https://images.unsplash.com/photo-1537634066038-aca1d26f2c62?w=500">
        <img src="https://images.unsplash.com/photo-1529636798458-92182e662485?w=500">
    </div>
</section>

<footer>
    <p>Made with ❤️ for Prasanna & Mani Wedding</p>
</footer>

<!-- COUNTDOWN -->
<script>
const weddingDate = new Date("May 3, 2026 18:00:00").getTime();

setInterval(() => {
    const now = new Date().getTime();
    const gap = weddingDate - now;

    const d = Math.floor(gap / (1000 * 60 * 60 * 24));
    const h = Math.floor((gap % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const m = Math.floor((gap % (1000 * 60 * 60)) / (1000 * 60));
    const s = Math.floor((gap % (1000 * 60)) / 1000);

    document.getElementById("countdown").innerText =
    `${d} Days ${h} Hours ${m} Minutes ${s} Seconds`;
}, 1000);

/* FLOWERS */
for(let i=0;i<20;i++){
    let flower=document.createElement("div");
    flower.innerHTML="🌸";
    flower.className="flower";
    flower.style.left=Math.random()*100+"vw";
    flower.style.animationDuration=(4+Math.random()*6)+"s";
    document.body.appendChild(flower);
}
</script>

</body>
</html>
