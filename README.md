<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Selamat Ulang Tahun Cherry! 🧸🎂</title>

    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Google Fonts: Fredoka & Quicksand -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@500;600;700&family=Quicksand:wght@500;600;700&display=swap" rel="stylesheet">

    <style>
        :root {
            --cream-bg: #FFF9F0;
            --honey-light: #FDE68A;
            --honey-warm: #F59E0B;
            --bear-brown: #8D5B4C;
            --bear-dark: #5C3A2E;
            --blush-pink: #FBCFE8;
            --rose-soft: #F472B6;
        }

        body {
            font-family: 'Quicksand', sans-serif;
            background-color: var(--cream-bg);
            background-image:
                radial-gradient(#FDE68A 1.6px, transparent 1.6px),
                radial-gradient(#FBCFE8 1.6px, #FFF9F0 1.6px);
            background-size: 36px 36px;
            background-position: 0 0, 18px 18px;
            color: var(--bear-dark);
            overflow-x: hidden;
            min-height: 100vh;
            -webkit-tap-highlight-color: transparent;
        }

        h1, h2, h3, .font-cute {
            font-family: 'Fredoka', sans-serif;
        }

        /* Animasi Beruang Melayang Lembut */
        @keyframes floatSlow {
            0%, 100% { transform: translateY(0px) rotate(-2deg); }
            50% { transform: translateY(-10px) rotate(2deg); }
        }
        .animate-float {
            animation: floatSlow 3.4s ease-in-out infinite;
        }
        .animate-float-delay {
            animation: floatSlow 3.8s ease-in-out 1.2s infinite;
        }

        /* Animasi Kue Menggemaskan */
        @keyframes cakeBounce {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.04); }
        }
        .animate-cake {
            animation: cakeBounce 2.2s ease-in-out infinite;
        }

        /* Animasi Api Lilin */
        @keyframes candleFlicker {
            0%, 100% { transform: scale(1) rotate(-2deg); opacity: 1; }
            50% { transform: scale(1.12, 0.92) rotate(3deg); opacity: 0.9; }
        }
        .flame-glow {
            transform-origin: bottom center;
            animation: candleFlicker 0.8s infinite alternate ease-in-out;
            transition: opacity 0.3s ease, transform 0.3s ease;
        }
        .flame-out {
            opacity: 0 !important;
            transform: scale(0) !important;
            animation: none !important;
        }

        /* Animasi Asap Lilin Saat Ditiup */
        @keyframes smokeRise {
            0% { opacity: 0.85; transform: translateY(0) scale(0.8); }
            100% { opacity: 0; transform: translateY(-28px) scale(1.8); }
        }
        .smoke-puff {
            opacity: 0;
        }
        .smoke-active {
            animation: smokeRise 1s ease-out forwards;
        }

        /* Kartu Kaca Krem Hangat */
        .bear-card {
            background: rgba(255, 253, 249, 0.94);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 3px solid #F3E5D8;
            box-shadow: 0 16px 36px -12px rgba(141, 91, 76, 0.18);
        }

        /* Bingkai Foto Polaroid Telinga Beruang */
        .bear-polaroid {
            background: #FFFFFF;
            border: 3px solid #E6CCB2;
            border-radius: 1.5rem;
            padding: 0.65rem 0.65rem 1rem 0.65rem;
            box-shadow: 0 12px 24px -8px rgba(92, 58, 46, 0.16);
            position: relative;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .bear-polaroid:hover {
            transform: translateY(-6px) rotate(1deg);
            box-shadow: 0 18px 30px -8px rgba(92, 58, 46, 0.24);
        }
        /* Telinga Kiri & Kanan pada Bingkai Foto */
        .bear-polaroid::before,
        .bear-polaroid::after {
            content: '';
            position: absolute;
            top: -14px;
            width: 34px;
            height: 26px;
            background-color: #B08968;
            border: 3px solid #8D5B4C;
            border-radius: 50% 50% 0 0;
            z-index: -1;
        }
        .bear-polaroid::before {
            left: 18px;
            transform: rotate(-14deg);
        }
        .bear-polaroid::after {
            right: 18px;
            transform: rotate(14deg);
        }

        /* Animasi Masuk Halaman Ucapan */
        @keyframes popIn {
            0% { opacity: 0; transform: scale(0.92) translateY(20px); }
            100% { opacity: 1; transform: scale(1) translateY(0); }
        }
        .reveal-stage {
            animation: popIn 0.65s cubic-bezier(0.22, 1, 0.36, 1) forwards;
        }

        /* Stiker Beruang Melayang */
        @keyframes floatStickerUp {
            0% { transform: translateY(105vh) rotate(0deg) scale(0.8); opacity: 0; }
            15% { opacity: 1; }
            85% { opacity: 1; }
            100% { transform: translateY(-15vh) rotate(25deg) scale(1.1); opacity: 0; }
        }
        .floating-sticker {
            position: fixed;
            bottom: -60px;
            pointer-events: none;
            z-index: 30;
            animation: floatStickerUp linear forwards;
        }

        /* Kursor Efek Ketik */
        .typing-cursor::after {
            content: '🐾';
            font-size: 0.9em;
            margin-left: 4px;
            animation: blinkPaw 0.9s infinite;
        }
        @keyframes blinkPaw {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0.2; }
        }
    </style>
</head>
<body class="flex flex-col items-center justify-center p-4 sm:p-6 relative">

    <!-- Canvas Konfeti -->
    <canvas id="confetti-canvas" class="fixed inset-0 w-full h-full pointer-events-none z-40"></canvas>

    <!-- Kontainer Stiker Beruang & Hati Melayang -->
    <div id="sticker-layer" class="fixed inset-0 pointer-events-none overflow-hidden z-30"></div>

    <!-- Tombol Kontrol Pojok Kanan Atas (Musik & Edit Ucapan/Foto) -->
    <div class="fixed top-3 right-3 sm:top-4 sm:right-4 z-50 flex items-center gap-2">
        <button id="btn-music" onclick="toggleMusic()" title="Putar / Hentikan Musik"
            class="bear-card px-3.5 py-2.5 rounded-full text-xs font-bold text-[#6F4E37] hover:bg-amber-50 active:scale-95 transition flex items-center gap-1.5 shadow-sm">
            <span id="music-emoji">🔇</span>
            <span id="music-text" class="hidden sm:inline">Musik</span>
        </button>
        <button onclick="openCustomModal()" title="Edit Ucapan & Foto"
            class="bg-[#8D5B4C] text-white px-4 py-2.5 rounded-full text-xs font-bold hover:bg-[#73483B] active:scale-95 transition flex items-center gap-1.5 shadow-md">
            <span>✏️</span>
            <span>Edit Ucapan & Foto</span>
        </button>
    </div>

    <!-- ===================================================================== -->
    <!-- LAYAR 1: LAYAR AWAL (PENCET KUE ULANG TAHUN BERUANG LUCU)             -->
    <!-- ===================================================================== -->
    <main id="screen-cake" class="w-full max-w-md mx-auto text-center z-20 my-auto py-8">
        <div class="bear-card rounded-[2.2rem] p-6 sm:p-8 relative overflow-hidden">

            <!-- Hiasan Dua Beruang Mengintip di Kiri & Kanan Atas -->
            <div class="flex justify-between items-center mb-2 px-2">
                <!-- Beruang Cokelat dengan Topi Pesta -->
                <div class="animate-float select-none" title="Halo!">
                    <svg class="w-16 h-16 sm:w-20 sm:h-20" viewBox="0 0 120 120" fill="none">
                        <polygon points="60,8 42,38 78,38" fill="#F472B6"/>
                        <circle cx="60" cy="8" r="5" fill="#FDE047"/>
                        <circle cx="32" cy="48" r="14" fill="#9C6644"/>
                        <circle cx="32" cy="48" r="7" fill="#DDB892"/>
                        <circle cx="88" cy="48" r="14" fill="#9C6644"/>
                        <circle cx="88" cy="48" r="7" fill="#DDB892"/>
                        <ellipse cx="60" cy="70" rx="36" ry="32" fill="#B08968"/>
                        <ellipse cx="60" cy="78" rx="14" ry="11" fill="#EDE0D4"/>
                        <ellipse cx="60" cy="74" rx="5" ry="3.5" fill="#5C3A2E"/>
                        <path d="M55 81Q60 85 65 81" stroke="#5C3A2E" stroke-width="2.5" stroke-linecap="round"/>
                        <circle cx="46" cy="65" r="3.5" fill="#3D251E"/>
                        <circle cx="74" cy="65" r="3.5" fill="#3D251E"/>
                        <ellipse cx="38" cy="73" rx="5" ry="3" fill="#F472B6" fill-opacity="0.55"/>
                        <ellipse cx="82" cy="73" rx="5" ry="3" fill="#F472B6" fill-opacity="0.55"/>
                    </svg>
                </div>

                <span class="px-3.5 py-1.5 rounded-full bg-amber-100 border border-amber-300 text-amber-800 text-xs font-bold tracking-wide">
                    🧸 BEAR DAY SPECIAL
                </span>

                <!-- Beruang Putih / Krem Lucu -->
                <div class="animate-float-delay select-none" title="Yeay!">
                    <svg class="w-16 h-16 sm:w-20 sm:h-20" viewBox="0 0 120 120" fill="none">
                        <polygon points="60,8 42,38 78,38" fill="#60A5FA"/>
                        <circle cx="60" cy="8" r="5" fill="#F472B6"/>
                        <circle cx="32" cy="48" r="14" fill="#E6CCB2"/>
                        <circle cx="32" cy="48" r="7" fill="#FBCFE8"/>
                        <circle cx="88" cy="48" r="14" fill="#E6CCB2"/>
                        <circle cx="88" cy="48" r="7" fill="#FBCFE8"/>
                        <ellipse cx="60" cy="70" rx="36" ry="32" fill="#FFF8F0" stroke="#E6CCB2" stroke-width="2"/>
                        <ellipse cx="60" cy="78" rx="14" ry="11" fill="#F3E5D8"/>
                        <ellipse cx="60" cy="74" rx="5" ry="3.5" fill="#6F4E37"/>
                        <path d="M55 81Q60 85 65 81" stroke="#6F4E37" stroke-width="2.5" stroke-linecap="round"/>
                        <circle cx="46" cy="65" r="3.5" fill="#3D251E"/>
                        <circle cx="74" cy="65" r="3.5" fill="#3D251E"/>
                        <ellipse cx="38" cy="73" rx="5" ry="3" fill="#F472B6" fill-opacity="0.55"/>
                        <ellipse cx="82" cy="73" rx="5" ry="3" fill="#F472B6" fill-opacity="0.55"/>
                    </svg>
                </div>
            </div>

            <h1 class="font-cute text-2xl sm:text-3xl font-bold text-[#5C3A2E] leading-snug">
                Ada Kejutan Manis Buat <br>
                <span id="intro-name" class="text-[#D97706]">Cherry</span>! 🍯
            </h1>
            <p class="text-xs sm:text-sm text-[#8D5B4C] font-semibold mt-1.5 mb-5">
                Buat permohonan dulu, terus pencet kue ulang tahunnya ya!
            </p>

            <!-- KUE ULANG TAHUN INTERAKTIF DENGAN TOPPER BERUANG -->
            <div class="flex justify-center my-2">
                <button onclick="openBirthdaySurprise()" aria-label="Pencet Kue Ulang Tahun"
                    class="group relative focus:outline-none animate-cake cursor-pointer p-3 rounded-3xl transition transform hover:scale-105 active:scale-95">

                    <!-- Cahaya Hangat di Belakang Kue -->
                    <div class="absolute inset-4 bg-amber-200/50 rounded-full blur-2xl group-hover:bg-pink-200/60 transition"></div>

                    <svg class="w-56 h-56 sm:w-64 sm:h-64 relative drop-shadow-xl" viewBox="0 0 260 260" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <!-- Piring Kue -->
                        <ellipse cx="130" cy="232" rx="102" ry="15" fill="#E6CCB2"/>
                        <ellipse cx="130" cy="228" rx="92" ry="11" fill="#FFFDF9"/>

                        <!-- Layer Kue Bawah (Cokelat Susu Lembut) -->
                        <rect x="50" y="164" width="160" height="62" rx="18" fill="#B08968"/>
                        <!-- Krim Leleh Putih Susu -->
                        <path d="M50 175C50 168 57 164 65 164H195C203 164 210 168 210 175V183C210 190 200 194 194 187C188 180 178 196 170 187C162 178 152 197 142 186C132 175 122 196 112 186C102 176 92 196 82 186C72 176 62 194 55 186C51 182 50 185 50 180V175Z" fill="#FFFDF9"/>

                        <!-- Layer Kue Atas (Stroberi Pink Pastel) -->
                        <rect x="70" y="114" width="120" height="52" rx="15" fill="#F9A8D4"/>
                        <!-- Krim Leleh Atas -->
                        <path d="M70 123C70 118 76 114 83 114H177C184 114 190 118 190 123V130C190 136 181 140 176 133C171 126 162 141 154 133C146 125 137 141 129 133C121 125 112 141 104 133C96 125 87 139 80 133C74 128 70 132 70 127V123Z" fill="#FFF1F2"/>

                        <!-- Hiasan Stroberi Kecil -->
                        <circle cx="84" cy="112" r="7" fill="#FB7185"/>
                        <path d="M81 106L84 109L87 106" stroke="#22C55E" stroke-width="2" stroke-linecap="round"/>
                        <circle cx="176" cy="112" r="7" fill="#FB7185"/>
                        <path d="M173 106L176 109L179 106" stroke="#22C55E" stroke-width="2" stroke-linecap="round"/>

                        <!-- Topper Beruang Mungil di Atas Kue -->
                        <g transform="translate(95, 58)">
                            <circle cx="16" cy="22" r="9" fill="#8D5B4C"/>
                            <circle cx="54" cy="22" r="9" fill="#8D5B4C"/>
                            <ellipse cx="35" cy="36" rx="23" ry="20" fill="#9C6644"/>
                            <ellipse cx="35" cy="41" rx="9" ry="7" fill="#EDE0D4"/>
                            <ellipse cx="35" cy="39" rx="3.5" ry="2.2" fill="#5C3A2E"/>
                            <circle cx="26" cy="33" r="2.5" fill="#2B1914"/>
                            <circle cx="44" cy="33" r="2.5" fill="#2B1914"/>
                            <circle cx="21" cy="39" r="3" fill="#F472B6" fill-opacity="0.6"/>
                            <circle cx="49" cy="39" r="3" fill="#F472B6" fill-opacity="0.6"/>
                        </g>

                        <!-- Lilin Ulang Tahun di Tengah -->
                        <rect x="124" y="42" width="12" height="30" rx="4" fill="#FEF08A" stroke="#F59E0B" stroke-width="1.5"/>
                        <path d="M124 49L136 54M124 58L136 63" stroke="#F472B6" stroke-width="2.5" stroke-linecap="round"/>
                        <line x1="130" y1="35" x2="130" y2="42" stroke="#5C3A2E" stroke-width="2"/>

                        <!-- Api Lilin Menyala -->
                        <g id="candle-flame" class="flame-glow">
                            <ellipse cx="130" cy="24" rx="12" ry="15" fill="#FDE047" fill-opacity="0.4"/>
                            <path d="M130 10C130 10 139 20 139 27C139 31.9706 134.971 36 130 36C125.029 36 121 31.9706 121 27C121 20 130 10 130 10Z" fill="#F97316"/>
                            <path d="M130 16C130 16 135 22 135 27C135 29.7614 132.761 32 130 32C127.239 32 125 29.7614 125 27C125 22 130 16 130 16Z" fill="#FEF08A"/>
                        </g>

                        <!-- Asap Tipis Saat Lilin Padam -->
                        <g id="candle-smoke" class="smoke-puff">
                            <circle cx="130" cy="24" r="5" fill="#D6D3D1"/>
                            <circle cx="135" cy="17" r="4" fill="#E7E5E4"/>
                        </g>

                        <!-- Meses Warna-Warni -->
                        <circle cx="80" cy="205" r="3.5" fill="#FDE047"/>
                        <circle cx="112" cy="208" r="3.5" fill="#F472B6"/>
                        <circle cx="148" cy="204" r="3.5" fill="#38BDF8"/>
                        <circle cx="180" cy="207" r="3.5" fill="#FDE047"/>
                        <circle cx="105" cy="152" r="3" fill="#FDE047"/>
                        <circle cx="155" cy="151" r="3" fill="#60A5FA"/>
                    </svg>
                </button>
            </div>

            <!-- Tombol Utama Pencet Kue -->
            <button onclick="openBirthdaySurprise()"
                class="mt-2 w-full py-4 px-6 rounded-2xl bg-gradient-to-r from-[#F59E0B] via-[#EC4899] to-[#8D5B4C] text-white font-cute text-lg font-bold shadow-lg shadow-pink-500/25 hover:brightness-105 active:scale-95 transition flex items-center justify-center gap-2">
                <span>Pencet Kue Ulang Tahunnya!</span>
                <span class="text-xl">🎂🧸</span>
            </button>
        </div>
    </main>

    <!-- ===================================================================== -->
    <!-- LAYAR 2: HALAMAN UCAPAN & GALERI 3 FOTO BERUANG LUCU                  -->
    <!-- ===================================================================== -->
    <section id="screen-celebration" class="hidden w-full max-w-3xl mx-auto z-20 py-12 px-1 sm:px-3">

        <!-- Header Ucapan dengan Dua Beruang Bersorak -->
        <div class="bear-card rounded-[2.2rem] p-6 sm:p-8 text-center mb-7 relative overflow-hidden">
            <div class="flex items-center justify-center gap-3 sm:gap-5 mb-2">
                <span class="text-3xl sm:text-4xl animate-float">🧸</span>
                <span class="px-4 py-1.5 rounded-full bg-pink-100 border border-pink-200 text-pink-600 text-xs font-extrabold tracking-wider">
                    ✨ HAPPY BIRTHDAY ✨
                </span>
                <span class="text-3xl sm:text-4xl animate-float-delay">🐻‍❄️</span>
            </div>

            <h1 class="font-cute text-3xl sm:text-4xl md:text-5xl font-bold text-[#5C3A2E] leading-tight">
                Selamat Ulang Tahun, <br>
                <span id="display-recipient" class="text-transparent bg-clip-text bg-gradient-to-r from-[#D97706] via-[#DB2777] to-[#8D5B4C]">
                    Cherry!
                </span> 🥳🎂
            </h1>
            <p class="text-xs sm:text-sm text-[#8D5B4C] font-semibold mt-2">
                Semoga hari-harimu selalu hangat, manis, dan penuh pelukan seperti beruang lucu! 🍯💛
            </p>
        </div>

        <!-- GALERI 3 FOTO SPESIAL DALAM BINGKAI TELINGA BERUANG -->
        <div class="mb-7">
            <div class="flex items-center justify-between mb-4 px-2">
                <h2 class="font-cute text-xl sm:text-2xl font-bold text-[#5C3A2E] flex items-center gap-2">
                    <span>📸</span> Kenangan Manis
                </h2>
                <span class="text-xs font-bold text-[#8D5B4C] bg-amber-100/80 px-3 py-1 rounded-full">
                    🐾 3 Foto Spesial
                </span>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-3 gap-6 pt-3">
                <!-- FOTO 1: 115743.webp -->
                <div class="bear-polaroid flex flex-col">
                    <div class="aspect-square w-full rounded-2xl overflow-hidden bg-amber-50 border border-amber-100 relative">
                        <img id="photo-1" src="115743.webp" alt="Foto Kenangan 1"
                            onerror="handleImageFallback(this, '115743.webp')"
                            class="w-full h-full object-cover">
                        <span class="absolute bottom-2 right-2 bg-white/85 backdrop-blur-sm text-xs px-2 py-0.5 rounded-full shadow-sm">🐾</span>
                    </div>
                    <p id="caption-1" class="font-cute text-center text-sm font-semibold text-[#5C3A2E] mt-2.5 px-1">
                        Cantik & Gemes Banget 🧸✨
                    </p>
                </div>

                <!-- FOTO 2: 115293.jpg -->
                <div class="bear-polaroid flex flex-col">
                    <div c
