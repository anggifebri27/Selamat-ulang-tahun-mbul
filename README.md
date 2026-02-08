# Selamat-ulang-tahun-mbul
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday, Sayang! 🎂</title>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #ff9a9e, #fecfef, #a8edea);
            color: #333;
            text-align: center;
            padding: 20px;
            margin: 0;
            overflow-x: hidden;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            animation: fadeIn 2s ease-in;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }
        h1 {
            font-size: 3em;
            color: #ff6b6b;
            animation: bounce 2s infinite;
            margin-bottom: 20px;
        }
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-20px); }
            60% { transform: translateY(-10px); }
        }
        .hearts {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        .heart {
            position: absolute;
            font-size: 2em;
            color: #ff4757;
            animation: float 6s infinite linear;
        }
        @keyframes float {
            0% { transform: translateY(100vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-100px) rotate(360deg); opacity: 0; }
        }
        p {
            font-size: 1.2em;
            line-height: 1.6;
            margin: 20px 0;
        }
        .birthday-date {
            font-weight: bold;
            color: #ff6b6b;
            font-size: 1.5em;
        }
        .image-slider {
            margin: 30px 0;
            overflow: hidden;
            border-radius: 15px;
        }
        .slider {
            display: flex;
            animation: slide 10s infinite;
        }
        .slider img {
            width: 100%;
            height: 300px;
            object-fit: cover;
        }
        @keyframes slide {
            0%, 100% { transform: translateX(0); }
            33% { transform: translateX(-100%); }
            66% { transform: translateX(-200%); }
        }
        .button {
            background: linear-gradient(45deg, #ff6b6b, #ffa500);
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.3s;
            margin-top: 20px;
        }
        .button:hover {
            transform: scale(1.1);
        }
        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background: #ffd700;
            animation: confettiFall 5s infinite linear;
        }
        @keyframes confettiFall {
            0% { transform: translateY(-100vh) rotate(0deg); }
            100% { transform: translateY(100vh) rotate(360deg); }
        }
    </style>
</head>
<body>
    <div class="hearts">
        <!-- Floating hearts animation -->
        <div class="heart" style="left: 10%; animation-delay: 0s;">❤️</div>
        <div class="heart" style="left: 20%; animation-delay: 1s;">💖</div>
        <div class="heart" style="left: 30%; animation-delay: 2s;">💕</div>
        <div class="heart" style="left: 40%; animation-delay: 3s;">❤️</div>
        <div class="heart" style="left: 50%; animation-delay: 4s;">💖</div>
        <div class="heart" style="left: 60%; animation-delay: 5s;">💕</div>
        <div class="heart" style="left: 70%; animation-delay: 6s;">❤️</div>
        <div class="heart" style="left: 80%; animation-delay: 7s;">💖</div>
        <div class="heart" style="left: 90%; animation-delay: 8s;">💕</div>
    </div>
    <div class="container">
        <h1>Happy Birthday, Sayang! 🎉🎂</h1>
        <p class="birthday-date">15 Maret - Hari Spesialmu!</p>
        <p>Selamat ulang tahun yang ke-[usia], cinta! Kamu adalah alasan aku tersenyum setiap hari. Semoga tahun ini penuh dengan cinta, kebahagiaan, petualangan, dan semua impianmu tercapai. Aku sayang kamu lebih dari kata-kata bisa ungkapkan. 😘💕</p>
        <div class="image-slider">
            <div class="slider">
                <!-- Ganti dengan URL gambar pribadi Anda, misal foto bersama -->
                <img src="https://via.placeholder.com/800x300/ff9a9e/ffffff?text=Foto+Kita+1" alt="Foto Kita 1">
                <img src="https://via.placeholder.com/800x300/fecfef/ffffff?text=Foto+Kita+2" alt="Foto Kita 2">
                <img src="https://via.placeholder.com/800x300/a8edea/ffffff?text=Foto+Kita+3" alt="Foto Kita 3">
            </div>
        </div>
        <p>Klik tombol di bawah untuk kejutan spesial!</p>
        <button class="button" onclick="alert('Aku sayang kamu! 🎁')">Klik Saya! 💖</button>
    </div>
    <!-- Musik latar (ganti VIDEO_ID dengan ID lagu romantis dari YouTube, misal "dQw4w9WgXcQ" untuk lagu happy birthday) -->
    <iframe width="0" height="0" src="https://www.youtube.com/embed/dQw4w9WgXcQ?autoplay=1&loop=1&playlist=dQw4w9WgXcQ" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    <script>
        // Tambah confetti effect
        function createConfetti() {
            const confetti = document.createElement('div');
            confetti.className = 'confetti';
            confetti.style.left = Math.random() * 100 + '%';
            confetti.style.animationDelay = Math.random() * 5 + 's';
            document.body.appendChild(confetti);
            setTimeout(() => confetti.remove(), 5000);
        }
        setInterval(createConfetti, 200);
    </script>
</body>
</html>
