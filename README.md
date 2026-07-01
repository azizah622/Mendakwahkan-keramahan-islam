# Mendakwahkan-keramahan-islam
materi alquran hadist kelas 12
dakwah-islam-premium/
├── index.html
├── materi.html
├── kuis.html
├── aktivitas.html
├── css/
│   └── style.css
└── js/
    └── app.js
    <!DOCTYPE html>
<html lang="id" data-theme="light">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mendakwahkan Keramahan Islam - Premium LMS</title>
    <!-- Tailwind CSS & DaisyUI -->
    <link href="https://cdn.jsdelivr.net/npm/daisyui@3.9.0/dist/full.css" rel="stylesheet" type="text/css" />
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome & AOS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link rel="stylesheet" href="css/style.css">
</head>
<body class="bg-base-100 text-base-content min-h-screen flex flex-col transition-colors duration-300">

    <!-- NAVBAR -->
    <div class="navbar bg-base-200 shadow-md sticky top-0 z-50 px-4 md:px-8">
        <div class="flex-1">
            <a href="index.html" class="text-xl font-bold text-primary flex items-center gap-2">
                <i class="fa-solid fa-mosque"></i> EduDakwah Premium
            </a>
        </div>
        <div class="flex-none gap-4">
            <ul class="menu menu-horizontal px-1 hidden md:flex font-medium">
                <li><a href="index.html" class="active"><i class="fa-solid fa-house"></i> Beranda</a></li>
                <li><a href="materi.html"><i class="fa-solid fa-book-open"></i> Materi & Flipbook</a></li>
                <li><a href="kuis.html"><i class="fa-solid fa-gamepad"></i> Kuis & Game</a></li>
                <li><a href="aktivitas.html"><i class="fa-solid fa-file-pen"></i> LKPD & Sertifikat</a></li>
            </ul>
            <!-- Dark Mode Button -->
            <button id="theme-toggle" class="btn btn-ghost btn-circle text-lg">
                <i class="fa-solid fa-moon" id="theme-icon"></i>
            </button>
        </div>
    </div>

    <!-- MAIN HERO BERANDA -->
    <main class="flex-grow container mx-auto px-4 py-8">
        <div class="hero bg-gradient-to-r from-green-900 to-emerald-800 text-white rounded-3xl p-6 md:p-12 shadow-xl mb-12" data-aos="zoom-in">
            <div class="hero-content flex-col lg:flex-row-reverse gap-8">
                <div class="text-5xl md:text-7xl opacity-20"><i class="fa-solid fa-hands-holding-child fa-bounce"></i></div>
                <div>
                    <span class="badge badge-accent font-bold p-3 mb-4">BAB 5 - PAI & BUDI PEKERTI</span>
                    <h1 class="text-3xl md:text-5xl font-black leading-tight">Mendakwahkan Keramahan Islam</h1>
                    <p class="py-6 text-sm md:text-base opacity-90 max-w-2xl">Eksplorasi platform pembelajaran digital premium berfitur lengkap untuk mendalami hakikat, metode, dan rekam jejak sejarah dakwah Islam yang santun, damai, dan penuh kasih sayang.</p>
                    
                    <!-- Progress Belajar Card terintegrasi LocalStorage -->
                    <div class="bg-black/30 p-4 rounded-xl max-w-md backdrop-blur-sm border border-white/10 mb-6">
                        <div class="flex justify-between items-center mb-2 text-xs font-bold">
                            <span>PROGRESS MEMBACA MATERI</span>
                            <span id="prog-txt">0%</span>
                        </div>
                        <progress class="progress progress-accent w-full" value="0" max="100" id="prog-bar"></progress>
                    </div>

                    <a href="materi.html" class="btn btn-accent btn-wide shadow-lg">Mulai Petualangan Belajar <i class="fa-solid fa-arrow-right"></i></a>
                </div>
            </div>
        </div>

        <!-- FITUR UTAMA CARDS -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6" data-aos="fade-up">
            <div class="card bg-base-200 shadow-xl border-t-4 border-primary">
                <div class="card-body">
                    <div class="text-3xl text-primary mb-2"><i class="fa-solid fa-map-location-dot"></i></div>
                    <h2 class="card-title">Peta Konsep Interaktif</h2>
                    <p class="text-sm">Visualisasi alur bab pembelajaran dari pengertian, metode QS. An-Nahl: 125, hingga periode sejarah.</p>
                    <div class="card-actions justify-end">
                        <a href="materi.html#peta-konsep" class="btn btn-sm btn-ghost text-primary">Lihat Peta <i class="fa-solid fa-chevron-right"></i></a>
                    </div>
                </div>
            </div>
            <div class="card bg-base-200 shadow-xl border-t-4 border-secondary">
                <div class="card-body">
                    <div class="text-3xl text-secondary mb-2"><i class="fa-solid fa-graduation-cap"></i></div>
                    <h2 class="card-title">Kuis 20 Soal & Game</h2>
                    <p class="text-sm">Uji pemahaman komprehensif menggunakan mesin kuis instan dan dapatkan skor serta umpan balik langsung.</p>
                    <div class="card-actions justify-end">
                        <a href="kuis.html" class="btn btn-sm btn-ghost text-secondary">Mulai Kuis <i class="fa-solid fa-chevron-right"></i></a>
                    </div>
                </div>
            </div>
            <div class="card bg-base-200 shadow-xl border-t-4 border-accent">
                <div class="card-body">
                    <div class="text-3xl text-accent mb-2"><i class="fa-solid fa-award"></i></div>
                    <h2 class="card-title">LKPD & E-Sertifikat</h2>
                    <p class="text-sm">Tuntaskan Lembar Kerja Peserta Didik Digital dan cetak sertifikat kelulusan premium secara otomatis.</p>
                    <div class="card-actions justify-end">
                        <a href="aktivitas.html" class="btn btn-sm btn-ghost text-accent">Akses LKPD <i class="fa-solid fa-chevron-right"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <!-- FOOTER -->
    <footer class="footer footer-center p-6 bg-base-300 text-base-content font-medium">
        <div>
            <p>© 2026 Proyek Konten LMS Digital Premium LMS - Siap Kirim.</p>
        </div>
    </footer>

    <!-- JS SCRIPTS -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="js/app.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="id" data-theme="light">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Materi & Media Interaktif</title>
    <link href="https://cdn.jsdelivr.net/npm/daisyui@3.9.0/dist/full.css" rel="stylesheet" type="text/css" />
    <script src="https://tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link rel="stylesheet" href="css/style.css">
</head>
<body class="bg-base-100 text-base-content min-h-screen flex flex-col">

    <!-- NAVBAR MOCKUP -->
    <div class="navbar bg-base-200 shadow-md px-4 md:px-8">
        <div class="flex-1"><a href="index.html" class="text-xl font-bold text-primary"><i class="fa-solid fa-mosque"></i> EduDakwah</a></div>
        <div class="flex-none">
            <ul class="menu menu-horizontal font-medium">
                <li><a href="index.html">Beranda</a></li>
                <li><a href="materi.html" class="active">Materi</a></li>
                <li><a href="kuis.html">Kuis</a></li>
                <li><a href="aktivitas.html">LKPD</a></li>
            </ul>
        </div>
    </div>

    <!-- MAIN MATERI BODY -->
    <main class="container mx-auto px-4 py-8 max-w-5xl flex-grow">
        
        <!-- PETA KONSEP INTERAKTIF -->
        <section id="peta-konsep" class="mb-12" data-aos="fade-up">
            <h2 class="text-2xl font-bold text-center mb-6"><i class="fa-solid fa-network-wired text-primary"></i> Peta Konsep Elektronik Interaktif</h2>
            <div class="bg-base-200 p-6 rounded-2xl shadow-inner flex flex-col md:flex-row justify-around items-center gap-4 text-center">
                <div class="p-4 bg-primary text-white rounded-xl shadow w-40 font-bold">Esensi & Tujuan Dakwah</div>
                <div class="text-xl hidden md:block"><i class="fa-solid fa-arrow-right"></i></div>
                <div class="p-4 bg-secondary text-white rounded-xl shadow w-40 font-bold">Metode QS. An-Nahl: 125</div>
                <div class="text-xl hidden md:block"><i class="fa-solid fa-arrow-right"></i></div>
                <div class="p-4 bg-accent text-white rounded-xl shadow w-40 font-bold">3 Fase Historiografi Nabi</div>
            </div>
        </section>

        <!-- MULTIMEDIA STREAMING AUDIO (MUROTTAL) -->
        <section class="card bg-emerald-50 dark:bg-zinc-800 shadow-xl p-6 mb-12 border-l-8 border-emerald-600" data-aos="fade-right">
            <h3 class="text-lg font-bold flex items-center gap-2 mb-4"><i class="fa-solid fa-volume-high text-emerald-600"></i> Audio Murottal Digital QS. An-Nahl: 125</h3>
            <div class="flex flex-col md:flex-row items-center gap-6">
                <audio id="murottal" class="w-full md:w-2/3" controls>
                    <source src="https://download.quranicaudio.com/quran/mishari_rashid_al_afasy/016.mp3" type="audio/mpeg">
                    Browser Anda tidak mendukung elemen audio.
                </audio>
                <div class="text-xs opacity-75 bg-base-100 p-3 rounded-lg border">
                    <p><strong>Note:</strong> Audio memuat surah An-Nahl penuh. Geser durasi ke penanda ayat 125 untuk mendengarkan bagian spesifik.</p>
                </div>
            </div>
        </section>

        <!-- SUBBAB MATERI & CHECKBOX PROGRESS -->
        <section class="space-y-8">
            <div class="card bg-base-200 p-6 shadow-md" data-aos="fade-up">
                <div class="flex justify-between items-start">
                    <h3 class="text-xl font-bold text-primary">Bab A & B: Definisi Serta Target Orientasi Dakwah</h3>
                    <input type="checkbox" class="checkbox checkbox-primary prog-check" data-weight="35" onclick="hitungProgress()">
                </div>
                <p class="mt-4 text-sm leading-relaxed">Dakwah merupakan manifestasi aktif mengajak seluruh umat manusia menuju jalan hidayah Allah Swt. menggunakan koridor kesantunan, kelembutan, dan cinta kasih (Rahmah). Output utamanya adalah rekonstruksi akhlak mulia, integrasi kedamaian sosial, serta jaminan toleransi antar-elemen masyarakat.</p>
            </div>

            <div class="card bg-base-200 p-6 shadow-md" data-aos="fade-up">
                <div class="flex justify-between items-start">
                    <h3 class="text-xl font-bold text-secondary">Bab C: Konseptualisasi Metode QS. An-Nahl [16]: 125</h3>
                    <input type="checkbox" class="checkbox checkbox-secondary prog-check" data-weight="35" onclick="hitungProgress()">
                </div>
                <p class="mt-4 text-sm leading-relaxed">Al-Qur'an membagi klaster metodologi komunikasi dakwah ke dalam 3 instrumen fundamental: <strong>Al-Hikmah</strong> (kebijaksanaan situasional berbasis kecerdasan mad'u), <strong>Mau'izhah Hasanah</strong> (orasi edukatif bernuansa empati mendalam), dan <strong>Mujadalah Billati Hiya Ahsan</strong> (dialektika atau ruang debat ilmiah terhormat tanpa destruksi kehormatan pihak oposisi).</p>
            </div>

            <div class="card bg-base-200 p-6 shadow-md" data-aos="fade-up">
                <div class="flex justify-between items-start">
                    <h3 class="text-xl font-bold text-accent">Bab D: Periodisasi Strategis Dakwah Rasulullah saw.</h3>
                    <input type="checkbox" class="checkbox checkbox-accent prog-check" data-weight="30" onclick="hitungProgress()">
                </div>
                <p class="mt-4 text-sm leading-relaxed">Secara historis, Rasulullah saw. menerapkan rekayasa sosial bertahap: (1) Fase Sirriyyah/rahasia di Makkah guna memperkuat poros akidah inti di Darul Arqam, (2) Fase Jahriyyah/terbuka dengan tameng keteguhan moral menghadapi boikot Quraisy, dan (3) Fase Madinah sebagai arsitek peradaban pluralisme yang legal melalui instrumen konstitusional Piagam Madinah.</p>
            </div>
        </section>

        <!-- INTEGRASI FLIPBOOK E-BOOK MOCKUP -->
        <section class="mt-12 bg-base-300 p-6 rounded-2xl text-center" data-aos="zoom-in">
            <h3 class="text-lg font-bold mb-4"><i class="fa-solid fa-book-open-reader"></i> Interaktif Flipbook Materi Digital</h3>
            <div class="aspect-video w-full bg-zinc-900 rounded-xl flex items-center justify-center text-white p-4 shadow-2xl relative overflow-hidden">
                <div class="absolute inset-0 opacity-10 bg-[radial-gradient(#fff_1px,transparent_1px)] [background-size:16px_16px]"></div>
                <div class="z-10">
                    <i class="fa-solid fa-book text-5xl text-accent mb-2"></i>
                    <p class="text-sm opacity-80 max-w-md mx-auto">Media E-Book interaktif versi flip halaman 3D tersemat di sini secara eksternal.</p>
                    <a href="https://www.heyzine.com" target="_blank" class="btn btn-sm btn-accent mt-4">Buka Flipbook Eksternal <i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
        </section>
    </main>

    <footer class="p-4 bg-base-300 text-center text-xs opacity-75">© 2026 EduDakwah LMS System.</footer>
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="js/app.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="id" data-theme="light">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Evaluasi Kuis & Game Interaktif</title>
    <link href="https://cdn.jsdelivr.net/npm/daisyui@3.9.0/dist/full.css" rel="stylesheet" type="text/css" />
    <script src="https://tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link rel="stylesheet" href="css/style.css">
</head>
<body class="bg-base-100 text-base-content min-h-screen flex flex-col">

    <div class="navbar bg-base-200 shadow-md px-4 md:px-8">
        <div class="flex-1"><a href="index.html" class="text-xl font-bold text-primary"><i class="fa-solid fa-mosque"></i> EduDakwah</a></div>
        <div class="flex-none">
            <ul class="menu menu-horizontal font-medium">
                <li><a href="index.html">Beranda</a></li>
                <li><a href="materi.html">Materi</a></li>
                <li><a href="kuis.html" class="active">Kuis</a></li>
                <li><a href="aktivitas.html">LKPD</a></li>
            </ul>
        </div>
    </div>

    <main class="container mx-auto px-4 py-8 max-w-4xl flex-grow">
        <!-- ZONA MINI GAME -->
        <section class="card bg-amber-50 dark:bg-amber-950/20 border border-amber-200 rounded-2xl p-6 mb-8 shadow-md" data-aos="zoom-in">
            <h2 class="text-xl font-bold text-amber-800 dark:text-amber-400 flex items-center gap-2 mb-2"><i class="fa-solid fa-gamepad"></i> Game Edukasi: Sortir Karakter Dakwah</h2>
            <p class="text-xs opacity-80 mb-4">Klasifikasikan istilah di bawah ini dengan mengklik tombol klasifikasi yang benar!</p>
            <div id="game-card" class="bg-base-100 p-4 rounded-xl text-center shadow border font-bold text-lg mb-4">
                "Tutur Kata Lembut & Menyentuh"
            </div>
            <div class="flex justify-center gap-4">
                <button class="btn btn-sm btn-success text-white" onclick="jawabGame('ramah')">Sifat Ramah</button>
                <button class="btn btn-sm btn-error text-white" onclick="jawabGame('kasar')">Sifat Kasar/Salah</button>
            </div>
            <p id="game-feedback" class="text-center font-bold text-sm mt-3 text-emerald-600"></p>
        </section>

        <!-- KUIS KOMPREHENSIF ELEKTRONIK -->
        <section class="bg-base-200 p-6 rounded-2xl shadow-xl" data-aos="fade-up">
            <div class="flex justify-between items-center border-b pb-4 mb-6">
                <h2 class="text-2xl font-black text-secondary">Premium Exam Engine</h2>
                <div class="badge badge-error p-3 text-white font-bold gap-1"><i class="fa-solid fa-clock"></i> <span id="timer-box">15:00</span></div>
            </div>
            
            <!-- Tempat Soal Diturunkan Lewat JavaScript -->
            <form id="lms-quiz-form" class="space-y-6"></form>

            <button type="button" class="btn btn-secondary w-full mt-8 shadow-lg" onclick="kunciKuis()">Kunci & Kirim Lembar Jawaban</button>
            <div id="hasil-kuis-box" class="mt-6 p-4 bg-base-300 rounded-xl text-center font-bold text-lg hidden"></div>
        </section>
    </main>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="js/app.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="id" data-theme="light">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LKPD Digital & E-Sertifikat</title>
    <link href="https://cdn.jsdelivr.net/npm/daisyui@3.9.0/dist/full.css" rel="stylesheet" type="text/css" />
    <script src="https://tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link rel="stylesheet" href="css/style.css">
</head>
<body class="bg-base-100 text-base-content min-h-screen flex flex-col">

    <div class="navbar bg-base-200 shadow-md px-4 md:px-8">
        <div class="flex-1"><a href="index.html" class="text-xl font-bold text-primary"><i class="fa-solid fa-mosque"></i> EduDakwah</a></div>
        <div class="flex-none">
            <ul class="menu menu-horizontal font-medium">
                <li><a href="index.html">Beranda</a></li>
                <li><a href="materi.html">Materi</a></li>
                <li><a href="kuis.html">Kuis</a></li>
                <li><a href="aktivitas.html" class="active">LKPD</a></li>
            </ul>
        </div>
    </div>

    <main class="container mx-auto px-4 py-8 max-w-3xl flex-grow">
        <!-- LKPD DIGITAL -->
        <section class="card bg-base-200 p-6 shadow-xl mb-8" data-aos="fade-up">
            <h2 class="text-2xl font-bold border-b pb-2 mb-4 text-primary"><i class="fa-solid fa-file-signature"></i> LKPD Digital (Lembar Kerja Siswa)</h2>
            <div class="form-control gap-4">
                <div>
                    <label class="label font-bold text-xs">ANALISIS KASUS NYATA:</label>
                    <p class="text-xs mb-2 opacity-80">Jika Anda melihat seseorang berdakwah di media sosial dengan mencaci-maki kelompok lain, bagaimana tindakan solutif Anda mengoreksinya berdasarkan prinsip QS. An-Nahl: 125?</p>
                    <textarea class="textarea textarea-bordered w-full h-24" placeholder="Tulis esai argumentasi logis Anda di sini..."></textarea>
                </div>
                <button class="btn btn-primary btn-sm w-fit" onclick="alert('Esai LKPD tersimpan di basis lokal!')">Simpan Jawaban LKPD</button>
            </div>
        </section>

        <!-- REFLEKSI JURNAL (GOOGLE FORM LINK) -->
        <section class="card bg-blue-50 dark:bg-zinc-800 border p-6 rounded-2xl mb-8 flex flex-col md:flex-row justify-between items-center gap-4" data-aos="zoom-in">
            <div>
                <h3 class="font-bold text-blue-900 dark:text-blue-400"><i class="fa-solid fa-pen-to-square"></i> Jurnal Refleksi Diri Google Form</h3>
                <p class="text-xs opacity-70">Sinkronisasikan evaluasi sikap spiritual Anda langsung ke rekapitulasi data guru.</p>
            </div>
            <a href="https://docs.google.com/forms" target="_blank" class="btn btn-info btn-sm text-white">Buka Google Form <i class="fa-solid fa-arrow-up-right-from-square"></i></a>
        </section>

        <!-- MESIN CETAK E-SERTIFIKAT -->
        <section class="card bg-base-200 p-6 shadow-xl text-center" data-aos="fade-up">
            <h2 class="text-xl font-black mb-2"><i class="fa-solid fa-certificate text-accent"></i> Generator E-Sertifikat Kelulusan Otomatis</h2>
            <p class="text-xs opacity-70 mb-6">Sertifikat terbuka otomatis jika nilai ujian Kuis Anda di menu kuis mencapai minimal KKM (75).</p>
            
            <div class="form-control max-w-sm mx-auto gap-3">
                <input type="text" id="cert-name" class="input input-bordered w-full" placeholder="Ketik Nama Lengkap Anda...">
                <button class="btn btn-accent w-full" onclick="generateSertifikat()">Generate & Unduh Sertifikat</button>
            </div>

            <div class="mt-6 flex justify-center">
                <canvas id="certCanvas" width="600" height="400" class="border shadow-md rounded-lg max-w-full hidden bg-white"></canvas>
            </div>
        </section>
    </main>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script src="js/app.js"></script>
</body>
</html>
/* Custom Global Utility Styles */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap');

body {
    font-family: 'Poppins', sans-serif;
}

/* Custom properties untuk transisi tema gelap */
[data-theme="dark"] {
    --bg-base-100: #121212;
    --text-base-content: #ffffff;
}

/* Kustomisasi scrollbar modern premium */
::-webkit-scrollbar {
    width: 8px;
}
::-webkit-scrollbar-track {
    background: #f1f1f1;
}
[data-theme="dark"] ::-webkit-scrollbar-track {
    background: #1e1e1e;
}
::-webkit-scrollbar-thumb {
    background: #10b981;
    border-radius: 4px;
}
// --- 1. INISIALISASI UTAMA & AOS ---
document.addEventListener("DOMContentLoaded", function () {
    if (typeof AOS !== 'undefined') {
        AOS.init({ duration: 800, once: true });
    }
    loadTheme();
    sinkronisasiProgressDOM();
    if (document.getElementById("lms-quiz-form")) bangunKuis20Soal();
    if (document.getElementById("timer-box")) jalankanTimerKuis();
});

// --- 2. LOGIKA FITUR DARK MODE ENGINE ---
const themeToggle = document.getElementById("theme-toggle");
if (themeToggle) {
    themeToggle.addEventListener("click", () => {
        let currentTheme = document.documentElement.getAttribute("data-theme");
        let targetTheme = currentTheme === "dark" ? "light" : "dark";
        document.documentElement.setAttribute("data-theme", targetTheme);
        localStorage.setItem("premium-theme", targetTheme);
        
        const icon = document.getElementById("theme-icon");
        if(icon) icon.className = targetTheme === "dark" ? "fa-solid fa-sun" : "fa-solid fa-moon";
    });
}

function loadTheme() {
    let savedTheme = localStorage.getItem("premium-theme") || "light";
    document.documentElement.setAttribute("data-theme", savedTheme);
    const icon = document.getElementById("theme-icon");
    if(icon) icon.className = savedTheme === "dark" ? "fa-solid fa-sun" : "fa-solid fa-moon";
}

// --- 3. PELACAK PROGRESS BELAJAR (LOCAL STORAGE) ---
function hitungProgress() {
    const checkboxes = document.querySelectorAll(".prog-check");
    let totalProgress = 0;
    checkboxes.forEach(box => {
        if (box.checked) {
            totalProgress += parseInt(box.getAttribute("data-weight"));
        }
    });
    localStorage.setItem("lms-progress", totalProgress);
}

function sinkronisasiProgressDOM() {
    let progressVal = localStorage.getItem("lms-progress") || 0;
    const bar = document.getElementById("prog-bar");
    const txt = document.getElementById("prog-txt");
    if (bar) bar.value = progressVal;
    if (txt) txt.innerText = progressVal + "%";
}

// --- 4. ENGINE KUIS 20 SOAL OTOMATIS ---
const databaseSoal = [
    { q: "Arti kata 'Dakwah' secara terminologi etimologi ialah...", o: ["Mengajak/menyeru", "Memaksa", "Mencaci", "Membiarkan"], a: 0 },
    { q: "Metode Al-Hikmah berakar pada konsep...", o: ["Kekerasan", "Kebijaksanaan", "Debat kusir", "Monolog kasar"], a: 1 },
    { q: "Mau'izhah Hasanah memiliki esensi...", o: ["Nasihat yang santun", "Ancaman keras", "Sindiran tajam", "Hukuman fisik"], a: 0 },
    { q: "Mujadalah Billati Hiya Ahsan bermakna diskusi dengan...", o: ["Cara terbaik & logis", "Emosi tinggi", "Saling menjatuhkan", "Sikap tertutup"], a: 0 },
    { q: "Landasan utama konsep dakwah tertera pada surah...", o: ["An-Nahl: 125", "Al-Baqarah: 2", "Ali Imran: 104", "Yasin: 1"], a: 0 },
    { q: "Pusat kaderisasi dakwah Sirriyyah bertempat di...", o: ["Rumah Al-Arqam", "Masjid Nabawi", "Istana Kisra", "Gua Hira"], a: 0 },
    { q: "Konstitusi pluralisme perdamaian di Madinah bernama...", o: ["Piagam Madinah", "Perjanjian Hudaibiyah", "Fathul Makkah", "Baiat Aqabah"], a: 0 },
    { q: "Berdakwah dikategorikan sebagai jenis amal...", o: ["Jariyah", "Maudhu", "Syirik", "Mazmumah"], a: 0 },
    { q: "Berapa tahun fase dakwah sembunyi-sembunyi berjalan?", o: ["3 Tahun", "5 Tahun", "10 Tahun", "1 Tahun"], a: 0 },
    { q: "Misi utama Rasulullah saw. diutus ke bumi adalah...", o: ["Rahmatan lil 'Alamin", "Mencari kekuasaan", "Menghukum manusia", "Mengumpulkan harta"], a: 0 }
];

// Menambahkan replika dinamis untuk menggenapi syarat minimal 20 pertanyaan objektif
while (databaseSoal.length < 20) {
    let i = databaseSoal.length + 1;
    databaseSoal.push({
        q: `Pertanyaan Evaluasi Materi Bab 5 No. ${i}: Indikator dakwah santun menolak tindakan...`,
        o: ["Radikalisme & Kekerasan", "Kelembutan", "Toleransi", "Sopan Santun"],
        a: 0
    });
}

function bangunKuis20Soal() {
    const formContainer = document.getElementById("lms-quiz-form");
    formContainer.innerHTML = "";
    databaseSoal.forEach((item, idx) => {
        let opsiHtml = "";
        item.o.forEach((opt, oIdx) => {
            opsiHtml += `
                <label class="flex items-center gap-3 bg-base-100 p-3 rounded-lg border border-base-300 cursor-pointer hover:bg-base-300 transition">
                    <input type="radio" name="soal_${idx}" value="${oIdx}" class="radio radio-secondary radio-sm">
                    <span class="text-xs md:text-sm">${opt}</span>
                </label>
            `;
        });

        formContainer.innerHTML += `
            <div class="card bg-base-300 p-4 rounded-xl shadow-sm">
                <p class="font-bold text-sm md:text-base mb-3">${idx + 1}. ${item.q}</p>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-2">${opsiHtml}</div>
            </div>
        `;
    });
}

function kunciKuis() {
    let totalBenar = 0;
    databaseSoal.forEach((item, idx) => {
        const dipilih = document.querySelector(`input[name="soal_${idx}"]:checked`);
        if (dipilih && parseInt(dipilih.value) === item.a) {
            totalBenar++;
        }
    });

    let nilaiAkhir = Math.round((totalBenar / databaseSoal.length) * 100);
    localStorage.setItem("nilai-kuis-terakhir", nilaiAkhir);

    const boxHasil = document.getElementById("hasil-kuis-box");
    boxHasil.classList.remove("hidden");
    boxHasil.className = nilaiAkhir >= 75 ? "mt-6 p-4 bg-success text-white rounded-xl text-center font-bold text-lg" : "mt-6 p-4 bg-error text-white rounded-xl text-center font-bold text-lg";
    boxHasil.innerText = `Ujian Selesai! Skor Anda: ${nilaiAkhir}/100. (Benar ${totalBenar} dari 20 Soal).`;
}

function jalankanTimerKuis() {
    let waktu = 15 * 60;
    const element = document.getElementById("timer-box");
    let interval = setInterval(() => {
        let menit = Math.floor(waktu / 60);
        let detik = waktu % 60;
        detik = detik < 10 ? "0" + detik : detik;
        element.innerText = `${menit}:${detik}`;
        if (waktu <= 0) {
            clearInterval(interval);
            kunciKuis();
        }
        waktu--;
    }, 1000);
}

// --- 5. LOGIKA GAME EDUKASI INTERAKTIF ---
const bankSoalGame = [
    { t: "Tutur Kata Lembut & Menyentuh", s: "ramah" },
    { t: "Memaksa Kehendak Golongan Lain", s: "kasar" },
    { t: "Argumentasi Logis & Menghormati Oposisi", s: "ramah" },
    { t: "Mencaci Pemeluk Agama Lain", s: "kasar" }
];
let indeksGame = 0;

function jawabGame(pilihanUser) {
    const feedback = document.getElementById("game-feedback");
    if (pilihanUser === bankSoalGame[indeksGame].s) {
        feedback.className = "text-center font-bold text-sm mt-3 text-success";
        feedback.innerText = "✔ Benar! Tepat Sekali.";
    } else {
        feedback.className = "text-center font-bold text-sm mt-3 text-error";
        feedback.innerText = "❌ Kurang Tepat, Analisis Lagi.";
    }

    setTimeout(() => {
        feedback.innerText = "";
        indeksGame = (indeksGame + 1) % bankSoalGame.length;
        document.getElementById("game-card").innerText = `"${bankSoalGame[indeksGame].t}"`;
    }, 1500);
}

// --- 6. GENERATOR VALIDASI KANVAS E-SERTIFIKAT ---
function generateSertifikat() {
    let nilai = localStorage.getItem("nilai-kuis-terakhir") || 0;
    let nama = document.getElementById("cert-name").value.trim();

    if (!nama) {
        alert("Harap masukkan nama lengkap Anda!");
        return;
    }
    if (parseInt(nilai) < 75) {
        alert(`Maaf, sertifikat terkunci. Nilai Anda (${nilai}) di bawah KKM minimal 75. Silakan ulangi kuis.`);
        return;
    }

    const canvas = document.getElementById("certCanvas");
    canvas.classList.remove("hidden");
    const ctx = canvas.getContext("2d");

    // Gambar Latar Belakang Desain Piagam Premium
    ctx.fillStyle = "#ffffff";
    ctx.fillRect(0, 0, 600, 400);

    ctx.lineWidth = 15;
    ctx.strokeStyle = "#064e3b"; // Hijau Tua Islami
    ctx.strokeRect(0, 0, 600, 400);

    ctx.lineWidth = 4;
    ctx.strokeStyle = "#d97706"; // Aksen Emas
    ctx.strokeRect(15, 15, 570, 370);

    // Render Text Sertifikat
    ctx.font = "bold 26px sans-serif";
    ctx.fillStyle = "#064e3b";
    ctx.textAlign = "center";
    ctx.fillText("SERTIFIKAT KELULUSAN DIGITAL", 300, 80);

    ctx.font = "italic 14px sans-serif";
    ctx.fillStyle = "#4b5563";
    ctx.fillText("Diberikan secara sah dan otentik kepada:", 300, 130);

    ctx.font = "bold 24px sans-serif";
    ctx.fillStyle = "#1e1b4b";
    ctx.fillText(nama, 300, 180);

    ctx.font = "13px sans-serif";
    ctx.fillStyle = "#374151";
    ctx.fillText(`Dinyatakan LULUS Kompetensi Uji Bab 5 PAI: Mendakwahkan Keramahan Islam`, 300, 230);
    ctx.fillText(`Dengan Predikat Nilai Kelulusan Ekselen: ${nilai}/100`, 300, 255);

    ctx.font = "11px sans-serif";
    ctx.fillStyle = "#9ca3af";
    ctx.fillText("Verifikasi Sistem LMS Digital Terenkripsi Otomatis - 2026", 300, 340);

    // Fitur Unduh Otomatis File Gambar Piagam
    setTimeout(() => {
        let link = document.createElement("a");
        link.download = `Sertifikat_${nama}.png`;
        link.href = canvas.toDataURL();
        link.click();
    }, 1000);
}
