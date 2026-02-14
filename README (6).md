# v-day
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine For You 💌</title>

    <style>
        body {
            margin: 0;
            font-family: "Poppins", sans-serif;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .container {
            width: 90%;
            max-width: 500px;
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        }

        h1 {
            color: #fff;
            margin-bottom: 15px;
        }

        p {
            color: #fff;
            font-size: 18px;
            line-height: 1.6;
        }

        .emoji {
            font-size: 35px;
            margin-bottom: 15px;
        }

        button {
            margin-top: 25px;
            padding: 12px 25px;
            border: none;
            border-radius: 25px;
            background: #ff4d6d;
            color: white;
            font-size: 16px;
            cursor: pointer;
            transition: 0.3s;
        }

        button:hover {
            background: #ff1f4b;
            transform: scale(1.05);
        }

        .slide {
            display: none;
            animation: fade 0.7s;
        }

        .active {
            display: block;
        }

        @keyframes fade {
            from {opacity: 0;}
            to {opacity: 1;}
        }

        footer {
            margin-top: 15px;
            font-size: 14px;
            color: #ffe6ea;
        }
    </style>
</head>

<body>

<div class="container">

    <!-- SLIDE 1 -->
    <div class="slide active">
        <div class="emoji">💌✨</div>
        <h1>Hai Kamu...</h1>
        <p>
            Aku bikin website kecil ini khusus buat kamu.<br>
            Gak lebay, gak alay, cuma jujur dari hati 😄
        </p>
    </div>

    <!-- SLIDE 2 -->
    <div class="slide">
        <div class="emoji">😊🌸</div>
        <h1>Tentang Kamu</h1>
        <p>
            Kamu itu tipe orang yang bikin nyaman.<br>
            Gak ribet, gak drama,<br>
            tapi selalu bikin suasana jadi lebih baik.
        </p>
    </div>

    <!-- SLIDE 3 -->
    <div class="slide">
        <div class="emoji">☕📱</div>
        <h1>Jujur Ya...</h1>
        <p>
            Kadang aku senyum sendiri cuma gara-gara chat kamu.<br>
            Kayak: "Lah kok bisa ya sesimpel ini bikin happy?"
        </p>
    </div>

    <!-- SLIDE 4 -->
    <div class="slide">
        <div class="emoji">💭💖</div>
        <h1>Bukan Gombal</h1>
        <p>
            Ini bukan rayuan murahan.<br>
            Ini cuma pengakuan sederhana:<br>
            Aku nyaman sama kamu.
        </p>
    </div>

    <!-- SLIDE 5 -->
    <div class="slide">
        <div class="emoji">🌹🤍</div>
        <h1>Valentine Ini</h1>
        <p>
            Walau kita belum "apa-apa",<br>
            aku bersyukur bisa kenal kamu.<br>
            Semoga kamu selalu bahagia ✨
        </p>
    </div>

    <!-- SLIDE 6 -->
    <div class="slide">
        <div class="emoji">🥰💌</div>
        <h1>Terakhir...</h1>
        <p>
            Kalau suatu hari kamu butuh teman cerita,<br>
            teman ketawa,<br>
            atau teman ngopi...<br>
            Aku siap 😄☕
        </p>
    </div>

    <button onclick="nextSlide()">Next ➡️</button>

    <footer>
        Made with ❤️ just for you
    </footer>

</div>

<script>
    let currentSlide = 0;
    const slides = document.querySelectorAll(".slide");

    function nextSlide() {
        slides[currentSlide].classList.remove("active");
        currentSlide++;

        if (currentSlide >= slides.length) {
            currentSlide = 0;
        }

        slides[currentSlide].classList.add("active");
    }
</script>

</body>
</html>
