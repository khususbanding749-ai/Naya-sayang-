
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Untuk Naya Tersayang 💕</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: #0d0d0d;
            min-height: 100vh;
            width: 100%;
            overflow-x: hidden;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
            position: relative;
        }

        /* Background Blur */
        .bg-image {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('https://files.catbox.moe/vxmarw.jpg');
            background-size: cover;
            background-position: center;
            filter: blur(8px) brightness(0.4);
            z-index: -2;
            transform: scale(1.1); /* Biar pinggiran blur gak keliatan */
        }

        /* Container Hati Berjatuhan */
        .hearts-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
            overflow: hidden;
        }

        .heart {
            position: absolute;
            top: -10vh;
            font-size: 20px;
            color: #ff4d6d;
            animation: fall linear forwards;
            text-shadow: 0 0 10px rgba(255, 77, 109, 0.8);
        }

        @keyframes fall {
            to {
                transform: translateY(110vh) rotate(360deg);
            }
        }

        /* Kotak Teks Romantis */
        .romantic-card {
            background: rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.15);
            border-radius: 24px;
            padding: 30px;
            max-width: 600px;
            width: 100%;
            text-align: center;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.5);
            margin-top: 20px;
            margin-bottom: 30px;
            z-index: 10;
            animation: fadeIn 2s ease-in-out;
        }

        .romantic-card h1 {
            font-family: 'Dancing Script', cursive;
            font-size: clamp(2rem, 6vw, 3rem);
            color: #ffb3c6;
            margin-bottom: 15px;
            text-shadow: 0 0 15px rgba(255, 179, 198, 0.6);
        }

        .romantic-card p {
            font-size: clamp(0.9rem, 3vw, 1.1rem);
            color: #f8f9fa;
            line-height: 1.8;
            margin-bottom: 15px;
            text-shadow: 0 2px 4px rgba(0,0,0,0.8);
            font-weight: 300;
        }

        .romantic-card .highlight {
            color: #ff4d6d;
            font-weight: 600;
        }

        /* Galeri Foto Kolase */
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            max-width: 900px;
            width: 100%;
            padding: 10px;
            z-index: 10;
        }

        .photo-frame {
            background: #fff;
            padding: 10px 10px 30px 10px; /* Efek bingkai polaroid */
            box-shadow: 0 10px 20px rgba(0,0,0,0.5);
            border-radius: 4px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            animation: float 4s ease-in-out infinite;
        }

        .photo-frame img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 2px;
            display: block;
        }

        /* Ukuran foto di layar besar */
        .photo-frame:nth-child(1) { width: 180px; height: 240px; transform: rotate(-5deg); animation-delay: 0s; }
        .photo-frame:nth-child(2) { width: 180px; height: 240px; transform: rotate(4deg); animation-delay: 1s; margin-top: 20px; }
        .photo-frame:nth-child(3) { width: 180px; height: 240px; transform: rotate(-2deg); animation-delay: 2s; }
        .photo-frame:nth-child(4) { width: 180px; height: 240px; transform: rotate(6deg); animation-delay: 1.5s; margin-top: 15px; }
        .photo-frame:nth-child(5) { width: 180px; height: 240px; transform: rotate(-4deg); animation-delay: 0.5s; }

        /* Efek Hover */
        .photo-frame:hover {
            transform: scale(1.1) rotate(0deg);
            box-shadow: 0 15px 30px rgba(255, 77, 109, 0.3);
            z-index: 20;
        }

        /* Animasi Melayang */
        @keyframes float {
            0% { transform: translateY(0px) rotate(var(--rot)); }
            50% { transform: translateY(-10px) rotate(var(--rot)); }
            100% { transform: translateY(0px) rotate(var(--rot)); }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Responsif buat HP */
        @media (max-width: 600px) {
            .gallery { gap: 10px; }
            .photo-frame { width: 130px !important; height: 180px !important; padding: 6px 6px 20px 6px; }
            .romantic-card { padding: 20px 15px; }
        }
    </style>
</head>
<body>

    <div class="bg-image"></div>
    <div class="hearts-container" id="hearts"></div>

    <div class="romantic-card">
        <h1>Naya Tersayang...</h1>
        <p>Putra minta maaf ya, Naya. Kalau ada salah kata atau tingkah Putra yang bikin kamu sedih, Putra bener-bener nyesel dan gak pernah niat buat nyakitin kamu.</p>
        <p>Setiap detik yang kita lewatin itu <span class="highlight">berharga banget</span> buat Putra. Kamu itu alasan Putra senyum tiap hari, dan Putra gak mau kehilangan itu cuma gara-gara kesalahan kecil.</p>
        <p>Putra bikin ini semua karena Putra <span class="highlight">sayang banget sama kamu</span>. Semoga hati kamu luluh ya, dan kita bisa balik baik lagi kayak sebelumnya. I love you, Naya. 💕</p>
    </div>

    <div class="gallery">
        <div class="photo-frame" style="--rot: -5deg"><img src="https://files.catbox.moe/u37689.jpg" alt="Foto 1"></div>
        <div class="photo-frame" style="--rot: 4deg"><img src="https://files.catbox.moe/97791z.jpg" alt="Foto 2"></div>
        <div class="photo-frame" style="--rot: -2deg"><img src="https://files.catbox.moe/lidaek.jpg" alt="Foto 3"></div>
        <div class="photo-frame" style="--rot: 6deg"><img src="https://files.catbox.moe/p9xl8x.jpg" alt="Foto 4"></div>
        <div class="photo-frame" style="--rot: -4deg"><img src="https://files.catbox.moe/vxmarw.jpg" alt="Foto 5"></div>
    </div>

    <script>
        // Script buat Animasi Hati Berjatuhan
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerHTML = ['💖', '💕', '❤️', '💘', '💗'][Math.floor(Math.random() * 5)];
            
            // Posisi X random
            heart.style.left = Math.random() * 100 + 'vw';
            
            // Kecepatan jatuh random (3s - 6s)
            const duration = Math.random() * 3 + 3;
            heart.style.animationDuration = duration + 's';
            
            // Ukuran random (15px - 30px)
            heart.style.fontSize = (Math.random() * 15 + 15) + 'px';
            
            // Opacity random
            heart.style.opacity = Math.random() * 0.5 + 0.5;

            document.getElementById('hearts').appendChild(heart);

            // Hapus elemen setelah jatuh biar gak berat
            setTimeout(() => {
                heart.remove();
            }, duration * 1000);
        }

        // Bikin hati baru tiap 300ms
        setInterval(createHeart, 300);
    </script>

</body>
</html>
