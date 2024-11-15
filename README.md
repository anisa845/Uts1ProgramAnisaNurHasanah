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
    <title>Hitung Luas Persegi Panjang</title>
    <script>
        function hitungLuasPersegiPanjang() {
            const panjang = parseFloat(document.getElementById("panjang").value);
            const lebar = parseFloat(document.getElementById("lebar").value);

            // Validasi input
            if (isNaN(panjang) || isNaN(lebar) || panjang <= 0 || lebar <= 0) {
                document.getElementById("hasil").innerText = "Masukkan panjang dan lebar yang valid!";
                return;
            }

            // Hitung luas
            const luas = panjang * lebar;

            // Tampilkan hasil
            document.getElementById("hasil").innerText = `Luas Persegi Panjang: ${luas} satuan luas.`;
        }
    </script>
</head>
<body>
    <h1>Hitung Luas Persegi Panjang</h1>
    <p>Masukkan nilai panjang dan lebar persegi panjang:</p>
    <label for="panjang">Panjang:</label>
    <input type="number" id="panjang" placeholder="Masukkan panjang"><br><br>
    <label for="lebar">Lebar:</label>
    <input type="number" id="lebar" placeholder="Masukkan lebar"><br><br>
    <button onclick="hitungLuasPersegiPanjang()">Hitung Luas</button>
    <p id="hasil" style="font-weight: bold; color: green;"></p>
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



