<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio | Kurnia Adela, S.Pd. - Administrative & Data Specialist</title>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        earth: {
                            50: '#FDFBF7',
                            100: '#F7F2EA',
                            200: '#EFE5D5',
                            300: '#E1D1B7',
                            400: '#CBB28F',
                            500: '#B29168',
                            600: '#8E6F47',
                            700: '#6B5233',
                            800: '#4A3722',
                            900: '#2D2013',
                        },
                        maroon: {
                            DEFAULT: '#7A1C1C',
                            light: '#9B2C2C',
                            dark: '#521010',
                            soft: '#F9ECEC',
                            muted: '#A84343'
                        },
                        sand: '#FAF6F0',
                        terracotta: '#C86D51'
                    },
                    fontFamily: {
                        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
                        serif: ['"Playfair Display"', 'serif'],
                    },
                    boxShadow: {
                        'soft-warm': '0 10px 30px -5px rgba(122, 28, 28, 0.05), 0 4px 12px -2px rgba(142, 111, 71, 0.08)',
                        'hover-warm': '0 20px 40px -10px rgba(122, 28, 28, 0.12), 0 8px 16px -4px rgba(142, 111, 71, 0.12)',
                    }
                }
            }
        }
    </script>
    
    <style>
        /* Custom scrollbar and subtle pattern */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #F7F2EA;
        }
        ::-webkit-scrollbar-thumb {
            background: #CBB28F;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #7A1C1C;
        }
        .bg-grid-pattern {
            background-image: radial-gradient(#8E6F47 0.75px, transparent 0.75px);
            background-size: 24px 24px;
            opacity: 0.15;
        }
    </style>
</head>
<body class="bg-earth-50 text-earth-900 font-sans antialiased selection:bg-maroon selection:text-white leading-relaxed">

    <!-- HEADER / NAVIGATION -->
    <header class="fixed top-0 left-0 right-0 z-50 bg-earth-50/90 backdrop-blur-md border-b border-earth-200/80 transition-all duration-300" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- Brand Logo -->
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-10 h-10 rounded-full bg-maroon text-earth-50 flex items-center justify-center font-serif font-bold text-xl shadow-md group-hover:bg-maroon-dark transition-colors">
                    K
                </div>
                <div class="flex flex-col">
                    <span class="font-serif font-bold text-lg text-earth-900 tracking-wide group-hover:text-maroon transition-colors">Kurnia Adela, S.Pd.</span>
                </div>
            </a>

            <!-- Desktop Menu -->
            <nav class="hidden md:flex items-center gap-8 font-medium text-sm text-earth-800">
                <a href="#about" class="hover:text-maroon transition-colors py-1 relative after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-maroon hover:after:w-full after:transition-all">Tentang Saya</a>
                <a href="#experience" class="hover:text-maroon transition-colors py-1 relative after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-maroon hover:after:w-full after:transition-all">Pengalaman</a>
                <a href="#projects" class="hover:text-maroon transition-colors py-1 relative after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-maroon hover:after:w-full after:transition-all">Proyek</a>
                <a href="#skills" class="hover:text-maroon transition-colors py-1 relative after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-maroon hover:after:w-full after:transition-all">Keahlian</a>
                <a href="#contact" class="hover:text-maroon transition-colors py-1 relative after:absolute after:bottom-0 after:left-0 after:w-0 after:h-0.5 after:bg-maroon hover:after:w-full after:transition-all">Kontak</a>
            </nav>

            <!-- CTA Header Button -->
            <div class="hidden md:flex items-center gap-3">
                <a href="#contact" class="px-5 py-2.5 rounded-full bg-maroon text-white font-medium text-sm hover:bg-maroon-dark transition-all duration-300 shadow-sm hover:shadow-md flex items-center gap-2">
                    <span>Hubungi Saya</span>
                    <i class="fa-solid fa-arrow-right text-xs"></i>
                </a>
            </div>

            <!-- Mobile Menu Toggle Button -->
            <button id="menu-btn" class="md:hidden p-2 rounded-lg text-earth-800 hover:bg-earth-100 focus:outline-none" aria-label="Toggle Navigation">
                <i class="fa-solid fa-bars text-xl" id="menu-icon"></i>
            </button>
        </div>

        <!-- Mobile Navigation Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-earth-50 border-b border-earth-200 px-6 py-6 space-y-4 shadow-lg transition-all">
            <a href="#about" class="block text-earth-800 font-medium hover:text-maroon transition-colors py-2">Tentang Saya</a>
            <a href="#experience" class="block text-earth-800 font-medium hover:text-maroon transition-colors py-2">Pengalaman</a>
            <a href="#projects" class="block text-earth-800 font-medium hover:text-maroon transition-colors py-2">Proyek</a>
            <a href="#skills" class="block text-earth-800 font-medium hover:text-maroon transition-colors py-2">Keahlian</a>
            <a href="#contact" class="block text-earth-800 font-medium hover:text-maroon transition-colors py-2">Kontak</a>
            <div class="pt-4 border-t border-earth-200">
                <a href="#contact" class="w-full py-3 rounded-xl bg-maroon text-white text-center font-medium block shadow">
                    Hubungi Saya
                </a>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="relative pt-32 pb-20 md:pt-40 md:pb-28 overflow-hidden">
        <!-- Subtle background pattern -->
        <div class="absolute inset-0 bg-grid-pattern pointer-events-none"></div>
        
        <!-- Ambient Warm Glows -->
        <div class="absolute top-1/4 -left-20 w-80 h-80 bg-earth-200/50 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute bottom-10 right-0 w-96 h-96 bg-maroon-soft/60 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-8 items-center">
                
                <!-- Left Column: Content -->
                <div class="lg:col-span-7 space-y-8">
                    <!-- Availability Pill -->
                    <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-earth-100 border border-earth-300/60 text-earth-800 text-xs sm:text-sm font-medium shadow-sm">
                        <span class="w-2.5 h-2.5 rounded-full bg-emerald-600 animate-pulse"></span>
                        <span>Terbuka untuk Peran Administrasi, Data, & Instructional Design</span>
                    </div>

                    <!-- Main Heading -->
                    <div class="space-y-3">
                        <h1 class="text-4xl sm:text-5xl lg:text-6xl font-serif font-bold text-earth-900 leading-tight">
                            Mengelola Data & Operasional dengan <span class="text-maroon underline decoration-earth-300 decoration-wavy decoration-2">Presisi</span> & Integritas.
                        </h1>
                        <p class="text-lg sm:text-xl text-earth-700 font-medium">
                            Kurnia Adela, S.Pd. – Administrative Specialist, Data Analyst & Educator
                        </p>
                    </div>

                    <!-- Target Quote / Tagline Section -->
                    <div class="relative p-6 sm:p-8 rounded-2xl bg-earth-100/80 border-l-4 border-maroon shadow-soft-warm backdrop-blur-sm">
                        <div class="absolute top-4 right-6 text-earth-300 text-4xl font-serif opacity-60">“</div>
                        <p class="text-earth-800 font-serif italic leading-relaxed text-sm sm:text-base relative z-10 pr-4">
                            "Tetap melangkah untuk menjadi pribadi yang bermanfaat, menunaikan kepercayaan dengan penuh tanggung jawab, serta menjadikan setiap perjuangan sebagai bukti bahwa pengorbanan orang tua tidak sia-sia."
                        </p>
                    </div>

                    <!-- Action Buttons (CTA) -->
                    <div class="flex flex-wrap items-center gap-4 pt-2">
                        <a href="#projects" class="px-7 py-3.5 rounded-full bg-maroon hover:bg-maroon-dark text-white font-semibold text-sm shadow-md hover:shadow-lg transition-all duration-300 flex items-center gap-3 group">
                            <span>Lihat Portofolio</span>
                            <i class="fa-solid fa-arrow-down group-hover:translate-y-1 transition-transform"></i>
                        </a>
                        <a href="#contact" class="px-7 py-3.5 rounded-full bg-earth-100 hover:bg-earth-200 text-earth-900 border border-earth-300 font-semibold text-sm transition-all duration-300 flex items-center gap-2">
                            <i class="fa-regular fa-paper-plane text-maroon"></i>
                            <span>Diskusi Kerjasama</span>
                        </a>
                        <a href="mailto:krniadlaa@gmail.com" class="px-5 py-3.5 rounded-full text-earth-700 hover:text-maroon text-sm font-medium transition-colors flex items-center gap-2">
                            <i class="fa-solid fa-envelope"></i>
                            <span>Kirim Email</span>
                        </a>
                    </div>

                    <!-- Social Media Quick Links -->
                    <div class="flex items-center gap-4 pt-4 border-t border-earth-200/80">
                        <span class="text-xs font-semibold uppercase tracking-wider text-earth-600">Terhubung:</span>
                        <div class="flex items-center gap-3">
                            <a href="https://linkedin.com/in/kurniaadela" target="_blank" rel="noopener noreferrer" class="w-9 h-9 rounded-full bg-earth-100 hover:bg-maroon hover:text-white text-earth-800 flex items-center justify-center transition-all duration-300" aria-label="LinkedIn">
                                <i class="fa-brands fa-linkedin-in text-sm"></i>
                            </a>
                            <a href="mailto:krniadlaa@gmail.com" class="w-9 h-9 rounded-full bg-earth-100 hover:bg-maroon hover:text-white text-earth-800 flex items-center justify-center transition-all duration-300" aria-label="Email">
                                <i class="fa-solid fa-envelope text-sm"></i>
                            </a>
                            <a href="https://wa.me/62895335507650" target="_blank" rel="noopener noreferrer" class="w-9 h-9 rounded-full bg-earth-100 hover:bg-maroon hover:text-white text-earth-800 flex items-center justify-center transition-all duration-300" aria-label="WhatsApp">
                                <i class="fa-brands fa-whatsapp text-sm"></i>
                            </a>
                        </div>
                    </div>
                </div>

                <!-- Right Column: Profile Card Visual -->
                <div class="lg:col-span-5 flex justify-center">
                    <div class="relative w-full max-w-md">
                        <!-- Decorative Frame Layer -->
                        <div class="absolute inset-0 bg-maroon rounded-3xl rotate-3 scale-95 opacity-20 transition-transform hover:rotate-6"></div>
                        <div class="absolute inset-0 bg-earth-300 rounded-3xl -rotate-2 scale-95 opacity-40"></div>
                        
                        <!-- Main Card Overlay -->
                        <div class="relative bg-earth-100 border border-earth-200 p-6 rounded-3xl shadow-hover-warm space-y-6">
                            <!-- Image / Avatar Container -->
                            <div class="relative h-96 rounded-2xl overflow-hidden bg-earth-200 group flex items-center justify-center">
                                <img id="hero-profile-img" src="MEITU_20260730_103042047.jpg.jpeg" 
                                     alt="Kurnia Adela, S.Pd." 
                                     class="w-full h-full object-cover object-center group-hover:scale-105 transition-transform duration-500"
                                     onerror="this.onerror=null; this.src='MEITU_20260730_103042047.jpg.jpeg';">
                                <div class="absolute inset-0 bg-gradient-to-t from-earth-900/80 via-transparent to-transparent"></div>
                                
                                <div class="absolute bottom-4 left-4 right-4 text-white">
                                    <p class="text-xs uppercase tracking-widest text-earth-200 font-semibold">Berbasis di</p>
                                    <p class="font-medium text-sm flex items-center gap-1.5">
                                        <i class="fa-solid fa-location-dot text-maroon-muted"></i>
                                        Tanjungpinang, Kepulauan Riau
                                    </p>
                                </div>
                            </div>

                            <!-- Highlights Info Pill -->
                            <div class="pt-2">
                                <div class="p-3.5 rounded-xl bg-earth-50 border border-earth-200 text-center shadow-sm">
                                    <span class="block text-2xl font-bold font-serif text-maroon">IPK 3.66</span>
                                    <span class="text-xs text-earth-600 font-medium">Lulusan Cumlaude</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- ABOUT ME SECTION -->
    <section id="about" class="py-20 bg-earth-100/60 border-y border-earth-200/80 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-3xl mx-auto text-center mb-16 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-maroon">Mengenal Lebih Dekat</span>
                <h2 class="text-3xl sm:text-4xl font-serif font-bold text-earth-900">Tentang Saya & Profesionalisme Kerja</h2>
                <div class="w-16 h-1 bg-maroon mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 items-center">
                <!-- Left text content -->
                <div class="lg:col-span-7 space-y-6 text-earth-800 leading-relaxed text-base">
                    <h3 class="text-2xl font-serif font-semibold text-earth-900">
                        Menggabungkan Analisis Kuantitatif dengan Tata Kelola Operasional & Komunikasi Efektif.
                    </h3>
                    <p>
                        Saya adalah seorang lulusan <strong class="text-maroon font-semibold">S1 Pendidikan Matematika</strong> dari Universitas Maritim Raja Ali Haji (UMRAH) dengan predikat *Honors* (IPK 3.66/4.00). Memiliki fondasi analitis kuantitatif yang kuat, pengolahan data terstruktur, serta keahlian penyusunan alur kerja administrasi.
                    </p>
                    <p>
                        Dengan pengalaman langsung sebagai Sekretaris Eksekutif Administrasi di lingkungan kemasyarakatan serta Asisten Pengajar & Instructional Designer di SMP Negeri 1 Tanjungpinang, saya terbiasa melakukan pemutakhiran data, pengarsipan digital 100% akurat, serta pengelolaan dinamika tim.
                    </p>
                    <p>
                        Bagi saya, kerapian administrasi dan kejelasan arus informasi adalah kunci utama efisiensi operasional suatu organisasi.
                    </p>

                    <!-- Core Value Cards -->
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 pt-4">
                        <div class="p-4 rounded-xl bg-earth-50 border border-earth-200 space-y-2">
                            <i class="fa-solid fa-database text-maroon text-xl"></i>
                            <h4 class="font-semibold text-earth-900 text-sm">Integritas Data</h4>
                            <p class="text-xs text-earth-600">Verifikasi dan validasi data dengan tingkat akurasi tinggi.</p>
                        </div>
                        <div class="p-4 rounded-xl bg-earth-50 border border-earth-200 space-y-2">
                            <i class="fa-solid fa-folder-tree text-maroon text-xl"></i>
                            <h4 class="font-semibold text-earth-900 text-sm">Pengarsipan Digital</h4>
                            <p class="text-xs text-earth-600">Sistem temu-kembali dokumen yang terstruktur & efisien.</p>
                        </div>
                        <div class="p-4 rounded-xl bg-earth-50 border border-earth-200 space-y-2">
                            <i class="fa-solid fa-handshake text-maroon text-xl"></i>
                            <h4 class="font-semibold text-earth-900 text-sm">Tanggung Jawab</h4>
                            <p class="text-xs text-earth-600">Komitmen penuh pada efisiensi tugas dan kepercayaan.</p>
                        </div>
                    </div>
                </div>

                <!-- Right Quick Details Box -->
                <div class="lg:col-span-5">
                    <div class="p-8 rounded-2xl bg-earth-50 border border-earth-200 shadow-soft-warm space-y-6">
                        <h4 class="font-serif font-bold text-xl text-earth-900 border-b border-earth-200 pb-4">
                            Informasi Ringkas CV
                        </h4>
                        
                        <div class="space-y-4 text-sm">
                            <div class="flex justify-between border-b border-earth-200/60 pb-3">
                                <span class="text-earth-600 font-medium">Nama Lengkap:</span>
                                <span class="font-semibold text-earth-900">Kurnia Adela, S.Pd.</span>
                            </div>
                            <div class="flex justify-between border-b border-earth-200/60 pb-3">
                                <span class="text-earth-600 font-medium">Pendidikan:</span>
                                <span class="font-semibold text-earth-900">S1 Pendidikan Matematika</span>
                            </div>
                            <div class="flex justify-between border-b border-earth-200/60 pb-3">
                                <span class="text-earth-600 font-medium">Institusi:</span>
                                <span class="font-semibold text-earth-900">UMRAH (IPK 3.66/4.00)</span>
                            </div>
                            <div class="flex justify-between border-b border-earth-200/60 pb-3">
                                <span class="text-earth-600 font-medium">Lokasi:</span>
                                <span class="font-semibold text-earth-900">Tanjungpinang, Riau Islands</span>
                            </div>
                            <div class="flex justify-between border-b border-earth-200/60 pb-3">
                                <span class="text-earth-600 font-medium">Kemampuan Bahasa:</span>
                                <span class="font-semibold text-earth-900">Indonesia & Inggris</span>
                            </div>
                            <div class="flex justify-between pb-1">
                                <span class="text-earth-600 font-medium">Status Karir:</span>
                                <span class="font-semibold text-emerald-700 bg-emerald-50 px-2 py-0.5 rounded text-xs">Siap Bekerja</span>
                            </div>
                        </div>

                        <div class="pt-2">
                            <a href="#contact" class="w-full py-3 rounded-xl bg-maroon hover:bg-maroon-dark text-white font-medium text-center block transition-colors">
                                Kirim Pesan Langsung
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- EXPERIENCE SECTION -->
    <section id="experience" class="py-20 bg-earth-50 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-3xl mx-auto text-center mb-16 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-maroon">Jejak Karir</span>
                <h2 class="text-3xl sm:text-4xl font-serif font-bold text-earth-900">Pengalaman Kerja & Organisasi</h2>
                <div class="w-16 h-1 bg-maroon mx-auto rounded-full"></div>
            </div>

            <!-- Experience Timeline -->
            <div class="max-w-4xl mx-auto relative before:absolute before:inset-0 before:left-4 sm:before:left-1/2 before:-ml-px before:w-0.5 before:bg-earth-300">
                
                <!-- Item 1 -->
                <div class="relative mb-12 sm:mb-16">
                    <div class="flex flex-col sm:flex-row items-start">
                        <!-- Dot Icon -->
                        <div class="absolute left-4 sm:left-1/2 -translate-x-1/2 w-8 h-8 rounded-full bg-maroon text-white flex items-center justify-center text-xs shadow-md z-10 my-1">
                            <i class="fa-solid fa-file-signature"></i>
                        </div>
                        
                        <!-- Content Card (Left or Right) -->
                        <div class="pl-12 sm:pl-0 sm:w-1/2 sm:pr-12 text-left sm:text-right">
                            <span class="inline-block px-3 py-1 rounded-full bg-maroon-soft text-maroon text-xs font-bold mb-2">2026 - 2031 (Ongoing)</span>
                            <h3 class="text-xl font-serif font-bold text-earth-900">Executive Administrative Secretary</h3>
                            <h4 class="text-sm font-semibold text-earth-600 mb-3">Rukun Tetangga (Local Neighborhood Organization)</h4>
                            <p class="text-sm text-earth-700 leading-relaxed bg-earth-100 p-5 rounded-2xl border border-earth-200">
                                Mengoperasikan pengarsipan digital dokumen kependudukan, verifikasi data bansos & sensus warga, serta mempercepat distribusi informasi organisasi hingga 30%.
                            </p>
                        </div>
                    </div>
                </div>

                <!-- Item 2 -->
                <div class="relative mb-12 sm:mb-16">
                    <div class="flex flex-col sm:flex-row items-start">
                        <!-- Dot Icon -->
                        <div class="absolute left-4 sm:left-1/2 -translate-x-1/2 w-8 h-8 rounded-full bg-earth-600 text-white flex items-center justify-center text-xs shadow-md z-10 my-1">
                            <i class="fa-solid fa-chalkboard-user"></i>
                        </div>
                        
                        <!-- Content Card (Right side on desktop) -->
                        <div class="pl-12 sm:pl-0 sm:w-1/2 sm:ml-auto sm:pl-12 text-left">
                            <span class="inline-block px-3 py-1 rounded-full bg-earth-200 text-earth-800 text-xs font-bold mb-2">Agt 2024 - Des 2024</span>
                            <h3 class="text-xl font-serif font-bold text-earth-900">Teaching Assistant & Instructional Designer</h3>
                            <h4 class="text-sm font-semibold text-earth-600 mb-3">SMP Negeri 1 Tanjungpinang</h4>
                            <p class="text-sm text-earth-700 leading-relaxed bg-earth-100 p-5 rounded-2xl border border-earth-200">
                                Merancang modul pembelajaran interaktif untuk 120+ siswa, menyusun metrik evaluasi pemahaman berbasis data, serta mengelola dinamika kelompok besar (30+ siswa per sesi).
                            </p>
                        </div>
                    </div>
                </div>

                <!-- Item 3 -->
                <div class="relative">
                    <div class="flex flex-col sm:flex-row items-start">
                        <!-- Dot Icon -->
                        <div class="absolute left-4 sm:left-1/2 -translate-x-1/2 w-8 h-8 rounded-full bg-earth-400 text-white flex items-center justify-center text-xs shadow-md z-10 my-1">
                            <i class="fa-solid fa-bullhorn"></i>
                        </div>
                        
                        <!-- Content Card (Left side on desktop) -->
                        <div class="pl-12 sm:pl-0 sm:w-1/2 sm:pr-12 text-left sm:text-right">
                            <span class="inline-block px-3 py-1 rounded-full bg-earth-200 text-earth-800 text-xs font-bold mb-2">Agustus 2025</span>
                            <h3 class="text-xl font-serif font-bold text-earth-900">Public Relations Officer</h3>
                            <h4 class="text-sm font-semibold text-earth-600 mb-3">Kuliah Kerja Nyata (KKN) UMRAH</h4>
                            <p class="text-sm text-earth-700 leading-relaxed bg-earth-100 p-5 rounded-2xl border border-earth-200">
                                Mengordinasikan komunikasi inter-organisasi antara ketua komite, peserta program, dan perangkat pemerintah daerah untuk memastikan kelancaran program kerja.
                            </p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- PROJECTS SECTION -->
    <section id="projects" class="py-20 bg-earth-100/50 border-t border-earth-200/80">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-3xl mx-auto text-center mb-12 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-maroon">Karya & Portfolio Studi</span>
                <h2 class="text-3xl sm:text-4xl font-serif font-bold text-earth-900">Proyek Administrasi & Analisis Pilihan</h2>
                <div class="w-16 h-1 bg-maroon mx-auto rounded-full"></div>
            </div>

            <!-- Project Filter Tabs -->
            <div class="flex flex-wrap items-center justify-center gap-2 mb-12">
                <button class="filter-btn active px-5 py-2 rounded-full bg-maroon text-white text-sm font-medium transition-all shadow-sm" data-filter="all">Semua Proyek</button>
                <button class="filter-btn px-5 py-2 rounded-full bg-earth-200/70 hover:bg-earth-300 text-earth-800 text-sm font-medium transition-all" data-filter="admin">Administrasi & Data</button>
                <button class="filter-btn px-5 py-2 rounded-full bg-earth-200/70 hover:bg-earth-300 text-earth-800 text-sm font-medium transition-all" data-filter="edu">Media & E-Learning</button>
                <button class="filter-btn px-5 py-2 rounded-full bg-earth-200/70 hover:bg-earth-300 text-earth-800 text-sm font-medium transition-all" data-filter="biz">Pengembangan Bisnis</button>
            </div>

            <!-- Projects Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- Project Card 1 -->
                <div class="project-card group bg-earth-50 border border-earth-200 rounded-2xl overflow-hidden shadow-soft-warm hover:shadow-hover-warm transition-all duration-300 flex flex-col" data-category="admin">
                    <div class="relative overflow-hidden h-52 bg-earth-200 flex items-center justify-center">
                        <img src="https://images.unsplash.com/photo-1450133064473-71024230f91b?q=80&w=800&auto=format&fit=crop" 
                             alt="Administrative Optimization Project" 
                             class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
                             onerror="this.src='https://placehold.co/600x400/8E6F47/FFF?text=Archival+Optimization'">
                        <div class="absolute inset-0 bg-earth-900/40 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center gap-3">
                            <a href="#contact" class="w-10 h-10 rounded-full bg-earth-50 text-maroon flex items-center justify-center shadow hover:scale-110 transition-transform" title="Detail Dokumen">
                                <i class="fa-solid fa-file-lines"></i>
                            </a>
                        </div>
                    </div>
                    <div class="p-6 flex-1 flex flex-col justify-between space-y-4">
                        <div>
                            <div class="flex items-center justify-between text-xs text-earth-600 mb-2">
                                <span class="font-semibold text-maroon bg-maroon-soft px-2.5 py-0.5 rounded">Proyek Administrasi</span>
                                <span>2026</span>
                            </div>
                            <h3 class="text-xl font-serif font-bold text-earth-900 group-hover:text-maroon transition-colors">Digital Archival & Quality Control Workflow</h3>
                            <p class="text-sm text-earth-700 mt-2 line-clamp-3">
                                Standardisasi template dokumentasi dan audit alur pengarsipan yang berhasil meminimalkan risiko kesalahan input data operasional secara signifikan.
                            </p>
                        </div>
                        <div class="pt-4 border-t border-earth-200/80 flex flex-wrap gap-2">
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">Document Archiving</span>
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">Data Auditing</span>
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">Standardization</span>
                        </div>
                    </div>
                </div>

                <!-- Project Card 2 -->
                <div class="project-card group bg-earth-50 border border-earth-200 rounded-2xl overflow-hidden shadow-soft-warm hover:shadow-hover-warm transition-all duration-300 flex flex-col" data-category="edu">
                    <div class="relative overflow-hidden h-52 bg-earth-200 flex items-center justify-center">
                        <img src="https://images.unsplash.com/photo-1509062522246-3755977927d7?q=80&w=800&auto=format&fit=crop" 
                             alt="Interactive Digital Media Project" 
                             class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
                             onerror="this.src='https://placehold.co/600x400/7A1C1C/FFF?text=Digital+Instructional+Media'">
                        <div class="absolute inset-0 bg-earth-900/40 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center gap-3">
                            <a href="#contact" class="w-10 h-10 rounded-full bg-earth-50 text-maroon flex items-center justify-center shadow hover:scale-110 transition-transform" title="Detail Modul">
                                <i class="fa-solid fa-laptop-code"></i>
                            </a>
                        </div>
                    </div>
                    <div class="p-6 flex-1 flex flex-col justify-between space-y-4">
                        <div>
                            <div class="flex items-center justify-between text-xs text-earth-600 mb-2">
                                <span class="font-semibold text-maroon bg-maroon-soft px-2.5 py-0.5 rounded">Desain Instruksional</span>
                                <span>2024</span>
                            </div>
                            <h3 class="text-xl font-serif font-bold text-earth-900 group-hover:text-maroon transition-colors">Interactive Media & Systems Design</h3>
                            <p class="text-sm text-earth-700 mt-2 line-clamp-3">
                                Perancangan konten digital interaktif berbasis Hirarki Informasi Logis (Information Hierarchy) untuk meningkatkan daya serap materi pembelajaran siswa.
                            </p>
                        </div>
                        <div class="pt-4 border-t border-earth-200/80 flex flex-wrap gap-2">
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">Instructional Design</span>
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">Information Flow</span>
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">Evaluation Analytics</span>
                        </div>
                    </div>
                </div>

                <!-- Project Card 3 -->
                <div class="project-card group bg-earth-50 border border-earth-200 rounded-2xl overflow-hidden shadow-soft-warm hover:shadow-hover-warm transition-all duration-300 flex flex-col" data-category="biz">
                    <div class="relative overflow-hidden h-52 bg-earth-200 flex items-center justify-center">
                        <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?q=80&w=800&auto=format&fit=crop" 
                             alt="Business & Financial Modeling" 
                             class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
                             onerror="this.src='https://placehold.co/600x400/4A3722/FFF?text=Financial+Modeling'">
                        <div class="absolute inset-0 bg-earth-900/40 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center gap-3">
                            <a href="#contact" class="w-10 h-10 rounded-full bg-earth-50 text-maroon flex items-center justify-center shadow hover:scale-110 transition-transform" title="Detail Model">
                                <i class="fa-solid fa-chart-line"></i>
                            </a>
                        </div>
                    </div>
                    <div class="p-6 flex-1 flex flex-col justify-between space-y-4">
                        <div>
                            <div class="flex items-center justify-between text-xs text-earth-600 mb-2">
                                <span class="font-semibold text-maroon bg-maroon-soft px-2.5 py-0.5 rounded">Riset & Analisis Produk</span>
                                <span>2025</span>
                            </div>
                            <h3 class="text-xl font-serif font-bold text-earth-900 group-hover:text-maroon transition-colors">Financial Modeling & Product Strategy</h3>
                            <p class="text-sm text-earth-700 mt-2 line-clamp-3">
                                Simulasi perhitungan Harga Pokok Penjualan (HPP), strategi penetapan harga kompetitif, serta kampanye Pre-Order untuk validasi respon pasar.
                            </p>
                        </div>
                        <div class="pt-4 border-t border-earth-200/80 flex flex-wrap gap-2">
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">Financial Modeling</span>
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">HPP Calculation</span>
                            <span class="text-xs px-2.5 py-1 rounded-md bg-earth-200 text-earth-800 font-medium">Market Strategy</span>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SKILLS SECTION -->
    <section id="skills" class="py-20 bg-earth-50 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-3xl mx-auto text-center mb-16 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-maroon">Kemampuan Teknis & Kompetensi</span>
                <h2 class="text-3xl sm:text-4xl font-serif font-bold text-earth-900">Keahlian & Perangkat Kerja</h2>
                <div class="w-16 h-1 bg-maroon mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- Skill Category 1 -->
                <div class="p-8 rounded-2xl bg-earth-100 border border-earth-200 shadow-soft-warm space-y-6">
                    <div class="flex items-center gap-3 border-b border-earth-200 pb-4">
                        <div class="w-10 h-10 rounded-xl bg-maroon text-white flex items-center justify-center text-lg">
                            <i class="fa-solid fa-folder-closed"></i>
                        </div>
                        <div>
                            <h3 class="font-serif font-bold text-lg text-earth-900">Administrasi & Arsip</h3>
                            <p class="text-xs text-earth-600">Manajemen Operasional</p>
                        </div>
                    </div>
                    
                    <div class="flex flex-wrap gap-2.5">
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-box-archive text-maroon text-sm"></i> Document Archiving
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-square-check text-emerald-700 text-sm"></i> Data Verification
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-shield-heart text-amber-700 text-sm"></i> Quality Control
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-building text-earth-700 text-sm"></i> Office Administration
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-list-check text-earth-700 text-sm"></i> Records Management
                        </span>
                    </div>
                </div>

                <!-- Skill Category 2 -->
                <div class="p-8 rounded-2xl bg-earth-100 border border-earth-200 shadow-soft-warm space-y-6">
                    <div class="flex items-center gap-3 border-b border-earth-200 pb-4">
                        <div class="w-10 h-10 rounded-xl bg-earth-800 text-white flex items-center justify-center text-lg">
                            <i class="fa-solid fa-microchip"></i>
                        </div>
                        <div>
                            <h3 class="font-serif font-bold text-lg text-earth-900">Perangkat & Software</h3>
                            <p class="text-xs text-earth-600">Teknologi & Pengolahan Data</p>
                        </div>
                    </div>
                    
                    <div class="flex flex-wrap gap-2.5">
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-file-excel text-emerald-600 text-sm"></i> MS Excel / Sheets
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-file-word text-blue-600 text-sm"></i> MS Word / Docs
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-file-powerpoint text-orange-600 text-sm"></i> PowerPoint / Slides
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-brands fa-google text-red-500 text-sm"></i> Google Workspace
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-chart-pie text-purple-600 text-sm"></i> Quantitative Analysis
                        </span>
                    </div>
                </div>

                <!-- Skill Category 3 -->
                <div class="p-8 rounded-2xl bg-earth-100 border border-earth-200 shadow-soft-warm space-y-6">
                    <div class="flex items-center gap-3 border-b border-earth-200 pb-4">
                        <div class="w-10 h-10 rounded-xl bg-maroon-muted text-white flex items-center justify-center text-lg">
                            <i class="fa-solid fa-users text-lg"></i>
                        </div>
                        <div>
                            <h3 class="font-serif font-bold text-lg text-earth-900">Komunikasi & Soft Skills</h3>
                            <p class="text-xs text-earth-600">Interaksi & Kepemimpinan</p>
                        </div>
                    </div>
                    
                    <div class="flex flex-wrap gap-2.5">
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-comments text-sky-600 text-sm"></i> Public Relations
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-microphone text-rose-600 text-sm"></i> Public Speaking
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-people-roof text-indigo-600 text-sm"></i> Team Management
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-scale-balanced text-amber-700 text-sm"></i> Conflict Resolution
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-earth-50 border border-earth-200 text-earth-900 text-xs font-semibold hover:border-maroon transition-colors shadow-sm">
                            <i class="fa-solid fa-pen-fancy text-earth-700 text-sm"></i> Copywriting
                        </span>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- CONTACT SECTION -->
    <section id="contact" class="py-20 bg-earth-100/70 border-t border-earth-200 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="max-w-3xl mx-auto text-center mb-16 space-y-3">
                <span class="text-xs font-bold uppercase tracking-widest text-maroon">Mari Bekerja Sama</span>
                <h2 class="text-3xl sm:text-4xl font-serif font-bold text-earth-900">Hubungi Saya</h2>
                <p class="text-earth-700 text-sm sm:text-base">
                    Apakah Anda membutuhkan tenaga profesional di bidang administrasi, pengelolaan data, atau pengarsipan? Mari berdiskusi.
                </p>
                <div class="w-16 h-1 bg-maroon mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12">
                <!-- Contact Info Box -->
                <div class="lg:col-span-5 space-y-8">
                    <div class="bg-earth-50 border border-earth-200 p-8 rounded-2xl shadow-soft-warm space-y-6">
                        <h3 class="font-serif font-bold text-2xl text-earth-900">Detail Kontak</h3>
                        
                        <div class="space-y-6">
                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 rounded-xl bg-maroon-soft text-maroon flex items-center justify-center shrink-0">
                                    <i class="fa-regular fa-envelope text-lg"></i>
                                </div>
                                <div>
                                    <span class="text-xs font-semibold uppercase text-earth-600 block">Email Resmi</span>
                                    <a href="mailto:krniadlaa@gmail.com" class="text-base font-semibold text-earth-900 hover:text-maroon transition-colors">
                                        krniadlaa@gmail.com
                                    </a>
                                </div>
                            </div>

                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 rounded-xl bg-earth-200 text-earth-800 flex items-center justify-center shrink-0">
                                    <i class="fa-brands fa-whatsapp text-lg"></i>
                                </div>
                                <div>
                                    <span class="text-xs font-semibold uppercase text-earth-600 block">WhatsApp / Telepon</span>
                                    <a href="https://wa.me/62895335507650" target="_blank" rel="noopener noreferrer" class="text-base font-semibold text-earth-900 hover:text-maroon transition-colors">
                                        +62 895-3355-07650
                                    </a>
                                </div>
                            </div>

                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 rounded-xl bg-earth-200 text-earth-800 flex items-center justify-center shrink-0">
                                    <i class="fa-brands fa-linkedin-in text-lg"></i>
                                </div>
                                <div>
                                    <span class="text-xs font-semibold uppercase text-earth-600 block">LinkedIn Profile</span>
                                    <a href="https://linkedin.com/in/kurniaadela" target="_blank" rel="noopener noreferrer" class="text-base font-semibold text-earth-900 hover:text-maroon transition-colors">
                                        linkedin.com/in/kurniaadela
                                    </a>
                                </div>
                            </div>

                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 rounded-xl bg-earth-200 text-earth-800 flex items-center justify-center shrink-0">
                                    <i class="fa-solid fa-location-dot text-lg"></i>
                                </div>
                                <div>
                                    <span class="text-xs font-semibold uppercase text-earth-600 block">Lokasi</span>
                                    <p class="text-base font-semibold text-earth-900">
                                        Tanjungpinang, Kepulauan Riau, Indonesia
                                    </p>
                                </div>
                            </div>
                        </div>

                        <!-- Response Time Badge -->
                        <div class="p-4 rounded-xl bg-earth-100/80 border border-earth-200 text-xs text-earth-700 flex items-center gap-3">
                            <i class="fa-regular fa-clock text-maroon text-base"></i>
                            <span>Waktu respons rata-rata: <strong>&lt; 24 jam</strong> pada hari kerja.</span>
                        </div>
                    </div>
                </div>

                <!-- Contact Form -->
                <div class="lg:col-span-7">
                    <form id="contact-form" class="bg-earth-50 border border-earth-200 p-8 rounded-2xl shadow-soft-warm space-y-6">
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                            <div class="space-y-2">
                                <label for="name" class="text-xs font-bold uppercase tracking-wider text-earth-800">Nama Lengkap *</label>
                                <input type="text" id="name" required placeholder="Nama Anda" 
                                       class="w-full px-4 py-3 rounded-xl bg-earth-100/50 border border-earth-300 text-earth-900 text-sm focus:outline-none focus:border-maroon focus:ring-1 focus:ring-maroon transition-all">
                            </div>
                            <div class="space-y-2">
                                <label for="email" class="text-xs font-bold uppercase tracking-wider text-earth-800">Alamat Email *</label>
                                <input type="email" id="email" required placeholder="email@domain.com" 
                                       class="w-full px-4 py-3 rounded-xl bg-earth-100/50 border border-earth-300 text-earth-900 text-sm focus:outline-none focus:border-maroon focus:ring-1 focus:ring-maroon transition-all">
                            </div>
                        </div>

                        <div class="space-y-2">
                            <label for="subject" class="text-xs font-bold uppercase tracking-wider text-earth-800">Subjek Pesan</label>
                            <input type="text" id="subject" placeholder="Penawaran Kerjasama Administrasi / Data" 
                                   class="w-full px-4 py-3 rounded-xl bg-earth-100/50 border border-earth-300 text-earth-900 text-sm focus:outline-none focus:border-maroon focus:ring-1 focus:ring-maroon transition-all">
                        </div>

                        <div class="space-y-2">
                            <label for="message" class="text-xs font-bold uppercase tracking-wider text-earth-800">Pesan Anda *</label>
                            <textarea id="message" rows="5" required placeholder="Tuliskan detail kebutuhan atau pertanyaan Anda..." 
                                      class="w-full px-4 py-3 rounded-xl bg-earth-100/50 border border-earth-300 text-earth-900 text-sm focus:outline-none focus:border-maroon focus:ring-1 focus:ring-maroon transition-all resize-none"></textarea>
                        </div>

                        <button type="submit" class="w-full py-4 rounded-xl bg-maroon hover:bg-maroon-dark text-white font-bold text-sm tracking-wide shadow-md transition-all duration-300 flex items-center justify-center gap-2">
                            <i class="fa-regular fa-paper-plane"></i>
                            <span>Kirim Pesan Sekarang</span>
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- SUCCESS TOAST NOTIFICATION (No Alert UI) -->
    <div id="toast-success" class="fixed bottom-6 right-6 z-50 transform translate-y-24 opacity-0 transition-all duration-300 max-w-sm w-full bg-earth-900 text-earth-50 border border-earth-700 p-4 rounded-2xl shadow-2xl flex items-center gap-4 pointer-events-none">
        <div class="w-10 h-10 rounded-full bg-emerald-800 text-emerald-200 flex items-center justify-center shrink-0">
            <i class="fa-solid fa-check text-lg"></i>
        </div>
        <div class="flex-1">
            <h4 class="font-bold text-sm text-white">Pesan Terkirim!</h4>
            <p class="text-xs text-earth-300">Terima kasih. Saya akan merespons pesan Anda secepatnya.</p>
        </div>
        <button id="close-toast" class="text-earth-400 hover:text-white text-sm p-1">
            <i class="fa-solid fa-xmark"></i>
        </button>
    </div>

    <!-- FOOTER -->
    <footer class="bg-earth-900 text-earth-300 py-12 border-t border-earth-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row items-center justify-between gap-6 pb-8 border-b border-earth-800">
                <!-- Brand -->
                <div class="flex items-center gap-3">
                    <div class="w-9 h-9 rounded-full bg-maroon text-white flex items-center justify-center font-serif font-bold">
                        K
                    </div>
                    <span class="font-serif font-bold text-lg text-white">Kurnia Adela, S.Pd.</span>
                </div>

                <!-- Footer Nav Links -->
                <div class="flex flex-wrap justify-center gap-6 text-xs font-medium text-earth-300">
                    <a href="#about" class="hover:text-white transition-colors">Tentang</a>
                    <a href="#experience" class="hover:text-white transition-colors">Pengalaman</a>
                    <a href="#projects" class="hover:text-white transition-colors">Proyek</a>
                    <a href="#skills" class="hover:text-white transition-colors">Keahlian</a>
                    <a href="#contact" class="hover:text-white transition-colors">Kontak</a>
                </div>

                <!-- Back to Top Button -->
                <a href="#" class="w-10 h-10 rounded-full bg-earth-800 hover:bg-maroon text-white flex items-center justify-center transition-colors" title="Kembali ke Atas">
                    <i class="fa-solid fa-arrow-up text-xs"></i>
                </a>
            </div>

            <div class="pt-8 flex flex-col sm:flex-row items-center justify-between text-xs text-earth-400 gap-4">
                <p>&copy; 2026 Kurnia Adela, S.Pd. Hak Cipta Dilindungi Undang-Undang.</p>
                <p class="italic">Dirancang dengan dedikasi & kehangatan nuansa beige & maroon earth tone.</p>
            </div>
        </div>
    </footer>

    <!-- INTERACTIVE JAVASCRIPT LOGIC -->
    <script>
        document.addEventListener('DOMContentLoaded', function () {
            // Mobile Menu Toggle
            const menuBtn = document.getElementById('menu-btn');
            const mobileMenu = document.getElementById('mobile-menu');
            const menuIcon = document.getElementById('menu-icon');

            if (menuBtn && mobileMenu) {
                menuBtn.addEventListener('click', function () {
                    mobileMenu.classList.toggle('hidden');
                    if (mobileMenu.classList.contains('hidden')) {
                        menuIcon.className = 'fa-solid fa-bars text-xl';
                    } else {
                        menuIcon.className = 'fa-solid fa-xmark text-xl';
                    }
                });

                // Close mobile menu when clicking nav links
                const mobileNavLinks = mobileMenu.querySelectorAll('a');
                mobileNavLinks.forEach(link => {
                    link.addEventListener('click', () => {
                        mobileMenu.classList.add('hidden');
                        menuIcon.className = 'fa-solid fa-bars text-xl';
                    });
                });
            }

            // Project Filter Interactive Tabs
            const filterBtns = document.querySelectorAll('.filter-btn');
            const projectCards = document.querySelectorAll('.project-card');

            filterBtns.forEach(btn => {
                btn.addEventListener('click', () => {
                    // Remove active styles from all buttons
                    filterBtns.forEach(b => {
                        b.classList.remove('active', 'bg-maroon', 'text-white');
                        b.classList.add('bg-earth-200/70', 'text-earth-800');
                    });

                    // Add active style to clicked button
                    btn.classList.add('active', 'bg-maroon', 'text-white');
                    btn.classList.remove('bg-earth-200/70', 'text-earth-800');

                    const filterValue = btn.getAttribute('data-filter');

                    projectCards.forEach(card => {
                        if (filterValue === 'all' || card.getAttribute('data-category') === filterValue) {
                            card.style.display = 'flex';
                        } else {
                            card.style.display = 'none';
                        }
                    });
                });
            });

            // Contact Form Handling (Interactive Toast Alert)
            const contactForm = document.getElementById('contact-form');
            const toast = document.getElementById('toast-success');
            const closeToast = document.getElementById('close-toast');

            if (contactForm && toast) {
                contactForm.addEventListener('submit', function (e) {
                    e.preventDefault();

                    // Show Toast Notification
                    toast.classList.remove('translate-y-24', 'opacity-0', 'pointer-events-none');

                    // Reset form fields
                    contactForm.reset();

                    // Auto hide after 5 seconds
                    setTimeout(() => {
                        toast.classList.add('translate-y-24', 'opacity-0', 'pointer-events-none');
                    }, 5000);
                });

                if (closeToast) {
                    closeToast.addEventListener('click', () => {
                        toast.classList.add('translate-y-24', 'opacity-0', 'pointer-events-none');
                    });
                }
            }
        });
    </script>
</body>
</html>
