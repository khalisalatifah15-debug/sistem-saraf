<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sistem Saraf - Kelompok 5</title>
    <style>
        :root {
            --bg-color: #8A9A40;
            --card-bg: #EAE6DF;
            --text-color: #2D311A;
            --accent-color: #5C6926;
            --header-bg: #798835;
            --white: #FFFFFF;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            padding: 30px 15px;
            line-height: 1.6;
        }

        .container {
            max-width: 850px;
            margin: 0 auto;
        }

        .header-card {
            background-color: var(--card-bg);
            border-radius: 12px;
            padding: 25px;
            text-align: center;
            margin-bottom: 25px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.15);
        }

        .header-card h1 {
            color: var(--accent-color);
            font-size: 2.2rem;
            margin-bottom: 10px;
        }

        .author-box {
            background-color: var(--header-bg);
            color: white;
            padding: 12px;
            border-radius: 8px;
            font-size: 0.95rem;
        }

        /* Styling Accordion / Klik Judul */
        .accordion-item {
            background-color: var(--card-bg);
            border-radius: 10px;
            margin-bottom: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            overflow: hidden;
        }

        .accordion-header {
            background-color: var(--card-bg);
            color: var(--accent-color);
            padding: 18px 25px;
            font-size: 1.25rem;
            font-weight: bold;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: background-color 0.3s ease;
            user-select: none;
        }

        .accordion-header:hover {
            background-color: #dfd9ce;
        }

        .accordion-header::after {
            content: '▼';
            font-size: 0.9rem;
            transition: transform 0.3s ease;
            color: var(--accent-color);
        }

        .accordion-item.active .accordion-header::after {
            transform: rotate(180deg);
        }

        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease-out, padding 0.3s ease;
            padding: 0 25px;
            background-color: #f7f5f0;
            border-top: 1px solid #ddd;
        }

        .accordion-item.active .accordion-content {
            padding: 20px 25px;
            max-height: 2000px; /* Cukup besar agar seluruh materi muat saat terbuka */
        }

        h3 {
            color: var(--accent-color);
            margin: 15px 0 8px;
        }

        ul, ol {
            margin-left: 20px;
            margin-bottom: 15px;
        }

        p, li {
            margin-bottom: 8px;
            font-size: 1.05rem;
        }

        .img-container {
            text-align: center;
            margin: 20px 0;
        }

        .img-container img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            box-shadow: 0 3px 8px rgba(0,0,0,0.15);
        }

        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-top: 10px;
        }

        .link-3d {
            display: inline-block;
            background-color: var(--accent-color);
            color: white;
            padding: 8px 16px;
            text-decoration: none;
            border-radius: 6px;
            margin-top: 10px;
            font-weight: bold;
        }

        @media (max-width: 600px) {
            .grid-2 { grid-template-columns: 1fr; }
            .accordion-header { font-size: 1.1rem; padding: 15px; }
        }
    </style>
</head>
<body>

<div class="container">

    <!-- Header Judul Utama -->
    <div class="header-card">
        <h1>Sistem Saraf</h1>
        <div class="author-box">
            <p><strong>Kelompok 5:</strong> Mia Nurhalimah (242154111055) | Khalisa Latifah (242154111057) | Lina Agustin (242154111059)</p>
        </div>
        <p style="margin-top: 10px; font-size: 0.9rem; color: #555;"><i>Klik pada salah satu judul materi di bawah untuk membuka penjelasan dan gambar.</i></p>
    </div>

    <!-- Materi 1 -->
    <div class="accordion-item">
        <div class="accordion-header">1. Sel Saraf (Neuron) & Anatomi</div>
        <div class="accordion-content">
            <p>Neuron adalah sel utama dalam sistem saraf yang berfungsi sebagai unit fungsional dasar untuk menerima, memproses, dan menghantarkan informasi dalam bentuk impuls listrik dan sinyal kimia.</p>
            
            <div class="img-container">
                <img src="neuron.png" alt="Anatomi Neuron" onerror="this.src='https://via.placeholder.com/600x300?text=Gambar+Anatomi+Neuron'">
            </div>

            <h3>Struktur Anatomi Neuron:</h3>
            <ul>
                <li><strong>Badan sel (soma):</strong> Pusat metabolik neuron, tidak memiliki sentriol.</li>
                <li><strong>Dendrit:</strong> Menerima sinyal/rangsangan dari neuron lain menuju badan sel & menentukan kekuatan sinyal.</li>
                <li><strong>Akson:</strong> Serabut panjang yang mengirimkan impuls saraf dari badan sel menuju neuron/otot target.</li>
                <li><strong>Selubung Mielin:</strong> Selaput lemak berbentuk lilin untuk memastikan sinyal listrik berjalan sesuai jalur.</li>
            </ul>
            <a href="https://skfb.ly/oPDwP" target="_blank" class="link-3d">🌐 Buka Anatomi Neuron (3D Interactive)</a>
        </div>
    </div>

    <!-- Materi 2 -->
    <div class="accordion-item">
        <div class="accordion-header">2. Klasifikasi Neuron</div>
        <div class="accordion-content">
            <p>Berdasarkan fungsinya, neuron diklasifikasikan menjadi:</p>
            <ul>
                <li><strong>Neuron Sensorik:</strong> Membawa informasi dari reseptor indra menuju sistem saraf pusat.</li>
                <li><strong>Neuron Motorik:</strong> Mengirimkan perintah dari sistem saraf pusat menuju otot atau kelenjar.</li>
                <li><strong>Interneuron:</strong> Penghubung antara neuron sensorik dan motorik di dalam sistem saraf pusat untuk mengintegrasikan informasi (berpikir, belajar, dan keputusan).</li>
            </ul>
            <div class="img-container">
                <img src="jenis-neuron.png" alt="Klasifikasi Neuron" onerror="this.style.display='none'">
            </div>
        </div>
    </div>

    <!-- Materi 3 -->
    <div class="accordion-item">
        <div class="accordion-header">3. Fisiologi Potensial Membran & Aksi</div>
        <div class="accordion-content">
            <div class="img-container">
                <img src="potensial.png" alt="Grafik Potensial Aksi" onerror="this.src='https://via.placeholder.com/600x300?text=Grafik+Potensial+Membran'">
            </div>
            <h3>Potensial Istirahat (-70 mV)</h3>
            <p>Bagian dalam neuron bermuatan lebih negatif dibanding luar. Dipertahankan oleh kerja pompa Na⁺/K⁺ dengan energi ATP.</p>
            
            <h3>Tahapan Potensial Aksi:</h3>
            <ul>
                <li><strong>Depolarisasi:</strong> Kanal Na⁺ terbuka, ion Na⁺ masuk, muatan sel jadi positif & memicu impuls.</li>
                <li><strong>Repolarisasi:</strong> Kanal Na⁺ tutup & kanal K⁺ terbuka, ion K⁺ keluar, muatan kembali negatif.</li>
                <li><strong>Hiperpolarisasi:</strong> Penurunan muatan sesaat melebihi batas istirahat sebelum stabil.</li>
                <li><strong>Konduksi Saltatori:</strong> Impuls "melompat" antar Nodus Ranvier mempercepat transmisi sinyal.</li>
            </ul>
        </div>
    </div>

    <!-- Materi 4 -->
    <div class="accordion-item">
        <div class="accordion-header">4. Transmisi Sinapsis Kimia & Neurotransmitter</div>
        <div class="accordion-content">
            <p>Sinapsis adalah titik pertemuan fungsional antar neuron yang dipisahkan oleh celah sinaptik (synaptic cleft).</p>
            
            <div class="img-container">
                <img src="sinapsis.png" alt="Mekanisme Sinapsis" onerror="this.src='https://via.placeholder.com/600x300?text=Mekanisme+Transmisi+Sinapsis'">
            </div>

            <h3>Mekanisme Kerja Sinapsis:</h3>
            <ol>
                <li>Impuls sampai di terminal akson → Kanal Ca²⁺ terbuka.</li>
                <li>Ion Ca²⁺ memicu pelepasan Neurotransmitter ke celah sinaptik secara eksositosis.</li>
                <li>Neurotransmitter berikatan dengan reseptor di membran postsinaptik.</li>
            </ol>
            
            <h3>Peran Neurotransmitter:</h3>
            <p>Zat kimia pembawa pesan (seperti Asetilkolin, Dopamin, Serotonin). Setelah bekerja, neurotransmitter diuraikan enzim atau diserap kembali (reuptake) agar tidak terjadi stimulasi berlebihan.</p>
        </div>
    </div>

    <!-- Materi 5 -->
    <div class="accordion-item">
        <div class="accordion-header">5. Otak Besar (Serebrum) & Lobus</div>
        <div class="accordion-content">
            <p>Porsi terbesar otak (2/3 berat total), terbagi menjadi 2 hemisfer (kanan & kiri) yang bersifat kontralateral. Memiliki lipatan Gyrus (tonjolan) dan Sulcus (celah).</p>
            
            <div class="img-container">
                <img src="otak.png" alt="Lobus Otak" onerror="this.src='https://via.placeholder.com/600x300?text=Lobus-Lobus+Korteks+Serebral'">
            </div>

            <h3>Pembagian Lobus Korteks Serebral:</h3>
            <ul>
                <li><strong>Lobus Frontalis:</strong> Kendali motorik, bicara, emosi, penalaran, & perencanaan.</li>
                <li><strong>Lobus Parietalis:</strong> Pemrosesan sensorik (sentuhan, tekanan, nyeri, spasial).</li>
                <li><strong>Lobus Oksipitalis:</strong> Pusat pemrosesan visual (penglihatan).</li>
                <li><strong>Lobus Temporalis:</strong> Pusat pendengaran, memori, & pemahaman bahasa.</li>
            </ul>
        </div>
    </div>

    <!-- Materi 6 -->
    <div class="accordion-item">
        <div class="accordion-header">6. Otak Kecil, Batang Otak & Diensefalon</div>
        <div class="accordion-content">
            <h3>Otak Kecil (Serebelum)</h3>
            <p>Menyelaraskan & mengkoordinasikan gerakan tubuh (terbagi atas Lobus Anterior, Posterior, & Flocculonodularis).</p>
            
            <h3>Batang Otak (Brainstem)</h3>
            <ul>
                <li><strong>Mesensefalon:</strong> Refleks penglihatan & pendengaran.</li>
                <li><strong>Pons:</strong> Jembatan saraf & pengatur irama pernapasan.</li>
                <li><strong>Medulla Oblongata:</strong> Pusat refleks otonom vital (denyut jantung, pernapasan, batuk).</li>
            </ul>

            <h3>Diensefalon (Otak Antara)</h3>
            <div class="grid-2">
                <div style="background:#fff; padding:10px; border-radius:6px;"><strong>Talamus:</strong> Stasiun pemancar sinyal sensorik.</div>
                <div style="background:#fff; padding:10px; border-radius:6px;"><strong>Hipotalamus:</strong> Pusat homeostasis & suhu.</div>
                <div style="background:#fff; padding:10px; border-radius:6px;"><strong>Epitalamus:</strong> Kelenjar pineal (melatonin).</div>
                <div style="background:#fff; padding:10px; border-radius:6px;"><strong>Subtalamus:</strong> Pemulusan gerakan motorik.</div>
            </div>
        </div>
    </div>

    <!-- Materi 7 -->
    <div class="accordion-item">
        <div class="accordion-header">7. Sumsum Tulang Belakang & Lengkung Refleks</div>
        <div class="accordion-content">
            <p>Lanjutan medulla oblongata yang dilindungi meninges & cairan serebrospinal. Berfungsi sebagai jalur Asenden (sensorik ke otak) dan Desenden (motorik ke otot).</p>

            <h3>Jalur Lengkung Refleks:</h3>
            <ul>
                <li><strong>Refleks Spinal:</strong> Diproses langsung di Medula Spinalis. <br><i>Alur: Reseptor → Neuron Sensorik → Sumsum Tulang Belakang → Neuron Motorik → Efektor.</i></li>
                <li><strong>Refleks Kranial:</strong> Diproses di Batang Otak (12 pasang saraf kranial), contoh: refleks pupil mata menyempit saat terkena cahaya terang.</li>
            </ul>
        </div>
    </div>

    <!-- Materi 8 -->
    <div class="accordion-item">
        <div class="accordion-header">8. Perbedaan Sistem Saraf Simpatis & Parasimpatis</div>
        <div class="accordion-content">
            <h3>1. Simpatis (Fight or Flight)</h3>
            <p>Bekerja saat stres/darurat: Pupil membesar, denyut jantung & pernapasan meningkat, kerja pencernaan melambat.</p>
            
            <h3>2. Parasimpatis (Rest and Digest)</h3>
            <p>Bekerja saat tenang/istirahat: Denyut jantung & nafas melambat, mengaktifkan kembali fungsi saluran pencernaan.</p>
        </div>
    </div>

    <!-- Materi 9 -->
    <div class="accordion-item">
        <div class="accordion-header">9. Kelainan & Penyakit Sistem Saraf</div>
        <div class="accordion-content">
            <ul>
                <li><strong>Stroke:</strong> Gangguan pasokan darah ke otak akibat penyumbatan (Iskemik) atau pecah pembuluh darah (Hemoragik).</li>
                <li><strong>Multiple Sclerosis (MS):</strong> Penyakit autoimun yang merusak selubung mielin.</li>
                <li><strong>Bell's Palsy:</strong> Kelumpuhan mendadak otot satu sisi wajah akibat peradangan Nervus VII.</li>
                <li><strong>Penyakit Parkinson:</strong> Degenerasi sel saraf penghasil dopamin yang memicu tremor dan kekakuan gerak.</li>
            </ul>
        </div>
    </div>

</div>

<script>
    // Fitur Klik Accordion (Buka / Tutup Judul)
    const accordionHeaders = document.querySelectorAll('.accordion-header');

    accordionHeaders.forEach(header => {
        header.addEventListener('click', () => {
            const accordionItem = header.parentElement;
            
            // Tutup item lain jika ingin hanya 1 materi yang terbuka (opsional)
            document.querySelectorAll('.accordion-item').forEach(item => {
                if (item !== accordionItem) {
                    item.classList.remove('active');
                }
            });

            // Toggle item yang diklik
            accordionItem.classList.toggle('active');
        });
    });
</script>

</body>
</html>
