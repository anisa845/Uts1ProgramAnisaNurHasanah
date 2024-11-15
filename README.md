# ProgramAnisaNurHasanah
Perkenalkan nama saya Anisa Nur Hasanah, Mahasiswa Semester 1 Jurusan Teknik Informatika, Kampus STIKOM MUHAMMADIYAH Batam.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello, World</title>
</head>
<body>
    <h1>Hello, World!</h1>
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
            const alas = parseFloat(document.getElementById("alas").value);
            const tinggi = parseFloat(document.getElementById("tinggi").value);
            if (alas > 0 && tinggi > 0) {
                const luas = 0.5 * alas * tinggi;
                document.getElementById("hasil").innerText = `Luas Segitiga: ${luas} satuan luas`;
            } else {
                document.getElementById("hasil").innerText = "Masukkan angka yang valid.";
            }
        }
    </script>
</head>
<body>
    <h2>Hitung Luas Segitiga</h2>
    <label>Alas: </label><input type="number" id="alas"><br><br>
    <label>Tinggi: </label><input type="number" id="tinggi"><br><br>
    <button onclick="hitungLuasSegitiga()">Hitung</button>
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <title>Luas Persegi Panjang</title>
    <script>
        function hitungLuas() {
            const panjang = parseFloat(document.getElementById("panjang").value);
            const lebar = parseFloat(document.getElementById("lebar").value);
            if (panjang > 0 && lebar > 0) {
                const luas = panjang * lebar;
                document.getElementById("hasil").innerText = `Luas Persegi Panjang: ${luas} satuan luas`;
            } else {
                document.getElementById("hasil").innerText = "Masukkan angka yang valid.";
            }
        }
    </script>
</head>
<body>
    <h2>Hitung Luas Persegi Panjang</h2>
    <label>Panjang: </label><input type="number" id="panjang"><br><br>
    <label>Lebar: </label><input type="number" id="lebar"><br><br>
    <button onclick="hitungLuas()">Hitung</button>
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <title>Konversi Suhu</title>
    <script>
        function konversiSuhu() {
            const celsius = parseFloat(document.getElementById("celsius").value);
            const fahrenheit = (celsius * 9 / 5) + 32;
            document.getElementById("hasil").innerText = `${celsius}°C = ${fahrenheit.toFixed(2)}°F`;
        }
    </script>
</head>
<body>
    <h2>Konversi Celsius ke Fahrenheit</h2>
    <label>Celsius: </label><input type="number" id="celsius"><br><br>
    <button onclick="konversiSuhu()">Konversi</button>
    <p id="hasil"></p>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <title>Kecepatan</title>
    <script>
        function hitungKecepatan() {
            const jarak = parseFloat(document.getElementById("jarak").value);
            const waktu = parseFloat(document.getElementById("waktu").value);
            if (waktu > 0) {
                const kecepatan = jarak / waktu;
                document.getElementById("hasil").innerText = `Kecepatan: ${kecepatan.toFixed(2)} m/s`;
            } else {
                document.getElementById("hasil").innerText = "Waktu tidak boleh nol.";
            }
        }
    </script>
</head>
<body>
    <h2>Hitung Kecepatan</h2>
    <label>Jarak (m): </label><input type="number" id="jarak"><br><br>
    <label>Waktu (s): </label><input type="number" id="waktu"><br><br>
    <button onclick="hitungKecepatan()">Hitung</button>
    <p id="hasil"></p>
</body>
</html>


