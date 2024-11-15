# ProgramAnisaNurHasanah
Perkenalkan nama saya Anisa Nur Hasanah, Mahasiswa Semester 1 Jurusan Teknik Informatika, Kampus STIKOM MUHAMMADIYAH Batam.



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello World</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>Welcome to my first HTML program.</p>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hitung Luas Segitiga</title>
    <script>
        function hitungLuasSegitiga() {
            const alas = parseFloat(document.getElementById("alas").value);
            const tinggi = parseFloat(document.getElementById("tinggi").value);

            // Validasi input
            if (isNaN(alas) || isNaN(tinggi) || alas <= 0 || tinggi <= 0) {
                document.getElementById("hasil").innerText = "Masukkan nilai alas dan tinggi yang valid!";
                return;
            }

            // Hitung luas segitiga
            const luas = 0.5 * alas * tinggi;

            // Tampilkan hasil
            document.getElementById("hasil").innerText = `Luas Segitiga: ${luas.toFixed(2)} satuan luas.`;
        }
    </script>
</head>
<body>
    <h1>Hitung Luas Segitiga</h1>
    <p>Masukkan nilai alas dan tinggi segitiga:</p>
    <label for="alas">Alas:</label>
    <input type="number" id="alas" placeholder="Masukkan alas"><br><br>
    <label for="tinggi">Tinggi:</label>
    <input type="number" id="tinggi" placeholder="Masukkan tinggi"><br><br>
    <button onclick="hitungLuasSegitiga()">Hitung Luas</button>
    <p id="hasil" style="font-weight: bold; color: blue;"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hitung Luas Persegi Panjang</title>
    <script>
        function hitungLuas() {
            var panjang = document.getElementById("panjang").value;
            var lebar = document.getElementById("lebar").value;
            var luas = panjang * lebar;
            document.getElementById("hasil").innerHTML = "Luas Persegi Panjang: " + luas + " cm²";
        }
    </script>
</head>
<body>
    <h1>Program Menghitung Luas Persegi Panjang</h1>
    <label for="panjang">Panjang (cm): </label>
    <input type="number" id="panjang" required><br><br>
    
    <label for="lebar">Lebar (cm): </label>
    <input type="number" id="lebar" required><br><br>
    
    <button onclick="hitungLuas()">Hitung Luas</button>
    
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Konversi Suhu Celsius ke Fahrenheit</title>
    <script>
        function konversiSuhu() {
            var celsius = document.getElementById("celsius").value;
            var fahrenheit = (celsius * 9/5) + 32;
            document.getElementById("hasil").innerHTML = celsius + "°C = " + fahrenheit.toFixed(2) + "°F";
        }
    </script>
</head>
<body>
    <h1>Program Konversi Suhu dari Celsius ke Fahrenheit</h1>
    <label for="celsius">Masukkan suhu dalam Celsius (°C): </label>
    <input type="number" id="celsius" required><br><br>
    
    <button onclick="konversiSuhu()">Konversi ke Fahrenheit</button>
    
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hitung Kecepatan</title>
    <script>
        function hitungKecepatan() {
            var jarak = document.getElementById("jarak").value;
            var waktu = document.getElementById("waktu").value;

            // Menghindari pembagian dengan nol
            if (waktu == 0) {
                document.getElementById("hasil").innerHTML = "Waktu tidak bisa nol!";
                return;
            }

            var kecepatan = jarak / waktu;
            document.getElementById("hasil").innerHTML = "Kecepatan: " + kecepatan.toFixed(2) + " m/s";
        }
    </script>
</head>
<body>
    <h1>Program Menghitung Kecepatan</h1>
    <label for="jarak">Jarak (meter): </label>
    <input type="number" id="jarak" required><br><br>
    
    <label for="waktu">Waktu (detik): </label>
    <input type="number" id="waktu" required><br><br>
    
    <button onclick="hitungKecepatan()">Hitung Kecepatan</button>
    
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hitung Resistansi Paralel 3 Resistor</title>
    <script>
        function hitungResistansiParalel() {
            var r1 = parseFloat(document.getElementById("r1").value);
            var r2 = parseFloat(document.getElementById("r2").value);
            var r3 = parseFloat(document.getElementById("r3").value);
            
            // Menghitung resistansi total menggunakan rumus paralel
            var rTotal = 1 / ((1 / r1) + (1 / r2) + (1 / r3));
            
            // Menampilkan hasil resistansi total
            document.getElementById("hasil").innerHTML = "Resistansi Total: " + rTotal.toFixed(2) + " Ohm";
        }
    </script>
</head>
<body>
    <h1>Program Menghitung Resistansi Paralel (3 Resistor)</h1>
    
    <label for="r1">Resistor 1 (Ohm): </label>
    <input type="number" id="r1" required><br><br>
    
    <label for="r2">Resistor 2 (Ohm): </label>
    <input type="number" id="r2" required><br><br>
    
    <label for="r3">Resistor 3 (Ohm): </label>
    <input type="number" id="r3" required><br><br>
    
    <button onclick="hitungResistansiParalel()">Hitung Resistansi Total</button>
    
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hitung Nilai Resistor 4 Gelang Warna</title>
    <script>
        // Kode warna untuk nilai resistor
        const warna = {
            "hitam": 0, "coklat": 1, "merah": 2, "oranye": 3,
            "kuning": 4, "hijau": 5, "biru": 6, "ungu": 7,
            "abu-abu": 8, "putih": 9
        };

        // Kode warna untuk pengali (faktor perbanyakan)
        const pengali = {
            "hitam": 1, "coklat": 10, "merah": 100, "oranye": 1000,
            "kuning": 10000, "hijau": 100000, "biru": 1000000, 
            "ungu": 10000000, "abu-abu": 100000000, "putih": 1000000000,
            "emas": 0.1, "perak": 0.01
        };

        function hitungNilaiResistor() {
            var gelang1 = document.getElementById("gelang1").value.toLowerCase();
            var gelang2 = document.getElementById("gelang2").value.toLowerCase();
            var gelang3 = document.getElementById("gelang3").value.toLowerCase();
            var gelang4 = document.getElementById("gelang4").value.toLowerCase();

            if (warna[gelang1] === undefined || warna[gelang2] === undefined || pengali[gelang3] === undefined) {
                document.getElementById("hasil").innerHTML = "Kode warna tidak valid.";
                return;
            }

            // Menentukan nilai resistor berdasarkan gelang warna
            var angka1 = warna[gelang1];
            var angka2 = warna[gelang2];
            var faktor = pengali[gelang3];
            var toleransi = (gelang4 === "emas") ? "±5%" : (gelang4 === "perak" ? "±10%" : "Tidak Diketahui");

            // Menghitung nilai resistor
            var nilaiResistor = (angka1 * 10 + angka2) * faktor;
            
            // Menampilkan hasil
            document.getElementById("hasil").innerHTML = "Nilai Resistor: " + nilaiResistor + " Ohm, Toleransi: " + toleransi;
        }
    </script>
</head>
<body>
    <h1>Program Menghitung Nilai Resistor dengan 4 Gelang Warna</h1>
    
    <label for="gelang1">Gelang 1 (Angka pertama): </label>
    <input type="text" id="gelang1" required><br><br>
    
    <label for="gelang2">Gelang 2 (Angka kedua): </label>
    <input type="text" id="gelang2" required><br><br>
    
    <label for="gelang3">Gelang 3 (Pengali): </label>
    <input type="text" id="gelang3" required><br><br>
    
    <label for="gelang4">Gelang 4 (Toleransi): </label>
    <input type="text" id="gelang4" required><br><br>
    
    <button onclick="hitungNilaiResistor()">Hitung Nilai Resistor</button>
    
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hitung Nilai Tertinggi dan Terendah</title>
    <script>
        function hitungNilai() {
            var angka = [];
            for (var i = 1; i <= 10; i++) {
                var nilai = parseFloat(document.getElementById("angka" + i).value);
                if (!isNaN(nilai)) {
                    angka.push(nilai);
                }
            }

            if (angka.length !== 10) {
                document.getElementById("hasil").innerHTML = "Harap masukkan 10 angka!";
                return;
            }

            var tertinggi = Math.max(...angka);
            var terendah = Math.min(...angka);

            document.getElementById("hasil").innerHTML = 
                "Nilai Tertinggi: " + tertinggi + "<br>" + 
                "Nilai Terendah: " + terendah;
        }
    </script>
</head>
<body>
    <h1>Program Menghitung Nilai Tertinggi dan Terendah dari 10 Angka</h1>
    
    <p>Masukkan 10 angka di bawah ini:</p>
    
    <form>
        <label for="angka1">Angka 1: </label><input type="number" id="angka1" required><br><br>
        <label for="angka2">Angka 2: </label><input type="number" id="angka2" required><br><br>
        <label for="angka3">Angka 3: </label><input type="number" id="angka3" required><br><br>
        <label for="angka4">Angka 4: </label><input type="number" id="angka4" required><br><br>
        <label for="angka5">Angka 5: </label><input type="number" id="angka5" required><br><br>
        <label for="angka6">Angka 6: </label><input type="number" id="angka6" required><br><br>
        <label for="angka7">Angka 7: </label><input type="number" id="angka7" required><br><br>
        <label for="angka8">Angka 8: </label><input type="number" id="angka8" required><br><br>
        <label for="angka9">Angka 9: </label><input type="number" id="angka9" required><br><br>
        <label for="angka10">Angka 10: </label><input type="number" id="angka10" required><br><br>
        
        <button type="button" onclick="hitungNilai()">Hitung Nilai Tertinggi dan Terendah</button>
    </form>
    
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hitung Nilai Mahasiswa</title>
    <script>
        function hitungNilai() {
            // Mengambil nilai tugas dan ujian dari input
            var nilaiTugas = parseFloat(document.getElementById("nilaiTugas").value);
            var nilaiUjian = parseFloat(document.getElementById("nilaiUjian").value);

            // Validasi input
            if (isNaN(nilaiTugas) || isNaN(nilaiUjian)) {
                document.getElementById("hasil").innerHTML = "Harap masukkan nilai yang valid.";
                return;
            }

            // Menghitung nilai akhir dengan bobot
            var nilaiAkhir = (nilaiTugas * 0.4) + (nilaiUjian * 0.6);

            // Menentukan grade berdasarkan nilai akhir
            var grade = "";
            if (nilaiAkhir >= 85) {
                grade = "A";
            } else if (nilaiAkhir >= 70) {
                grade = "B";
            } else if (nilaiAkhir >= 55) {
                grade = "C";
            } else if (nilaiAkhir >= 40) {
                grade = "D";
            } else {
                grade = "E";
            }

            // Menampilkan hasil
            document.getElementById("hasil").innerHTML = 
                "Nilai Akhir: " + nilaiAkhir.toFixed(2) + "<br>" + 
                "Grade: " + grade;
        }
    </script>
</head>
<body>
    <h1>Program Menghitung Nilai Mahasiswa</h1>
    
    <label for="nilaiTugas">Nilai Tugas (0-100): </label>
    <input type="number" id="nilaiTugas" min="0" max="100" required><br><br>
    
    <label for="nilaiUjian">Nilai Ujian (0-100): </label>
    <input type="number" id="nilaiUjian" min="0" max="100" required><br><br>
    
    <button onclick="hitungNilai()">Hitung Nilai Akhir</button>
    
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kalkulator Sederhana</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f4f4f9;
        }
        .kalkulator {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .kalkulator input {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            font-size: 18px;
        }
        .kalkulator button {
            width: 45%;
            padding: 10px;
            margin: 5px 2.5%;
            font-size: 18px;
            cursor: pointer;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
        }
        .kalkulator button:hover {
            background-color: #45a049;
        }
    </style>
    <script>
        function hitung(operator) {
            var num1 = parseFloat(document.getElementById("num1").value);
            var num2 = parseFloat(document.getElementById("num2").value);
            var hasil;

            // Validasi jika input kosong
            if (isNaN(num1) || isNaN(num2)) {
                document.getElementById("hasil").innerHTML = "Harap masukkan kedua angka!";
                return;
            }

            switch (operator) {
                case 'tambah':
                    hasil = num1 + num2;
                    break;
                case 'kurang':
                    hasil = num1 - num2;
                    break;
                case 'kali':
                    hasil = num1 * num2;
                    break;
                case 'bagi':
                    if (num2 === 0) {
                        document.getElementById("hasil").innerHTML = "Pembagian dengan nol tidak diperbolehkan!";
                        return;
                    }
                    hasil = num1 / num2;
                    break;
                default:
                    document.getElementById("hasil").innerHTML = "Operasi tidak valid!";
                    return;
            }

            document.getElementById("hasil").innerHTML = "Hasil: " + hasil;
        }
    </script>
</head>
<body>

    <div class="kalkulator">
        <h2>Kalkulator Sederhana</h2>
        <input type="number" id="num1" placeholder="Masukkan angka pertama" required><br>
        <input type="number" id="num2" placeholder="Masukkan angka kedua" required><br><br>

        <button onclick="hitung('tambah')">+</button>
        <button onclick="hitung('kurang')">-</button>
        <button onclick="hitung('kali')">*</button>
        <button onclick="hitung('bagi')">/</button><br><br>

        <p id="hasil"></p>
    </div>

</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aplikasi Kasir</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .kasir-container {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
            width: 300px;
        }
        h2 {
            text-align: center;
        }
        input, button {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            font-size: 16px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
        .total {
            font-size: 18px;
            font-weight: bold;
            margin-top: 15px;
        }
    </style>
    <script>
        function tambahItem() {
            var namaBarang = document.getElementById("namaBarang").value;
            var hargaBarang = parseFloat(document.getElementById("hargaBarang").value);
            var jumlahBarang = parseInt(document.getElementById("jumlahBarang").value);
            
            // Validasi input
            if (!namaBarang || isNaN(hargaBarang) || isNaN(jumlahBarang) || hargaBarang <= 0 || jumlahBarang <= 0) {
                alert("Harap masukkan data yang valid!");
                return;
            }
            
            var totalItem = hargaBarang * jumlahBarang;
            var row = document.createElement("tr");

            // Menambahkan nama barang, harga, jumlah, dan total ke tabel
            row.innerHTML = `<td>${namaBarang}</td><td>${hargaBarang}</td><td>${jumlahBarang}</td><td>${totalItem}</td>`;
            document.getElementById("listBarang").appendChild(row);

            // Menghitung total belanja
            updateTotal(totalItem);
        }

        var totalBelanja = 0;
        function updateTotal(totalItem) {
            totalBelanja += totalItem;
            document.getElementById("totalBelanja").innerText = "Total Belanja: Rp " + totalBelanja.toFixed(2);
        }

        function resetBelanja() {
            totalBelanja = 0;
            document.getElementById("totalBelanja").innerText = "Total Belanja: Rp 0.00";
            document.getElementById("listBarang").innerHTML = "";
        }
    </script>
</head>
<body>

    <div class="kasir-container">
        <h2>Aplikasi Kasir</h2>

        <label for="namaBarang">Nama Barang</label>
        <input type="text" id="namaBarang" placeholder="Masukkan Nama Barang" required>

        <label for="hargaBarang">Harga Barang (Rp)</label>
        <input type="number" id="hargaBarang" placeholder="Masukkan Harga Barang" required>

        <label for="jumlahBarang">Jumlah</label>
        <input type="number" id="jumlahBarang" placeholder="Masukkan Jumlah" required>

        <button onclick="tambahItem()">Tambah Item</button>
        <button onclick="resetBelanja()">Reset Belanja</button>

        <h3>Daftar Belanja</h3>
        <table border="1" cellpadding="5">
            <thead>
                <tr>
                    <th>Nama Barang</th>
                    <th>Harga (Rp)</th>
                    <th>Jumlah</th>
                    <th>Total (Rp)</th>
                </tr>
            </thead>
            <tbody id="listBarang">
                <!-- Item yang ditambahkan akan muncul di sini -->
            </tbody>
        </table>

        <p class="total" id="totalBelanja">Total Belanja: Rp 0.00</p>
    </div>

</body>
</html>





