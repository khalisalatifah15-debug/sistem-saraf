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
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
        }

        .card {
            background-color: var(--card-bg);
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.15);
        }

        h1, h2, h3 {
            color: var(--accent-color);
            margin-bottom: 15px;
        }

        h1 {
            font-size: 2.2rem;
            text-align: center;
        }

        h2 {
            font-size: 1.6rem;
            border-bottom: 2px solid var(--accent-color);
            padding-bottom: 8px;
            margin-top: 10px;
        }

        p, li {
            font-size: 1.05rem;
            margin-bottom: 10px;
        }

        ul, ol {
            margin-left: 25px;
            margin-bottom: 15px;
        }

        .img-container {
            text-align: center;
            margin: 20px 0;
        }

        .img-container img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            border: 2px solid #ccc;
        }

        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        @media (max-width: 768px) {
            .grid-2 {
                grid-template-columns: 1fr;
            }
        }

        .author-box {
            background-color: #798835;
            color: white;
            padding: 15px;
            border-radius: 8px;
            margin-top: 20px;
        }

        .author-box h3 {
            color: white;
        }

        .link-3d {
            display: inline-block;
            background-color: var(--accent-color);
            color: white;
            padding: 8px 15px;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 10px;
        }

        .link-3d:hover {
            background-color: #434d1b;
        }
    </style>
</head>
<body>

<div class="container">

    <!-- Slide 1: Cover -->
    <div class="card" style="text-align: center;">
        <h1>Sistem Saraf</h1>
        <div class="author-box">
            <h3>Kelompok 5</h3>
            <p>Anggota:</p>
            <p>1. Mia Nurhalimah (242154111055)</p>
            <p>2. Khalisa Latifah (242154111057)</p>
            <p>3. Lina Agustin (242154111059)</p>
        </div>
    </div>

    <!-- Slide 2 & 3: Sel Saraf (Neuron) -->
    <div class="card">
        <h2>Sel Saraf (Neuron)</h2>
        <p>Neuron adalah sel utama dalam sistem saraf yang berfungsi sebagai unit fungsional dasar untuk menerima, memproses, dan menghantarkan informasi dalam bentuk impuls listrik dan sinyal kimia.</p>
        
        <div class="img-container">
            <!-- Ganti src dengan nama/tautan gambar neuron dari PDF -->
            <img src="neuron.png" alt="Anatomi Neuron">
        </div>

        <h3>Struktur Anatomi Neuron</h3>
        <p>Struktur anatomi neuron terdiri dari:</p>
        <ul>
            <li><strong>Badan sel (soma):</strong> Badan sel merupakan pusat metabolik dari neuron. Ciri khas badan sel neuron ini adalah tidak memiliki sentriol.</li>
            <li><strong>Dendrit:</strong> Dendrit berfungsi menerima sinyal atau rangsangan dari neuron lain dan menghantarkannya menuju badan sel. Selain itu, dendrit juga berperan dalam menentukan kekuatan sinyal yang diterima oleh neuron.</li>
            <li><strong>Akson:</strong> Akson merupakan serabut panjang yang berfungsi mengirimkan impuls saraf dari badan sel menuju neuron lain atau target, seperti otot, atau kelenjar.</li>
            <li><strong>Selubung mielin:</strong> Selubung mielin merupakan selaput putih yang tersusun atas lemak berbentuk seperti wax/lilin yang membungkus sebagian besar serabut saraf panjang. Selubung ini memastikan sinyal listrik berjalan sesuai jalurnya.</li>
        </ul>
        <a href="https://skfb.ly/oPDwP" target="_blank" class="link-3d">Lihat Struktur Anatomi Neuron (3D)</a>
    </div>

    <!-- Slide 4: Klasifikasi Neuron -->
    <div class="card">
        <h2>Klasifikasi Neuron</h2>
        <p>Klasifikasi neuron berdasarkan fungsi terdiri dari:</p>
        <ul>
            <li><strong>Neuron Sensorik:</strong> Neuron sensorik berfungsi membawa informasi dari reseptor indra menuju sistem saraf pusat, seperti rangsangan sentuhan, cahaya, suara, dan rasa sakit.</li>
            <li><strong>Neuron Motorik:</strong> Neuron motorik berfungsi mengirimkan perintah dari sistem saraf pusat menuju otot atau kelenjar untuk menghasilkan respons berupa gerakan atau sekresi.</li>
            <li><strong>Interneuron:</strong> Interneuron berperan sebagai penghubung antara neuron sensorik dan neuron motorik di dalam sistem saraf pusat. Interneuron berfungsi memproses dan mengintegrasikan informasi sebelum menghasilkan respons yang sesuai. Jenis neuron ini sangat penting dalam aktivitas kompleks seperti berpikir, belajar, dan pengambilan keputusan.</li>
        </ul>
    </div>

    <!-- Slide 5, 6, 7: Fisiologi Potensial Membran & Potensial Aksi -->
    <div class="card">
        <h2>Fisiologi Potensial Membran Istirahat dan Generasi Potensial Aksi</h2>
        
        <div class="img-container">
            <img src="potensial.png" alt="Potensial Membran">
        </div>

        <h3>1. Potensial Istirahat</h3>
        <p>Pada keadaan istirahat (resting state), bagian dalam neuron cenderung bermuatan negatif dibandingkan bagian luar sel. Kondisi ini disebut sebagai potensial istirahat (resting membrane potential), yang umumnya berkisar sekitar -70 mV. Keadaan ini dipertahankan oleh kerja pompa natrium-kalium (Na⁺/K⁺ pump) yang secara aktif memompa ion natrium keluar sel dan ion kalium masuk ke dalam sel dengan menggunakan energi ATP.</p>

        <h3>2. Potensial Aksi</h3>
        <ul>
            <li><strong>Depolarisasi:</strong> Pada tahap ini, kanal natrium terbuka sehingga ion Na⁺ masuk ke dalam sel dan menyebabkan bagian dalam sel menjadi lebih positif. Perubahan ini memicu terbentuknya impuls listrik atau potensial aksi yang akan merambat sepanjang akson.</li>
            <li><strong>Repolarisasi:</strong> Setelah depolarisasi mencapai puncaknya, kanal natrium akan menutup dan kanal kalium (K⁺) terbuka. Ion kalium keluar dari sel, sehingga muatan di dalam sel kembali menjadi negatif.</li>
            <li><strong>Hiperpolarisasi:</strong> Penurunan muatan sesaat melebihi batas istirahat sebelum kembali stabil.</li>
        </ul>

        <h3>3. Konduksi Saltatori</h3>
        <p>Penghantaran impuls yang "melompat" antar Nodus Ranvier pada akson bermielin (mempercepat transmisi).</p>
    </div>

    <!-- Slide 8, 9, 10: Transmisi Sinapsis Kimia & Neurotransmitter -->
    <div class="card">
        <h2>Mekanisme Transmisi Sinapsis Kimia dan Peran Neurotransmitter</h2>
        <p>Sinapsis adalah titik pertemuan fungsional antara satu neuron dengan neuron lainnya, atau antara neuron dengan sel target seperti otot dan kelenjar. Pada sinapsis tidak terjadi kontak langsung antara membran sel, melainkan terdapat celah kecil yang disebut celah sinaptik (synaptic cleft). Melalui struktur inilah informasi dari satu neuron diteruskan ke neuron berikutnya dalam bentuk sinyal kimia.</p>

        <div class="img-container">
            <img src="sinapsis.png"Sinapsis Kimia">
        </div>

        <h3>Mekanisme Transmisi Sinapsis Kimia:</h3>
        <ol>
            <li>Impuls saraf sampai di terminal akson kemudian Kanal Kalsium (Ca²⁺) terbuka.</li>
            <li>Ion (Ca²⁺) masuk yang memicu untuk bergerak dan berfusi dengan membran presinaptik.</li>
            <li>Pelepasan Neurotransmitter ke celah sinaptik secara eksositosis.</li>
            <li>Neurotransmitter berikatan dengan reseptor di membran postsinaptik.</li>
            <li>Terjadi respon (eksitasi / inhibisi) pada sel penerima.</li>
        </ol>

        <h3>Peran Neurotransmitter</h3>
        <p>Neurotransmitter adalah zat kimia pembawa pesan yang berfungsi mentransfer informasi dari neuron presinaptik ke neuron postsinaptik. Contoh neurotransmitter antara lain asetilkolin, dopamin, serotonin, dan norepinefrin, yang masing-masing memiliki fungsi berbeda dalam sistem saraf.</p>
        <p>Setelah proses transmisi selesai, neurotransmitter akan diuraikan oleh enzim, diserap kembali ke neuron presinaptik (reuptake), atau menyebar menjauh dari sinapsis. Mekanisme ini penting untuk menghentikan sinyal agar tidak terjadi stimulasi berlebihan yang dapat mengganggu fungsi sistem saraf.</p>
    </div>

    <!-- Slide 11 & 12: Otak Besar (Serebrum) & Lobus -->
    <div class="card">
        <h2>Otak Besar (Serebrum)</h2>
        <ul>
            <li>Memiliki porsi otak terbesar dengan berat mencapai 2/3 dari berat keseluruhan.</li>
            <li>Terbagi menjadi 2 hemisfer yaitu otak kanan & otak kiri.</li>
            <li>Bersifat kontralateral.</li>
            <li>Dilapisi oleh lapisan luar yang disebut korteks serebral.</li>
            <li>Memiliki lipatan khas yaitu Gyrus (tonjolan) dan Sulcus (celah).</li>
        </ul>

        <div class="img-container">
            <img src="lobus-lobus korteks serebral.png"Lobus Otak">
        </div>

        <h3>Pembagian Fungsi Lobus-Lobus Korteks Serebral:</h3>
        <ol>
            <li><strong>Lobus Frontalis (Depan):</strong> Pusat kendali motorik, bicara, emosi, penalaran, & perencanaan.</li>
            <li><strong>Lobus Parietalis (Atas Tengah):</strong> Pusat pemrosesan sensorik (sentuhan, tekanan, nyeri, spasial).</li>
            <li><strong>Lobus Oksipitalis (Belakang):</strong> Pusat pemrosesan visual (penglihatan).</li>
            <li><strong>Lobus Temporalis (Samping):</strong> Pusat pendengaran, memori, & pemahaman bahasa (Area Wernicke).</li>
        </ol>
    </div>

    <!-- Slide 13: Otak Kecil (Serebelum) -->
    <div class="card">
        <h2>Otak Kecil (Serebelum)</h2>
        <p>Terdapat di bagian bawah belakang otak besar, tepat di belakang batang otak. Berfungsi untuk menyelaraskan dan mengkoordinasikan gerakan. Otak kecil ini terbagi menjadi 3 lobus utama yaitu:</p>
        <ol>
            <li><strong>Lobus Anterior:</strong> Mengatur postur & tonus otot.</li>
            <li><strong>Lobus Posterior:</strong> Mengatur keterampilan motorik halus.</li>
            <li><strong>Lobus Flocculonodularis:</strong> Menjaga keseimbangan & gerakan bola mata.</li>
        </ol>
    </div>

    <!-- Slide 14: Batang Otak (Brainstem) -->
    <div class="card">
        <h2>Batang Otak (Brainstem)</h2>
        <p>Penghubung antara otak besar (serebrum) dan sumsum tulang belakang (medula spinalis). Ada 3 bagian utama dari batang otak yaitu:</p>
        <ol>
            <li><strong>Otak Tengah (Mesensefalon):</strong> Pusat refleks penglihatan (superior colliculi), pendengaran (inferior colliculi), & kontrol gerakan (substantia nigra).</li>
            <li><strong>Pons:</strong> Jembatan sistem saraf & pengatur irama pernapasan.</li>
            <li><strong>Medulla Oblongata:</strong> Pusat refleks otonom vital (denyut jantung, tekanan darah, pernapasan, batuk, bersin, menelan).</li>
        </ol>
    </div>

    <!-- Slide 15: Diensefalon -->
    <div class="card">
        <h2>Diensefalon (Otak Antara)</h2>
        <p>Terletak di bagian tengah yaitu di antara otak besar (serebrum) dan batang otak. Diensefalon ini memiliki 4 bagian utama yaitu:</p>
        <div class="grid-2">
            <div style="background:#fff; padding:15px; border-radius:8px;">
                <h3>Talamus</h3>
                <p>Stasiun penerima & pemancar sinyal sensorik ke korteks otak.</p>
            </div>
            <div style="background:#fff; padding:15px; border-radius:8px;">
                <h3>Hipotalamus</h3>
                <p>Pusat homeostasis (keseimbangan tubuh), pengatur suhu, emosi, dorongan biologis, & penghubung ke sistem hormon (endokrin).</p>
            </div>
            <div style="background:#fff; padding:15px; border-radius:8px;">
                <h3>Epitalamus</h3>
                <p>Memuat kelenjar pineal (penghasil hormon melatonin untuk mengatur pola tidur).</p>
            </div>
            <div style="background:#fff; padding:15px; border-radius:8px;">
                <h3>Subtalamus</h3>
                <p>Membantu koordinasi dan pemulusan gerakan motorik.</p>
            </div>
        </div>
    </div>

    <!-- Slide 16, 17, 18: Sumsum Tulang Belakang -->
    <div class="card">
        <h2>Sumsum Tulang Belakang</h2>
        <ul>
            <li>Lanjutan dari medulla oblongata yang memanjang di dalam saluran tulang belakang.</li>
            <li>Dilindungi oleh tiga lapisan meninges yaitu dura mater (luar), arachnoid mater (tengah) dan pia mater (dalam).</li>
            <li>Memiliki cairan serebrospinal yang berfungsi untuk meredam benturan dan memberi nutrisi.</li>
        </ul>

        <h3>Fungsi Utama Sumsum Tulang Belakang:</h3>
        <ul>
            <li><strong>Jalur Asenden:</strong> Menghantar impuls indera dari tubuh ke otak.</li>
            <li><strong>Jalur Desenden:</strong> Menghantar perintah gerak dari otak ke organ/otot.</li>
            <li><strong>Pusat Integrasi Refleks:</strong> Mengendalikan refleks spinal spontan tanpa menunggu instruksi otak besar.</li>
        </ul>

        <h3>Struktur Penampang Melintang Sumsum Tulang Belakang:</h3>
        <ol>
            <li><strong>Substansia Alba (substansi putih):</strong> Berada di bagian luar, terdiri dari serat saraf bermielin. Memuat traktus asenden dan desenden.</li>
            <li><strong>Substansia Grisea (substansi kelabu):</strong> Berada di bagian dalam, terdiri dari akumulasi badan sel neuron & interneuron. Terbagi menjadi:
                <ul>
                    <li>Tanduk Dorsal (Belakang): Menerima masukan sinyal sensorik.</li>
                    <li>Tanduk Ventral (Depan): Mengirim perintah motorik ke otot.</li>
                    <li>Tanduk Lateral: Integrasi sistem saraf otonom.</li>
                </ul>
            </li>
            <li><strong>Kanalis Centralis:</strong> Saluran kecil di pusat medula spinalis yang berisi cairan serebrospinal.</li>
        </ol>
    </div>

    <!-- Slide 19 & 20: Lengkung Refleks Spinal dan Kranial -->
    <div class="card">
        <h2>Jalur Lengkung Refleks Spinal dan Kranial</h2>
        <p>Jalur saraf cepat & otomatis untuk tindakan perlindungan tubuh instan tanpa berpikir di otak besar.</p>

        <h3>1. Jalur Refleks Saraf Spinal</h3>
        <ul>
            <li>Dipproses langsung di Sumsum Tulang Belakang (Medula Spinalis).</li>
            <li>Mengontrol 31 pasang saraf spinal (Servikalis, Brakialis, Lumbalis, Sakralis).</li>
            <li><strong>Alur:</strong> Reseptor → Neuron Sensorik → Sumsum Tulang Belakang → Neuron Motorik → Efektor.</li>
        </ul>

        <h3>2. Jalur Refleks Saraf Kranial</h3>
        <ul>
            <li>Diproses langsung di Batang Otak (Brainstem) (Otak Tengah, Pons, & Medula Oblongata).</li>
            <li>Mengontrol 12 Pasang Saraf Kranial (area kepala, wajah, dan organ indra).</li>
            <li><strong>Komponen:</strong>
                <ul>
                    <li>Reseptor: Retina mata (menangkap stimulus cahaya).</li>
                    <li>Neuron Sensorik: Optic Nerve (membawa impuls ke batang otak).</li>
                    <li>Pusat Integrasi: Batang Otak (mengolah instruksi refleks).</li>
                    <li>Neuron Motorik: Third Cranial Nerve (Okulomotor).</li>
                    <li>Efektor: Otot pupil mata (pupil mengecil otomatis).</li>
                </ul>
            </li>
        </ul>
    </div>

    <!-- Slide 21: Simpatis dan Parasimpatis -->
    <div class="card">
        <h2>Perbedaan Fisiologi Sistem Saraf Simpatis dan Parasimpatis</h2>
        
        <h3>1. Sistem Saraf Simpatis (Fight or Flight)</h3>
        <p>Sistem Saraf Simpatis merupakan divisi Sistem Saraf Otonom yang mengendalikan respons tubuh saat menghadapi kondisi stres atau situasi darurat (fight or flight). Mekanisme utamanya berfokus pada pemanfaatan energi secara cepat dengan memacu kinerja organ vital, seperti meningkatkan denyut jantung dan pernapasan, sembari menghambat fungsi non-mendesak seperti pencernaan.</p>
        <p><em>Fungsi Simpatik:</em> Pupil mata membesar, nafas makin cepat, ludah berkurang, denyut jantung makin cepat, stimulasi gula darah, sekresi adrenalin, pelambatan kerja pencernaan, relaksasi kandung kemih, aktivitas genital terhambat.</p>

        <h3>2. Sistem Saraf Parasimpatis (Rest and Digest)</h3>
        <p>Sistem Saraf Parasimpatis merupakan divisi Sistem Saraf Otonom yang mendominasi saat tubuh berada dalam keadaan tenang, aman, dan beristirahat (rest and digest). Mekanisme utamanya berfokus pada pemulihan dan pemeliharaan energi tubuh dengan cara menenangkan laju kardiovaskular, melambatkan pernapasan, serta mengaktifkan kembali proses pencernaan.</p>
        <p><em>Fungsi Parasimpatik:</em> Pupil mata menyempit, stimulasi kelenjar ludah, nafas melambat, denyut jantung melambat, stimulasi kelenjar empedu, stimulasi saluran pencernaan, kontraksi kandung kemih, stimulasi alat kelamin.</p>
    </div>

    <!-- Slide 22, 23, 24, 25: Kelainan Sistem Saraf -->
    <div class="card">
        <h2>Kelainan Sistem Saraf</h2>

        <h3>1. Stroke</h3>
        <p>Stroke merupakan gangguan fungsi otak akut akibat terhentinya pasokan darah ke otak, baik karena penyumbatan (stroke iskemik) maupun pecahnya pembuluh darah (stroke hemoragik). Kondisi ini menyebabkan sel-sel otak mengalami kekurangan oksigen secara mendadak, sehingga memicu kerusakan jaringan saraf dan penurunan fungsi tubuh.</p>
        <ul>
            <li><strong>Stroke Iskemik:</strong> Gumpalan darah menghalangi aliran darah (Trombotik & Emboli).</li>
            <li><strong>Stroke Hemoragik:</strong> Pembuluh darah pecah dan pendarahan (Perdarahan Intraserebral/IHC & Perdarahan Subarachnoid/SAH).</li>
        </ul>

        <h3>2. Multiple Sclerosis (MS)</h3>
        <p>Multiple Sclerosis merupakan penyakit autoimun kronis pada sistem saraf pusat yang terjadi ketika sistem kekebalan tubuh merusak selubung mielin (pelindung serabut saraf). Kerusakan ini menghambat penghantaran impuls listrik saraf, sehingga memicu gangguan koordinasi, kelemahan otot, dan gangguan penglihatan.</p>

        <h3>3. Bell's Palsy</h3>
        <p>Bell's Palsy merupakan kondisi kelumpuhan atau kelemahan mendadak pada otot salah satu sisi wajah akibat peradangan atau penekanan pada Nervus Fasialis (Saraf Kranial VII). Gangguan ini bersifat sementara dan menyebabkan wajah tampak melorot, kesulitan tersenyum atau menutup mata, serta penurunan fungsi pengecapan pada lidah.</p>

        <h3>4. Penyakit Parkinson</h3>
        <p>Penyakit Parkinson merupakan gangguan degeneratif sistem saraf pusat yang terjadi akibat kemunduran sel-sel saraf penghasil dopamin di area substantia nigra otak. Defisiensi dopamin ini mengganggu sistem kontrol gerakan tubuh, sehingga memicu gejala khas berupa tremor saat istirahat (resting tremor), kekakuan otot, kelambatan gerak (bradikinesia), serta ketidakseimbangan postur.</p>
    </div>

    <!-- Slide 26: Referensi -->
    <div class="card">
        <h2>Referensi</h2>
        <ul style="font-size: 0.9rem;">
            <li>Akmal Subarjah, M., Muhammad Hasan, R., & Demexsi Rahmat, W. (2024). Sistem Saraf Otonom: Mengatur Aktivitas Tanpa Kesadaran. <i>Journal Human Resource Strengthening</i>, 1(1), 67-70.</li>
            <li>Dinata, C. A., Safrita, Y. S., & Sastri, S. (2013). Gambaran Faktor Risiko dan Tipe Stroke pada Pasien Rawat Inap di Bagian Penyakit Dalam RSUD Kabupaten Solok Selatan Periode 1 Januari 2010 -31 Juni 2012. <i>Jurnal Kesehatan Andalas</i>, 2(2), 57.</li>
            <li>Dobson, R., & Giovannoni, G. (2019). Multiple sclerosis - a review. <i>European Journal of Neurology</i>, 26(1), 27-40.</li>
            <li>Eva Zulisa, dkk. (2021). <i>ANATOMI DAN FISIOLOGI TUBUH MANUSIA</i>. Penerbit Zaini.</li>
            <li>Meutia, S., Utami, N., Rahmawati, S., & Himayani, R. (2021). Sistem Saraf Pusat dan Perifer. <i>Medical Profession Journal of Lampung</i>, 11(2), 306-311.</li>
            <li>Muttaqin, A. (2020). <i>Asuhan Keperawatan Klien dengan Gangguan Sistem Persarafan</i>. Salemba Medika.</li>
            <li>Ramadhani, K., dkk. <i>BUKU AJAR DASAR-DASAR ANATOMI DAN FISIOLOGI TUBUH MANUSIA</i>.</li>
            <li>Sari, N. R. (2021). <i>SISTEM SARAF</i>. NUSAMEDIA.</li>
            <li>Tranggono Yudo Utomo, & Frisca Angreni. <i>DASAR-DASAR ILMU SARAF: MEMAHAMI STRUKTUR DAN FUNGSI OTAK MANUSIA</i>.</li>
            <li>Widodo, H. (2019). <i>Memahami Sistem Saraf Manusia</i>. Mutiara Aksara.</li>
            <li>Yudawijaya & Pariama. (2024). <i>SISTEM SARAF PERIFERAL: STRUKTUR, FUNGSI, DAN GANGGUAN KLINIS</i>. Yayasan Putra Adi Dharma.</li>
            <li>Yunita, A. S. (2023). <i>STRUKTUR OTAK MANUSIA</i>.</li>
            <li>Zulkifli, Z., dkk. (2025). Mekanisme Kerja Otak dan Sistem Saraf: Perspektif Neurosains Pendidikan Islam. <i>Menara Ilmu</i>, 19(1), 118-130.</li>
        </ul>
    </div>

    <!-- Slide 27: Penutup -->
    <div class="card" style="text-align: center;">
        <h1>Terima Kasih</h1>
        <p>Sampai Jumpa di Pertemuan Selanjutnya</p>
    </div>

</div>

</body>
</html>
