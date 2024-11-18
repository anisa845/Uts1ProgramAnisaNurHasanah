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
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Luas Persegi Panjang</title>
    <script>
        function hitungLuas() {
            // Mengambil nilai panjang dan lebar dari input
            var panjang = document.getElementById('panjang').value;
            var lebar = document.getElementById('lebar').value;

            // Memastikan bahwa input valid
            if (panjang && lebar) {
                // Menghitung luas
                var luas = panjang * lebar;

                // Menampilkan hasil
                document.getElementById('hasil').innerHTML = 'Luas Persegi Panjang: ' + luas + ' cm²';
            } else {
                // Menampilkan pesan jika input kosong
                document.getElementById('hasil').innerHTML = 'Masukkan nilai panjang dan lebar!';
            }
        }
    </script>
</head>
<body>
    <h1>Perhitungan Luas Persegi Panjang</h1>
    
    <label for="panjang">Panjang (cm):</label>
    <input type="number" id="panjang" placeholder="Masukkan panjang" required>
    <br><br>

    <label for="lebar">Lebar (cm):</label>
    <input type="number" id="lebar" placeholder="Masukkan lebar" required>
    <br><br>

    <button onclick="hitungLuas()">Hitung Luas</button>

    <h2 id="hasil"></h2>
</body>
</html>







