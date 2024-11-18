# ProgramAnisaNurHasanah
Perkenalkan nama saya Anisa Nur Hasanah, Mahasiswa Semester 1 Jurusan Teknik Informatika, Kampus STIKOM MUHAMMADIYAH Batam.

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Program Lengkap</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        h2 {
            color: #333;
        }
        .form-group {
            margin-bottom: 10px;
        }
        input, button {
            padding: 5px;
            margin: 5px 0;
        }
        button {
            cursor: pointer;
            background-color: #4CAF50;
            color: white;
            border: none;
        }
        button:hover {
            background-color: #45a049;
        }
        .result {
            margin-top: 10px;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <h1>Program Lengkap dalam Satu Aplikasi</h1>

    <!-- Program Hello World -->
    <section>
        <h2>1. Hello World</h2>
        <button onclick="cetakHelloWorld()">Cetak Hello World</button>
        <p id="helloWorld"></p>
    </section>

    <section>
        <h2>2. Hitung Luas Segitiga</h2>
        <div class="form-group">
            <label for="alas">Alas:</label>
            <input type="number" id="alasSegitiga" required>
        </div>
        <div class="form-group">
            <label for="tinggi">Tinggi:</label>
            <input type="number" id="tinggiSegitiga" required>
        </div>
        <button onclick="hitungLuasSegitiga()">Hitung Luas</button>
        <p id="hasilLuasSegitiga" class="result"></p>
    </section>

    <section>
        <h2>3. Hitung Luas Persegi Panjang</h2>
        <div class="form-group">
            <label for="panjang">Panjang:</label>
            <input type="number" id="panjang" required>
        </div>
        <div class="form-group">
            <label for="lebar">Lebar:</label>
            <input type="number" id="lebar" required>
        </div>
        <button onclick="hitungLuasPersegiPanjang()">Hitung Luas</button>
        <p id="hasilLuasPersegiPanjang" class="result"></p>
    </section>

    <section>
        <h2>4. Konversi Suhu Celcius ke Fahrenheit</h2>
        <div class="form-group">
            <label for="celsius">Suhu (Celsius):</label>
            <input type="number" id="celsius" required>
        </div>
        <button onclick="konversiSuhu()">Konversi</button>
        <p id="hasilKonversiSuhu" class="result"></p>
    </section>

    <section>
        <h2>5. Nilai Mahasiswa</h2>
        <div class="form-group">
            <label for="nilai">Masukkan Nilai (0-100):</label>
            <input type="number" id="nilai" required>
        </div>
        <button onclick="cekNilai()">Cek Nilai</button>
        <p id="hasilNilai" class="result"></p>
    </section>

    <section>
        <h2>6. Hukum Newton (F = m * a)</h2>
        <div class="form-group">
            <label for="massa">Massa (kg):</label>
            <input type="number" id="massa" required>
        </div>
        <div class="form-group">
            <label for="percepatan">Percepatan (m/s²):</label>
            <input type="number" id="percepatan" required>
        </div>
        <button onclick="hitungGaya()">Hitung Gaya</button>
        <p id="hasilGaya" class="result"></p>
    </section>

    <section>
        <h2>7. Resistor Paralel (3 Resistor)</h2>
        <div class="form-group">
            <label for="r1">Resistor 1 (Ohm):</label>
            <input type="number" id="r1" required>
        </div>
        <div class="form-group">
            <label for="r2">Resistor 2 (Ohm):</label>
            <input type="number" id="r2" required>
        </div>
        <div class="form-group">
            <label for="r3">Resistor 3 (Ohm):</label>
            <input type="number" id="r3" required>
        </div>
        <button onclick="hitungResistorParalel()">Hitung Resistansi</button>
        <p id="hasilResistor" class="result"></p>
    </section>

    <section>
        <h2>8. Data Tertinggi dan Terendah</h2>
        <div class="form-group">
            <label for="dataInput">Masukkan 10 angka (pisahkan dengan koma):</label>
            <input type="text" id="dataInput" required>
        </div>
        <button onclick="prosesData()">Proses Data</button>
        <p id="hasilData" class="result"></p>
    </section>

    <section>
        <h2>9. Resistor 4 Gelang Warna</h2>
        <div class="form-group">
            <label for="gelang1">Gelang 1 (digit pertama):</label>
            <input type="text" id="gelang1" required>
        </div>
        <div class="form-group">
            <label for="gelang2">Gelang 2 (digit kedua):</label>
            <input type="text" id="gelang2" required>
        </div>
        <div class="form-group">
            <label for="gelang3">Gelang 3 (digit ketiga):</label>
            <input type="text" id="gelang3" required>
        </div>
        <div class="form-group">
            <label for="gelang4">Gelang 4 (pengali):</label>
            <input type="text" id="gelang4" required>
        </div>
        <button onclick="hitungResistorGelang()">Hitung Resistansi</button>
        <p id="hasilResistorGelang" class="result"></p>
    </section>

    <section>
        <h2>10. Kalkulator Sederhana</h2>
        <div class="form-group">
            <input type="number" id="angka1" placeholder="Angka pertama" required>
            <select id="operator" required>
                <option value="+">Tambah (+)</option>
                <option value="-">Kurang (-)</option>
                <option value="">Kali ()</option>
                <option value="/">Bagi (/)</option>
            </select>
            <input type="number" id="angka2" placeholder="Angka kedua" required>
        </div>
        <button onclick="hitungKalkulator()">Hitung</button>
        <p id="hasilKalkulator" class="result"></p>
    </section>

    <section>
        <h2>11. Kasir</h2>
        <div class="form-group">
            <label for="harga">Harga Barang:</label>
            <input type="number" id="harga" required>
        </div>
        <div class="form-group">
            <label for="jumlah">Jumlah Barang:</label>
            <input type="number" id="jumlah" required>
        </div>
        <button onclick="hitungKasir()">Hitung Total</button>
        <p id="hasilKasir" class="result"></p>
    </section>

    <script>
        function cetakHelloWorld() {
            document.getElementById("helloWorld").innerText = "Hello, World!";
        }

        function hitungLuasSegitiga() {
            let alas = document.getElementById("alasSegitiga").value;
            let tinggi = document.getElementById("tinggiSegitiga").value;
            let luas = (alas * tinggi) / 2;
            document.getElementById("hasilLuasSegitiga").innerText = Luas Segitiga: ${luas} m²;
        }

        function hitungLuasPersegiPanjang() {
            let panjang = document.getElementById("panjang").value;
            let lebar = document.getElementById("lebar").value;
            let luas = panjang * lebar;
            document.getElementById("hasilLuasPersegiPanjang").innerText = Luas Persegi Panjang: ${luas} m²;
        }

        function konversiS






