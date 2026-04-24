<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LABKOM 45 - Digital Log System</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Tailwind Config untuk animasi custom -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    animation: {
                        'shimmer': 'shimmer 1.5s infinite',
                        'pulse-slow': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                    },
                    keyframes: {
                        shimmer: {
                            '100%': { transform: 'translateX(100%)' }
                        }
                    }
                }
            }
        }
    </script>

    <!-- Custom Styles -->
    <style>
        /* Sembunyikan elemen yang belum aktif */
        .hidden-view { display: none !important; }
        
        /* Custom Scrollbar */
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #0f172a; }
        ::-webkit-scrollbar-thumb { background: #334155; border-radius: 4px; }
        ::-webkit-scrollbar-thumb:hover { background: #475569; }

        body {
            background-color: #020617; /* slate-950 */
            color: #e2e8f0; /* slate-200 */
        }
    </style>

    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
</head>
<body class="min-h-screen font-sans relative overflow-x-hidden selection:bg-indigo-500/30">

    <!-- Premium Background Effects -->
    <div class="fixed top-[-10%] left-[-10%] w-[40%] h-[40%] rounded-full bg-indigo-600/20 blur-[120px] pointer-events-none z-0"></div>
    <div class="fixed bottom-[-10%] right-[-10%] w-[40%] h-[40%] rounded-full bg-cyan-600/10 blur-[120px] pointer-events-none z-0"></div>

    <!-- Navbar Glassmorphism -->
    <nav class="sticky top-0 z-50 bg-slate-950/60 backdrop-blur-2xl border-b border-slate-800/60">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex items-center justify-between h-20">
            <div class="flex items-center gap-4">
                <div class="relative group cursor-pointer">
                    <div class="absolute inset-0 bg-indigo-500 rounded-xl blur opacity-40 group-hover:opacity-70 transition-opacity"></div>
                    <div class="relative bg-slate-900 border border-slate-700 p-2.5 rounded-xl">
                        <i data-lucide="monitor" class="text-indigo-400 w-6 h-6"></i>
                    </div>
                </div>
                <div>
                    <h1 class="font-bold text-xl tracking-wide text-white flex items-center gap-1">
                        LABKOM <span class="text-transparent bg-clip-text bg-gradient-to-r from-indigo-400 to-cyan-400">45</span>
                    </h1>
                    <p class="text-[10px] text-slate-400 tracking-widest uppercase font-semibold">Digital Log System</p>
                </div>
            </div>
            
            <div class="flex bg-slate-900/50 p-1.5 rounded-2xl border border-slate-800">
                <button onclick="switchView('check-in')" id="nav-check-in" class="nav-btn px-5 py-2.5 rounded-xl text-sm font-semibold transition-all flex items-center gap-2 bg-indigo-600/20 text-indigo-400 shadow-[inset_0_1px_1px_rgba(255,255,255,0.1)] border border-indigo-500/30">
                    <i data-lucide="user-plus" class="w-4 h-4"></i> <span class="hidden sm:inline">Presensi</span>
                </button>
                <button onclick="switchView('admin')" id="nav-admin" class="nav-btn px-5 py-2.5 rounded-xl text-sm font-semibold transition-all flex items-center gap-2 text-slate-400 hover:text-slate-200 hover:bg-slate-800 border border-transparent">
                    <i data-lucide="layout-dashboard" class="w-4 h-4"></i> <span class="hidden sm:inline">Dashboard</span>
                </button>
            </div>
        </div>
    </nav>

    <!-- MAIN CONTENT -->
    <main class="max-w-7xl mx-auto px-4 py-10 relative z-10">
        
        <!-- ==================== VIEW: CHECK-IN ==================== -->
        <div id="view-check-in" class="max-w-3xl mx-auto transition-opacity duration-500">
            
            <!-- Success Message (Hidden by default) -->
            <div id="success-message" class="hidden-view bg-slate-900/80 backdrop-blur-xl border border-emerald-500/30 p-12 rounded-[2rem] text-center shadow-2xl shadow-emerald-900/20">
                <div class="relative inline-block mb-6">
                    <div class="absolute inset-0 bg-emerald-500 blur-xl opacity-40 animate-pulse"></div>
                    <div class="relative bg-gradient-to-br from-emerald-400 to-emerald-600 w-20 h-20 rounded-2xl flex items-center justify-center shadow-inner mx-auto">
                        <i data-lucide="check-circle-2" class="text-white w-10 h-10"></i>
                    </div>
                </div>
                <h3 class="text-white font-black text-3xl mb-2 flex items-center justify-center gap-2">
                    Akses Diberikan <i data-lucide="sparkles" class="text-yellow-400 w-6 h-6"></i>
                </h3>
                <p class="text-emerald-400 text-lg font-medium">Data kunjungan Anda telah terenkripsi & tersimpan.</p>
                <p class="text-slate-500 mt-6 text-sm">Mengalihkan ke dashboard...</p>
            </div>

            <!-- Formulir Presensi -->
            <div id="form-container" class="bg-slate-900/60 backdrop-blur-xl border border-slate-800 p-8 sm:p-10 rounded-[2rem] shadow-2xl">
                <div class="mb-10 flex items-center gap-4 border-b border-slate-800 pb-8">
                    <div class="bg-indigo-500/10 p-4 rounded-2xl border border-indigo-500/20">
                        <i data-lucide="activity" class="text-indigo-400 w-8 h-8"></i>
                    </div>
                    <div>
                        <h2 class="text-3xl font-black text-white tracking-tight">Otorisasi Kunjungan</h2>
                        <p class="text-slate-400 mt-1">Lengkapi kredensial Anda untuk mengakses fasilitas.</p>
                    </div>
                </div>

                <form id="checkInForm" onsubmit="handleFormSubmit(event)" class="space-y-8">
                    <!-- Pilihan Lab -->
                    <div class="space-y-4">
                        <label class="text-xs font-bold text-slate-400 uppercase tracking-widest flex items-center gap-2">
                            <i data-lucide="monitor" class="w-3.5 h-3.5"></i> Pilih Sektor Laboratorium
                        </label>
                        <div class="grid grid-cols-1 sm:grid-cols-3 gap-4" id="lab-selection">
                            <!-- Tombol lab di-generate via JS -->
                        </div>
                        <input type="hidden" id="labId" name="labId" value="Lab 1" required>
                    </div>

                    <!-- Identitas -->
                    <div class="space-y-4">
                        <label class="text-xs font-bold text-slate-400 uppercase tracking-widest flex items-center gap-2">
                            <i data-lucide="user" class="w-3.5 h-3.5"></i> Identitas Pengguna
                        </label>
                        <div class="relative group">
                            <div class="absolute inset-y-0 left-0 pl-4 flex items-center pointer-events-none">
                                <div class="h-5 w-5 rounded-full bg-slate-800 flex items-center justify-center border border-slate-700">
                                    <i data-lucide="user" class="text-slate-400 w-2.5 h-2.5"></i>
                                </div>
                            </div>
                            <input required type="text" id="name" name="name" class="w-full pl-12 pr-5 py-4 rounded-2xl bg-slate-950/50 border border-slate-800 text-white placeholder-slate-600 focus:bg-slate-900 focus:ring-2 focus:ring-indigo-500/50 focus:border-indigo-500 transition-all outline-none" placeholder="Masukkan nama lengkap Anda...">
                        </div>
                    </div>

                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                        <!-- Kelas -->
                        <div class="space-y-4">
                            <label class="text-xs font-bold text-slate-400 uppercase tracking-widest flex items-center gap-2">
                                <i data-lucide="book-open" class="w-3.5 h-3.5"></i> Kelas / Divisi
                            </label>
                            <input required type="text" id="class" name="class" class="w-full px-5 py-4 rounded-2xl bg-slate-950/50 border border-slate-800 text-white placeholder-slate-600 focus:bg-slate-900 focus:ring-2 focus:ring-indigo-500/50 focus:border-indigo-500 transition-all outline-none" placeholder="Contoh: XII A">
                        </div>
                        <!-- Nomor PC -->
                        <div class="space-y-4">
                            <label class="text-xs font-bold text-slate-400 uppercase tracking-widest flex items-center gap-2">
                                <i data-lucide="cpu" class="w-3.5 h-3.5"></i> Workstation (PC)
                            </label>
                            <div class="relative">
                                <div class="absolute inset-y-0 left-0 pl-4 flex items-center pointer-events-none">
                                    <span class="text-slate-500 font-mono font-bold">PC-</span>
                                </div>
                                <input required type="number" id="computerNo" name="computerNo" class="w-full pl-12 pr-5 py-4 rounded-2xl bg-slate-950/50 border border-slate-800 text-white placeholder-slate-600 focus:bg-slate-900 focus:ring-2 focus:ring-indigo-500/50 focus:border-indigo-500 transition-all outline-none font-mono" placeholder="01">
                            </div>
                        </div>
                    </div>

                    <!-- Keperluan -->
                    <div class="space-y-4">
                        <label class="text-xs font-bold text-slate-400 uppercase tracking-widest flex items-center gap-2">
                            <i data-lucide="clipboard-list" class="w-3.5 h-3.5"></i> Tujuan Penggunaan
                        </label>
                        <select required id="purpose" name="purpose" class="w-full px-5 py-4 rounded-2xl bg-slate-950/50 border border-slate-800 text-white focus:bg-slate-900 focus:ring-2 focus:ring-indigo-500/50 focus:border-indigo-500 transition-all outline-none appearance-none">
                            <option value="" class="bg-slate-900 text-slate-500">Pilih Objektif...</option>
                            <option value="Praktikum Mandiri" class="bg-slate-900 text-white">Praktikum Mandiri</option>
                            <option value="Tugas Mapel" class="bg-slate-900 text-white">Penyelesaian Tugas</option>
                            <option value="Riset Terpadu" class="bg-slate-900 text-white">Riset Terpadu</option>
                            <option value="Ujian / Sertifikasi" class="bg-slate-900 text-white">Ujian / Sertifikasi</option>
                        </select>
                    </div>

                    <button type="submit" id="submitBtn" class="group relative w-full py-5 rounded-2xl font-bold text-lg overflow-hidden transition-all duration-300 flex items-center justify-center gap-3 bg-white text-slate-900 hover:bg-slate-100 shadow-[0_0_40px_rgba(255,255,255,0.1)] hover:shadow-[0_0_60px_rgba(255,255,255,0.2)] hover:-translate-y-1">
                        <div class="absolute inset-0 bg-gradient-to-r from-transparent via-white/50 to-transparent translate-x-[-100%] group-hover:animate-[shimmer_1.5s_infinite]"></div>
                        <i data-lucide="check-circle-2" class="w-5 h-5 submit-icon"></i> <span class="submit-text">KONFIRMASI AKSES</span>
                    </button>
                </form>
            </div>
        </div>

        <!-- ==================== VIEW: ADMIN DASHBOARD ==================== -->
        <div id="view-admin" class="space-y-8 hidden-view transition-opacity duration-500">
            <!-- Premium Dashboard Header -->
            <div class="flex flex-col xl:flex-row gap-6 justify-between items-start xl:items-center">
                <div>
                    <h2 class="text-3xl font-black text-white tracking-tight flex items-center gap-3">
                        System Command Center
                        <span class="flex items-center gap-2 text-xs px-3 py-1 rounded-full bg-emerald-500/10 border border-emerald-500/20 text-emerald-400 tracking-widest">
                            <span class="w-2 h-2 rounded-full bg-emerald-500 animate-pulse"></span> ONLINE
                        </span>
                    </h2>
                    <p class="text-slate-400 mt-2 flex items-center gap-2">
                        <i data-lucide="wifi" class="w-3.5 h-3.5"></i> Sinkronisasi Cloud: Google Sheets Database Aktif
                    </p>
                </div>
                
                <div class="flex flex-wrap items-center gap-3 bg-slate-900/50 p-2 rounded-2xl border border-slate-800 backdrop-blur-xl">
                    <div class="flex p-1 bg-slate-950 rounded-xl" id="filter-container">
                        <!-- Filter buttons generated via JS -->
                    </div>
                    
                    <div class="w-[1px] h-8 bg-slate-800 mx-2 hidden sm:block"></div>

                    <div class="relative">
                        <i data-lucide="search" class="absolute left-3 top-1/2 -translate-y-1/2 text-slate-500 w-4 h-4"></i>
                        <input type="text" id="searchInput" placeholder="Cari nama..." onkeyup="handleSearch()" class="pl-9 pr-4 py-2 rounded-xl bg-slate-950 border border-slate-800 text-white focus:ring-2 focus:ring-indigo-500/50 outline-none w-40 sm:w-48 text-sm">
                    </div>

                    <button onclick="toggleQRModal(true)" class="flex items-center gap-2 bg-slate-800 hover:bg-slate-700 text-white px-5 py-2.5 rounded-xl font-bold text-sm transition-all border border-slate-700 hover:border-slate-600">
                        <i data-lucide="qr-code" class="text-indigo-400 w-4 h-4"></i> Cetak QR Akses
                    </button>
                </div>
            </div>

            <!-- Stats Overview -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="bg-slate-900/60 backdrop-blur-xl border border-slate-800 p-6 rounded-3xl flex items-center gap-6">
                    <div class="bg-indigo-500/10 p-4 rounded-2xl border border-indigo-500/20">
                        <i data-lucide="users" class="text-indigo-400 w-7 h-7"></i>
                    </div>
                    <div>
                        <p class="text-slate-400 text-xs font-bold uppercase tracking-widest mb-1">Total Pengguna Hari Ini</p>
                        <p class="text-3xl font-black text-white" id="stat-total">0</p>
                    </div>
                </div>
                <div class="bg-slate-900/60 backdrop-blur-xl border border-slate-800 p-6 rounded-3xl flex items-center gap-6">
                    <div class="bg-emerald-500/10 p-4 rounded-2xl border border-emerald-500/20">
                        <i data-lucide="monitor" class="text-emerald-400 w-7 h-7"></i>
                    </div>
                    <div>
                        <p class="text-slate-400 text-xs font-bold uppercase tracking-widest mb-1">Workstation Aktif</p>
                        <p class="text-3xl font-black text-white" id="stat-active">0</p>
                    </div>
                </div>
                <div class="bg-slate-900/60 backdrop-blur-xl border border-slate-800 p-6 rounded-3xl flex items-center gap-6 relative overflow-hidden">
                    <div class="absolute right-[-20%] top-[-20%] opacity-10">
                        <i data-lucide="cpu" class="w-32 h-32"></i>
                    </div>
                    <div class="bg-cyan-500/10 p-4 rounded-2xl border border-cyan-500/20">
                        <i data-lucide="activity" class="text-cyan-400 w-7 h-7"></i>
                    </div>
                    <div>
                        <p class="text-slate-400 text-xs font-bold uppercase tracking-widest mb-1">Efisiensi Jaringan</p>
                        <p class="text-3xl font-black text-white">99.9%</p>
                    </div>
                </div>
            </div>
            
            <!-- Premium Grid Cards Container -->
            <div id="visitors-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6">
                <!-- Data akan di-render di sini oleh JavaScript -->
            </div>

            <!-- Empty State -->
            <div id="empty-state" class="hidden-view bg-slate-900/40 border border-slate-800 rounded-3xl p-20 text-center">
                <i data-lucide="search" class="mx-auto text-slate-600 mb-6 w-16 h-16"></i>
                <h3 class="text-xl font-bold text-slate-300 mb-2">Tidak Ada Aktivitas</h3>
                <p class="text-slate-500">Belum ada pengguna yang sesuai dengan filter.</p>
            </div>
        </div>
    </main>

    <!-- Premium QR Modal -->
    <div id="qr-modal" class="hidden-view fixed inset-0 z-[100] flex items-center justify-center bg-slate-950/80 backdrop-blur-xl p-4 transition-opacity duration-300 opacity-0">
        <div class="bg-slate-900 border border-slate-800 rounded-[2.5rem] p-8 sm:p-12 max-w-5xl w-full relative shadow-2xl shadow-indigo-500/10 transform scale-95 transition-transform duration-300" id="qr-modal-content">
            <button onclick="toggleQRModal(false)" class="absolute top-6 right-6 p-3 bg-slate-800 hover:bg-slate-700 text-slate-400 hover:text-white rounded-full transition-colors">
                <i data-lucide="x" class="w-6 h-6"></i>
            </button>
            
            <div class="text-center mb-12">
                <h3 class="text-3xl font-black text-white tracking-tight">Access Node QR</h3>
                <p class="text-slate-400 mt-2">Cetak dan posisikan pada pintu masuk masing-masing sektor lab.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8" id="qr-container">
                <!-- QR Codes generated by JS -->
            </div>
        </div>
    </div>

    <!-- Script Logika Aplikasi -->
    <script>
        // --- KONFIGURASI ---
        // URL GAS TERBARU TELAH DIMASUKKAN DI SINI
        const GAS_URL = "https://script.google.com/macros/s/AKfycbwwx9MZl-HJiOyp_mZ4L1qsieeWoFU491bp8UEl8UwcPpykQBohHSdU_D3Jtef2sDwRig/exec";
        
        const labsConfig = [
            { id: "Lab 1", icon: "monitor", colorClass: "from-blue-500 to-cyan-400", shadowClass: "shadow-cyan-500/20" },
            { id: "Lab 2", icon: "cpu", colorClass: "from-indigo-500 to-purple-500", shadowClass: "shadow-indigo-500/20" },
            { id: "Lab 3", icon: "activity", colorClass: "from-orange-500 to-pink-500", shadowClass: "shadow-orange-500/20" }
        ];

        // --- STATE ---
        let currentView = 'check-in';
        let activeLabFilter = 'Semua';
        let searchTerm = '';
        let isSubmitting = false;
        
        // Data Dummy (Bisa ditambah/dikurang sesuai kebutuhan)
        let visitors = [
            { id: 1, name: "Ahmad Fauzi", class: "XII RPL 1", purpose: "Praktikum Mandiri", date: new Date().toISOString().split('T')[0], time: "08:15", status: "Aktif", computerNo: "05", labId: "Lab 1" },
            { id: 2, name: "Siti Aminah", class: "XI TKJ 2", purpose: "Tugas Mapel", date: new Date().toISOString().split('T')[0], time: "09:30", status: "Aktif", computerNo: "12", labId: "Lab 2" },
        ];

        // --- INISIALISASI AWAL ---
        document.addEventListener('DOMContentLoaded', () => {
            // Cek parameter URL dari hasil scan QR Code
            const urlParams = new URLSearchParams(window.location.search);
            const labFromUrl = urlParams.get('lab');
            
            // Jika link diakses dari QR code dan membawa parameter yang valid, atur lab otomatis
            if (labFromUrl && labsConfig.some(l => l.id === labFromUrl)) {
                document.getElementById('labId').value = labFromUrl;
            }

            renderLabSelection();
            renderFilters();
            renderQRModal();
            updateDashboard();
            lucide.createIcons();
        });

        // --- NAVIGASI ---
        function switchView(viewName) {
            currentView = viewName;
            
            const btnCheckIn = document.getElementById('nav-check-in');
            const btnAdmin = document.getElementById('nav-admin');
            const viewCheckIn = document.getElementById('view-check-in');
            const viewAdmin = document.getElementById('view-admin');

            // Reset Styles
            btnCheckIn.className = "nav-btn px-5 py-2.5 rounded-xl text-sm font-semibold transition-all flex items-center gap-2 text-slate-400 hover:text-slate-200 hover:bg-slate-800 border border-transparent";
            btnAdmin.className = "nav-btn px-5 py-2.5 rounded-xl text-sm font-semibold transition-all flex items-center gap-2 text-slate-400 hover:text-slate-200 hover:bg-slate-800 border border-transparent";
            
            viewCheckIn.classList.add('hidden-view');
            viewAdmin.classList.add('hidden-view');

            // Apply Active Styles
            if(viewName === 'check-in') {
                btnCheckIn.className = "nav-btn px-5 py-2.5 rounded-xl text-sm font-semibold transition-all flex items-center gap-2 bg-indigo-600/20 text-indigo-400 shadow-[inset_0_1px_1px_rgba(255,255,255,0.1)] border border-indigo-500/30";
                viewCheckIn.classList.remove('hidden-view');
            } else {
                btnAdmin.className = "nav-btn px-5 py-2.5 rounded-xl text-sm font-semibold transition-all flex items-center gap-2 bg-indigo-600/20 text-indigo-400 shadow-[inset_0_1px_1px_rgba(255,255,255,0.1)] border border-indigo-500/30";
                viewAdmin.classList.remove('hidden-view');
                updateDashboard();
            }
        }

        // --- RENDER COMPONENT: LAB SELECTION (FORM) ---
        function renderLabSelection() {
            const container = document.getElementById('lab-selection');
            const labInput = document.getElementById('labId');
            container.innerHTML = '';

            labsConfig.forEach(lab => {
                const isSelected = labInput.value === lab.id;
                const baseClasses = "relative overflow-hidden group p-5 rounded-2xl border transition-all duration-300 w-full text-left";
                const activeClasses = `bg-slate-800 border-slate-600 ${lab.shadowClass}`;
                const inactiveClasses = "bg-slate-900/50 border-slate-800 hover:border-slate-700";
                
                const btn = document.createElement('button');
                btn.type = 'button';
                btn.className = `${baseClasses} ${isSelected ? activeClasses : inactiveClasses}`;
                btn.onclick = () => {
                    labInput.value = lab.id;
                    renderLabSelection(); // Re-render to update UI
                };

                let bgGradientHTML = isSelected ? `<div class="absolute inset-0 bg-gradient-to-br ${lab.colorClass} opacity-10"></div>` : '';
                let textClass = isSelected ? 'text-white' : 'text-slate-500 group-hover:text-slate-300';

                btn.innerHTML = `
                    ${bgGradientHTML}
                    <div class="flex items-center gap-3 relative z-10 ${textClass}">
                        <i data-lucide="${lab.icon}" class="w-4 h-4"></i>
                        <span class="font-bold tracking-wide">${lab.id}</span>
                    </div>
                `;
                container.appendChild(btn);
            });
            lucide.createIcons();
        }

        // --- SUBMIT DATA (FETCH KE GAS) ---
        async function handleFormSubmit(event) {
            event.preventDefault();
            if(isSubmitting) return;

            const form = event.target;
            const submitBtn = document.getElementById('submitBtn');
            const submitIcon = submitBtn.querySelector('.submit-icon');
            const submitText = submitBtn.querySelector('.submit-text');

            // Set Loading State
            isSubmitting = true;
            submitBtn.classList.add('bg-slate-800', 'text-slate-500', 'cursor-not-allowed');
            submitBtn.classList.remove('bg-white', 'text-slate-900', 'hover:bg-slate-100');
            submitIcon.setAttribute('data-lucide', 'loader-2');
            submitIcon.classList.add('animate-spin');
            submitText.textContent = "MENYINKRONKAN DATA...";
            lucide.createIcons();

            // Kumpulkan Data
            const payload = {
                id: Date.now(),
                name: form.name.value,
                class: form.class.value,
                purpose: form.purpose.value,
                computerNo: form.computerNo.value,
                labId: form.labId.value,
                date: new Date().toISOString().split('T')[0],
                time: new Date().toLocaleTimeString('id-ID', { hour: '2-digit', minute: '2-digit' })
            };

            try {
                // Kirim ke Google Apps Script
                await fetch(GAS_URL, {
                    method: 'POST',
                    mode: 'no-cors',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });

                // Jika berhasil, tambahkan ke data lokal
                payload.status = "Aktif";
                visitors.unshift(payload);
                showSuccessSequence();

            } catch (error) {
                console.error("Gagal mengirim ke Cloud:", error);
                // Fallback Simpan Lokal
                payload.status = "Lokal Only";
                visitors.unshift(payload);
                showSuccessSequence();
            } finally {
                // Reset Button State
                isSubmitting = false;
                submitBtn.classList.remove('bg-slate-800', 'text-slate-500', 'cursor-not-allowed');
                submitBtn.classList.add('bg-white', 'text-slate-900', 'hover:bg-slate-100');
                submitIcon.setAttribute('data-lucide', 'check-circle-2');
                submitIcon.classList.remove('animate-spin');
                submitText.textContent = "KONFIRMASI AKSES";
                lucide.createIcons();
                
                // Form di-reset tapi kembalikan lab yang sedang diakses dari URL jika ada
                form.reset();
                const urlParams = new URLSearchParams(window.location.search);
                const labFromUrl = urlParams.get('lab');
                document.getElementById('labId').value = (labFromUrl && labsConfig.some(l => l.id === labFromUrl)) ? labFromUrl : "Lab 1";
                renderLabSelection();
            }
        }

        function showSuccessSequence() {
            document.getElementById('form-container').classList.add('hidden-view');
            document.getElementById('success-message').classList.remove('hidden-view');
            
            setTimeout(() => {
                document.getElementById('success-message').classList.add('hidden-view');
                document.getElementById('form-container').classList.remove('hidden-view');
                switchView('admin');
            }, 3000);
        }

        // --- DASHBOARD & FILTERING ---
        function setFilter(filterVal) {
            activeLabFilter = filterVal;
            renderFilters();
            updateDashboard();
        }

        function handleSearch() {
            searchTerm = document.getElementById('searchInput').value.toLowerCase();
            updateDashboard();
        }

        function renderFilters() {
            const container = document.getElementById('filter-container');
            container.innerHTML = '';
            
            const filters = ['Semua', ...labsConfig.map(l => l.id)];
            filters.forEach(filter => {
                const isActive = activeLabFilter === filter;
                const activeClass = isActive ? 'bg-indigo-600 text-white shadow-lg shadow-indigo-600/20' : 'text-slate-500 hover:text-slate-300';
                
                const btn = document.createElement('button');
                btn.className = `px-4 py-2 rounded-lg text-sm font-bold transition-all ${activeClass}`;
                btn.textContent = filter;
                btn.onclick = () => setFilter(filter);
                container.appendChild(btn);
            });
        }

        function updateDashboard() {
            // Filter Data
            const filteredVisitors = visitors.filter(v => {
                const matchesSearch = v.name.toLowerCase().includes(searchTerm) || v.class.toLowerCase().includes(searchTerm);
                const matchesLab = activeLabFilter === 'Semua' || v.labId === activeLabFilter;
                return matchesSearch && matchesLab;
            });

            // Update Stats
            document.getElementById('stat-total').textContent = visitors.length;
            document.getElementById('stat-active').textContent = visitors.filter(v => v.status === "Aktif").length;

            // Render Grid
            const grid = document.getElementById('visitors-grid');
            const emptyState = document.getElementById('empty-state');
            grid.innerHTML = '';

            if(filteredVisitors.length === 0) {
                grid.classList.add('hidden-view');
                emptyState.classList.remove('hidden-view');
            } else {
                grid.classList.remove('hidden-view');
                emptyState.classList.add('hidden-view');

                filteredVisitors.forEach(v => {
                    const labConfig = labsConfig.find(l => l.id === v.labId);
                    const colorClass = labConfig ? labConfig.colorClass : 'from-slate-500 to-slate-400';
                    const iconName = labConfig ? labConfig.icon : 'monitor';
                    
                    const cardHTML = `
                        <div class="group bg-slate-900/40 hover:bg-slate-900/80 backdrop-blur-md border border-slate-800 hover:border-slate-700 p-6 rounded-3xl transition-all duration-300 relative overflow-hidden flex flex-col">
                            <div class="absolute top-0 left-0 right-0 h-1 bg-gradient-to-r ${colorClass} opacity-50 group-hover:opacity-100 transition-opacity"></div>
                            
                            <div class="flex justify-between items-start mb-6">
                                <span class="px-3 py-1 rounded-lg text-xs font-black uppercase tracking-widest bg-slate-950 border border-slate-800 text-slate-300 flex items-center gap-2">
                                    <i data-lucide="${iconName}" class="w-3.5 h-3.5"></i> ${v.labId}
                                </span>
                                <span class="flex items-center gap-1.5 text-xs font-medium bg-emerald-500/10 text-emerald-400 px-2.5 py-1 rounded-md border border-emerald-500/20">
                                    <span class="w-1.5 h-1.5 rounded-full bg-emerald-400 animate-pulse"></span> ${v.status}
                                </span>
                            </div>
                            
                            <div class="flex-grow">
                                <h4 class="font-black text-xl text-white mb-1 group-hover:text-indigo-300 transition-colors">${v.name}</h4>
                                <p class="text-slate-400 text-sm flex items-center gap-2 mb-4">
                                    <i data-lucide="book-open" class="w-3.5 h-3.5"></i> ${v.class}
                                </p>
                            </div>

                            <div class="bg-slate-950/50 p-4 rounded-2xl border border-slate-800/50 mt-4">
                                <div class="flex justify-between items-center mb-3">
                                    <p class="text-[10px] text-slate-500 font-bold uppercase tracking-widest">Workstation</p>
                                    <p class="font-mono font-bold text-cyan-400 text-sm border border-cyan-500/30 bg-cyan-500/10 px-2 py-0.5 rounded">PC-${v.computerNo}</p>
                                </div>
                                <div class="flex justify-between items-center">
                                    <p class="text-xs text-slate-400 truncate pr-2" title="${v.purpose}">${v.purpose}</p>
                                    <div class="text-right whitespace-nowrap">
                                        <p class="text-sm font-bold text-white flex items-center gap-1 justify-end">
                                            <i data-lucide="clock" class="text-indigo-400 w-3 h-3"></i> ${v.time}
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    `;
                    grid.insertAdjacentHTML('beforeend', cardHTML);
                });
                // Re-initialize icons inside the new HTML
                lucide.createIcons();
            }
        }

        // --- QR MODAL ---
        function toggleQRModal(show) {
            const modal = document.getElementById('qr-modal');
            const modalContent = document.getElementById('qr-modal-content');
            
            if(show) {
                modal.classList.remove('hidden-view');
                // Trigger reflow for animation
                void modal.offsetWidth;
                modal.classList.remove('opacity-0');
                modalContent.classList.remove('scale-95');
                modalContent.classList.add('scale-100');
            } else {
                modal.classList.add('opacity-0');
                modalContent.classList.remove('scale-100');
                modalContent.classList.add('scale-95');
                setTimeout(() => {
                    modal.classList.add('hidden-view');
                }, 300); // Wait for transition
            }
        }

        function renderQRModal() {
            const container = document.getElementById('qr-container');
            const baseUrl = window.location.href.split('?')[0]; // Ambil URL saat ini tanpa parameter
            
            labsConfig.forEach(lab => {
                const qrUrl = `https://api.qrserver.com/v1/create-qr-code/?size=300x300&data=${encodeURIComponent(baseUrl + "?lab=" + lab.id)}`;
                
                const html = `
                    <div class="bg-slate-950 border border-slate-800 p-8 rounded-3xl text-center group hover:border-slate-600 transition-colors flex flex-col items-center">
                        <div class="w-16 h-16 rounded-2xl bg-gradient-to-br ${lab.colorClass} flex items-center justify-center text-white mb-6 shadow-lg">
                            <i data-lucide="${lab.icon}" class="w-8 h-8"></i>
                        </div>
                        <h4 class="font-black text-white tracking-widest text-lg mb-6">${lab.id}</h4>
                        
                        <div class="bg-white p-3 rounded-2xl mb-6 inline-block">
                            <img src="${qrUrl}" alt="${lab.id}" class="w-48 h-48" />
                        </div>
                        
                        <button onclick="window.print()" class="w-full mt-auto flex items-center justify-center gap-2 bg-slate-800 hover:bg-indigo-600 text-white py-3.5 rounded-xl font-bold transition-colors border border-slate-700 hover:border-indigo-500">
                            <i data-lucide="printer" class="w-4 h-4"></i> Cetak Label
                        </button>
                    </div>
                `;
                container.insertAdjacentHTML('beforeend', html);
            });
        }
    </script>
</body>
</html>
