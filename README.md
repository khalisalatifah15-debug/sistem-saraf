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
            max-height: 3000px;
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
            background: #fff;
            padding: 10px;
            border-radius: 8px;
            border: 1px solid #ddd;
        }

        .img-container img {
            max-width: 100%;
            height: auto;
            border-radius: 6px;
        }

        .img-caption {
            font-size: 0.85rem;
            color: #666;
            margin-top: 5px;
            font-style: italic;
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

    <div class="header-card">
        <h1>Sistem Saraf</h1>
        <div class="author-box">
            <p><strong>Kelompok 5:</strong> Mia Nurhalimah (242154111055) | Khalisa Latifah (242154111057) | Lina Agustin (242154111059)</p>
        </div>
        <p style="margin-top: 10px; font-size: 0.9rem; color: #555;"><i>Klik pada salah satu judul materi untuk menampilkan penjelasannya beserta gambar.</i></p>
    </div>

    <!-- 1. Sel Saraf (Neuron) -->
    <div class="accordion-item">
        <div class="accordion-header">1. Sel Saraf (Neuron) & Anatomi</div>
        <div class="accordion-content">
            <p>Neuron adalah sel utama dalam sistem saraf yang berfungsi sebagai unit fungsional dasar untuk menerima, memproses, dan menghantarkan informasi dalam bentuk impuls listrik dan sinyal kimia.</p>
            
            <div class="img-container">
                <img src="neuron.png" alt="Anatomi Neuron">
                <div class="img-caption">Gambar 1: Struktur Anatomi Sel Saraf (Neuron)</div>
            </div>

            <h3>Struktur Anatomi Neuron:</h3>
            <ul>
                <li><strong>Badan sel (soma):</strong> Pusat metabolik neuron, tidak memiliki sentriol.</li>
                <li><strong>Dendrit:</strong> Menerima sinyal/rangsangan dari neuron lain menuju badan sel.</li>
                <li><strong>Akson:</strong> Serabut panjang yang mengirimkan impuls saraf dari badan sel menuju sel target.</li>
                <li><strong>Selubung Mielin:</strong> Selaput lemak pembungkus akson untuk mempercepat hantaran impuls.</li>
            </ul>
            <a href="https://skfb.ly/oPDwP" target="_blank" class="link-3d">🌐 Buka Model 3D Anatomi Neuron</a>
        </div>
    </div>

    <!-- 2. Klasifikasi Neuron -->
    <div class="accordion-item">
        <div class="accordion-header">2. Klasifikasi Neuron</div>
        <div class="accordion-content">
            <p>Berdasarkan fungsinya, neuron diklasifikasikan menjadi tiga jenis utama:</p>
            
            <div class="img-container">
                <img src="jenis-neuron.png" alt="Klasifikasi Neuron">
                <div class="img-caption">Gambar 2: Jenis-Jenis Neuron Berdasarkan Fungsi & Struktur</div>
            </div>

            <ul>
                <li><strong>Neuron Sensorik:</strong> Membawa informasi dari reseptor indra menuju sistem saraf pusat.</li>
                <li><strong>Neuron Motorik:</strong> Mengirimkan perintah dari sistem saraf pusat menuju otot atau kelenjar.</li>
                <li><strong>Interneuron:</strong> Penghubung neuron sensorik dan motorik di sistem saraf pusat untuk mengintegrasikan informasi.</li>
            </ul>
        </div>
    </div>

    <!-- 3. Potensial Membran & Aksi -->
    <div class="accordion-item">
        <div class="accordion-header">3. Fisiologi Potensial Membran & Aksi</div>
        <div class="accordion-content">
            <div class="img-container">
                <img src="potensial.png" alt="Grafik Potensial Aksi">
                <div class="img-caption">Gambar 3: Grafik Tahapan Potensial Aksi dan Membran Istirahat</div>
            </div>

            <h3>Potensial Istirahat (-70 mV)</h3>
            <p>Bagian dalam neuron bermuatan lebih negatif dibanding luar. Dipertahankan oleh pompa Na⁺/K⁺ dengan ATP.</p>
            
            <h3>Tahapan Potensial Aksi:</h3>
            <ul>
                <li><strong>Depolarisasi:</strong> Kanal Na⁺ terbuka, ion Na⁺ masuk, muatan sel menjadi positif.</li>
                <li><strong>Repolarisasi:</strong> Kanal Na⁺ tutup & kanal K⁺ terbuka, ion K⁺ keluar, muatan kembali negatif.</li>
                <li><strong>Hiperpolarisasi:</strong> Penurunan muatan sesaat melebihi batas istirahat.</li>
                <li><strong>Konduksi Saltatori:</strong> Impuls "melompat" antar Nodus Ranvier mempercepat transmisi sinyal.</li>
            </ul>
        </div>
    </div>

    <!-- 4. Sinapsis Kimia & Neurotransmitter -->
    <div class="accordion-item">
        <div class="accordion-header">4. Transmisi Sinapsis Kimia & Neurotransmitter</div>
        <div class="accordion-content">
            <p>Sinapsis adalah titik pertemuan fungsional antar neuron yang dipisahkan oleh celah sinaptik (synaptic cleft).</p>
            
            <div class="img-container">
                <img src="sinapsis.png" alt="Mekanisme Sinapsis">
                <div class="img-caption">Gambar 4: Mekanisme Pelepasan Neurotransmitter pada Celah Sinaptik</div>
            </div>

            <h3>Mekanisme Kerja Sinapsis:</h3>
            <ol>
                <li>Impuls sampai di terminal akson → Kanal Ca²⁺ terbuka.</li>
                <li>Ion Ca²⁺ memicu pelepasan Neurotransmitter ke celah sinaptik secara eksositosis.</li>
                <li>Neurotransmitter berikatan dengan reseptor di membran postsinaptik.</li>
            </ol>
        </div>
    </div>

    <!-- 5. Serebrum & Lobus Otak -->
    <div class="accordion-item">
        <div class="accordion-header">5. Otak Besar (Serebrum) & Lobus</div>
        <div class="accordion-content">
            <p>Porsi terbesar otak (2/3 berat total), terbagi menjadi 2 hemisfer (kanan & kiri) yang bersifat kontralateral.</p>
            
            <div class="img-container">
                <img src="otak.png" alt="Lobus Otak">
                <div class="img-caption">Gambar 5: Pembagian Lobus Korteks Serebral</div>
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

    <!-- 6. Batang Otak & Diensefalon -->
    <div class="accordion-item">
        <div class="accordion-header">6. Otak Kecil, Batang Otak & Diensefalon</div>
        <div class="accordion-content">
            <div class="img-container">
                <img src="batang-otak.png" alt="Batang Otak">
                <div class="img-caption">Gambar 6: Bagian-Bagian Batang Otak dan Diensefalon</div>
            </div>

            <h3>Otak Kecil (Serebelum)</h3>
            <p>Menyelaraskan & mengkoordinasikan gerakan tubuh (Lobus Anterior, Posterior, & Flocculonodularis).</p>
            
            <h3>Batang Otak (Brainstem)</h3>
            <ul>
                <li><strong>Mesensefalon:</strong> Refleks penglihatan & pendengaran.</li>
                <li><strong>Pons:</strong> Pengatur irama pernapasan.</li>
                <li><strong>Medulla Oblongata:</strong> Pusat refleks otonom vital (denyut jantung, pernapasan, batuk).</li>
            </ul>
        </div>
    </div>

    <!-- 7. Sumsum Tulang Belakang & Refleks -->
    <div class="accordion-item">
        <div class="accordion-header">7. Sumsum Tulang Belakang & Lengkung Refleks</div>
        <div class="accordion-content">
            <div class="img-container">
                <img src="sumsum.png" alt="Penampang Sumsum Tulang Belakang">
                <div class="img-caption">Gambar 7: Penampang Melintang Sumsum Tulang Belakang</div>
            </div>

            <div class="img-container">
                <img src="refleks.png" alt="Jalur Lengkung Refleks">
                <div class="img-caption">Gambar 8: Jalur Lengkung Refleks Spinal dan Kranial</div>
            </div>

            <h3>Jalur Lengkung Refleks:</h3>
            <p><i>Alur: Reseptor → Neuron Sensorik → Sumsum Tulang Belakang / Batang Otak → Neuron Motorik → Efektor.</i></p>
        </div>
    </div>

    <!-- 8. Simpatis & Parasimpatis -->
    <div class="accordion-item">
        <div class="accordion-header">8. Perbedaan Sistem Saraf Simpatis & Parasimpatis</div>
        <div class="accordion-content">
            <div class="img-container">
                <img src="otonom.png" alt="Saraf Simpatis dan Parasimpatis">
                <div class="img-caption">Gambar 9: Perbandingan Respon Organ Saraf Simpatis vs Parasimpatis</div>
            </div>

            <h3>1. Simpatis (Fight or Flight)</h3>
            <p>Bekerja saat stres/darurat: Pupil membesar, denyut jantung meningkat, kerja pencernaan melambat.</p>
            
            <h3>2. Parasimpatis (Rest and Digest)</h3>
            <p>Bekerja saat tenang/istirahat: Denyut jantung & nafas melambat, mengaktifkan kembali pencernaan.</p>
        </div>
    </div>

</div>

<script>
    const accordionHeaders = document.querySelectorAll('.accordion-header');

    accordionHeaders.forEach(header => {
        header.addEventListener('click', () => {
            const accordionItem = header.parentElement;
            
            document.querySelectorAll('.accordion-item').forEach(item => {
                if (item !== accordionItem) {
                    item.classList.remove('active');
                }
            });

            accordionItem.classList.toggle('active');
        });
    });
</script>

</body>
</html>
