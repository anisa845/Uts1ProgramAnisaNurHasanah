# ProgramAnisaNurHasanah
Perkenalkan nama saya Anisa Nur Hasanah, Mahasiswa Semester 1 Jurusan Teknik Informatika, Kampus STIKOM MUHAMMADIYAH Batam



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
    <title>Luas Segitiga</title>
    <script>
        function hitungLuasSegitiga() {
            // Ambil nilai alas dan tinggi dari input pengguna
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
            document.getElementById("hasil").innerText = "Luas Segitiga: " + luas.toFixed(2) + " satuan luas.";
        }
    </script>
</head>
<body>
    <h1>Hitung Luas Segitiga</h1>
    <p>Masukkan alas dan tinggi segitiga:</p>
    <label for="alas">Alas:</label>
    <input type="number" id="alas" placeholder="Masukkan alas" required>
    <br><br>
    <label for="tinggi">Tinggi:</label>
    <input type="number" id="tinggi" placeholder="Masukkan tinggi" required>
    <br><br>
    <button onclick="hitungLuasSegitiga()">Hitung Luas</button>
    <p id="hasil" style="font-weight: bold; color: blue;"></p>
</body>
</html>
