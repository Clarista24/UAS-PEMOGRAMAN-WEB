<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <title>SELAMAT DATANG DI ECO PAWS CAT!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #9aa654;
            padding: 20px;
        }

        h1, h2 {
            color: #000000;
        }

        .product {
            background-color: #f9f9f9;
            border: 1px solid #ddd;
            padding: 15px;
            margin-bottom: 15px;
            border-radius: 10px;
        }

        .price {
            font-weight: bold;
            color: #e91e63;
        }

        .buy-button {
            color: white;
            background-color: #4CAF50;
            padding: 10px 15px;
            text-decoration: none;
            border-radius: 5px;
            cursor: pointer;
            display: inline-block;
            margin-top: 10px;
        }

        .buy-button:hover {
            background-color: #45a049;
        }

        #order-form {
            display: none;
            margin-top: 20px;
        }

        input, select {
            padding: 8px;
            margin: 5px 0;
            width: 100%;
            box-sizing: border-box;
        }

        #order-summary {
            margin-top: 20px;
            background-color: #e8f5e9;
            padding: 15px;
            border-radius: 10px;
            border: 1px solid #c8e6c9;
        }

        #login-section {
            background-color: #ffffff;
            padding: 20px;
            border-radius: 10px;
            max-width: 400px;
            margin: auto;
            text-align: center;
        }

        #login-error {
            color: red;
        }
    </style>
</head>

<body>

<div id="login-section">
    <h2>Login ke ECO PAWS</h2>
    <input type="text" id="username" placeholder="Username"><br>
    <input type="password" id="password" placeholder="Password"><br>
    <button onclick="login()">Login</button>
    <p id="login-error"></p>
<p id="login-error"></p>
    <strong>Gunakan:
    </strong> Username: <code>admin</code>, Password: <code>12345</code></p>

</div>



<div id="main-content" style="display: none;">
    <h1>SELAMAT DATANG DI ECO PAWS CAT!</h1>

    <!-- CONTOH SATU PRODUK -->
    <div class="product">
        <h2>Pasir Kucing Wangi</h2>
        <img src="Pasir-kucing-top-5-liter.jpg" width="100">
        <p>Pasir kucing dengan aroma lavender untuk kenyamanan kucingmu.</p>
        <div class="price">Rp25.000</div>
        <div class="buy-button" onclick="selectProduct('Pasir Kucing Wangi', 25000)">Beli</div>
    </div>

    


<div class="product">
    <h2>Mainan Kucing Interaktif</h2>
    <img src="mianan kucing.jpg" width="100">
    <p>Mainan berbentuk tikus elektrik untuk stimulasi bermain kucing.</p>
    <div class="price">Rp30.000</div>
    <div class="buy-button" onclick="selectProduct('Mainan Kucing Interaktif', 30000)">Beli</div>
</div>

<div class="product">
    <h2>Makanan basah royal canin mother and baby</h2>
    <img src="royal canin mother and baby.jpg" width="100">
    <p>memenuhi kebutuhan nutrisi induk kucing dan anaknya dan dibuat khusus untuk pencernaan anak 
        kucing yang masih sensitif yaitu dengan mengurangi kandungan zat yang sulit dicerna.</p>
    <div class="price">Rp42.000</div>
    <div class="buy-button" onclick="selectProduct('Makanan basah royal canin mother and baby', 42000)">Beli</div>
</div>

<div class="product">
    <h2>Makanan basah royal canin kitten</h2>
    <img src="RC kitten.jpg" width="100">
    <p>mendukung pertumbuhan dan perkembangan dengan memberikan semua zat gizi 
        penting bagi kebutuhan anak kucing dalam tahun pertama kehidupannya.</p>
    <div class="price">Rp20.000</div>
    <div class="buy-button" onclick="selectProduct('Makanan basah royal canin kitten', 20000)">Beli</div>
</div>

<div class="product">
    <h2>gastrointestinal basah</h2>
    <img src="gastro.jpg" width="100">
    <p>Kaya nutrisi dan mudah dicerna, produk gastrointestinal 
        Royal Canin dirancang khusus untuk kucing yang mengalami masalah pencernaan.</p>
    <div class="price">Rp55.000</div>
    <div class="buy-button" onclick="selectProduct('gastrointestinal basah', 55000)">Beli</div>
</div>

<div class="product">
    <h2>royal canin hair and skin</h2>
    <img src="RC hair and skin.jpg" width="100">
    <p>diformulasikan khusus untuk kesehatan dan keindahan kulit 
        dan bulu kucing usia 1 tahun ke-atas.</p>
    <div class="price">Rp78.000</div>
    <div class="buy-button" onclick="selectProduct('royal canin hair and skin', 78000)">Beli</div>
</div>

<div class="product">
    <h2>royal canin persian</h2>
    <img src="RC persian.jpg" width="100">
    <p>makanan kucing yang diformulasikan khusus untuk kucing Persia, baik dewasa maupun anak-anak. </p>
    <div class="price">Rp78.000</div>
    <div class="buy-button" onclick="selectProduct('royal canin persian', 78000)">Beli</div>
</div>

<div class="product">
    <h2>royal canin british short hair</h2>
    <img src="rc bsh.jpg" width="100">
    <p>membantu menjaga massa otot kucing Anda. </p>
    <div class="price">Rp78.000</div>
    <div class="buy-button" onclick="selectProduct('royal canin british short hair', 78000)">Beli</div>
</div>

<div class="product">
    <h2>royal canin urinary</h2>
    <img src="rc urinary.jpg" width="100">
    <p>membantu menjaga kesehatan saluran kemih.</p>
    <div class="price">Rp78.000</div>
    <div class="buy-button" onclick="selectProduct('royal canin urinary', 78000)">Beli</div>
</div>

<div class="product">
    <h2>Makanan Kucing Me-O adult (TUNA)</h2>
    <img src="me o tuna.jpg" width="100">
    <p>Makanan kucing kering berkualitas dengan rasa tuna.</p>
    <div class="price">Rp40.000</div>
    <div class="buy-button" onclick="selectProduct('Makanan Kucing Me-O adult', 40000)">Beli</div>
</div>

<div class="product">
    <h2>Makanan Kucing Me-O adult (SEAFOOD)</h2>
    <img src="seafood adult.jpg" width="100">
    <p>mengandung nutrisi seimbang yang bermanfaat untuk kesehatan mata, sistem imun, gigi, tulang, serta mencegah penyakit saluran kemih. </p>
    <div class="price">Rp40.000</div>
    <div class="buy-button" onclick="selectProduct('Makanan Kucing Me-O', 40000)">Beli</div>
</div>

<div class="product">
    <h2>Makanan Kucing Me-O adult (GOURMET)</h2>
    <img src="GOERMANT ADULT.jpg" width="100">
    <p>meningkatkan sistem imun, memperkuat gigi dan tulang, menjaga mata sehat, mencegah penyakit saluran kencing, serta menjaga kesehatan bulu dan kulit.</p>
    <div class="price">Rp40.000</div>
    <div class="buy-button" onclick="selectProduct('Makanan Kucing Me-O', 40000)">Beli</div>
</div>

<div class="product">
    <h2>Makanan Kucing Me-O adult (OTAK-OTAK)</h2>
    <img src="OTAK OTAK ADULT.JPG" width="100">
    <p>mengandung nutrisi penting untuk kesehatan dan pertumbuhan kucing, seperti protein, omega 3 & 6, dan taurin.</p>
    <div class="price">Rp40.000</div>
    <div class="buy-button" onclick="selectProduct('Makanan Kucing Me-O', 40000)">Beli</div>
</div>


<div class="product">
    <h2>snack me o</h2>
    <img src="snack.jpg" width="100">
    <p>meningkatkan nafsu makan kucing atau dapat digunakan disaat bermain atau melatih kucing</p>
    <div class="price">Rp78.000</div>
    <div class="buy-button" onclick="selectProduct('snack me o', 78000)">Beli</div>
</div>

<div class="product">
    <h2>me o kitten (OCEAN FISH)</h2>
    <img src="me o ocean fish kitten.jpg" width="100">
    <p>untuk kesehatan mata, meningkatkan sistem imunitas tubuh, melindungi gigi dan tulang, mencegah risiko penyakit pada saluran kencing serta meningkatkan kesehatan bulu dan kulit kucing.</p>
    <div class="price">Rp78.000</div>
    <div class="buy-button" onclick="selectProduct('me o kitten ', 78000)">Beli</div>
</div>

<div class="product">
    <h2>ME O kitten (PILCHARD) </h2>
    <img src="PILCHARD ME O - Copy.jpg" width="100">
    <p>makanan kucing lengkap dan bernutrisi seimbang. </p>
    <div class="price">Rp40.000</div>
    <div class="buy-button" onclick="selectProduct('ME O kitten (PILCHARD)', 40000)">Beli</div>
</div>

<div class="product">
    <h2></h2>
    <img src="RC hair and skin.jpg" width="100">
    <p>diformulasikan khusus untuk kesehatan dan keindahan kulit 
        dan bulu kucing usia 1 tahun ke-atas.</p>
    <div class="price">Rp78.000</div>
    <div class="buy-button" onclick="selectProduct('RC hair and skin', 78000)">Beli</div>
</div>

<div class="product">
    <h2>ME O kitten (PESIAN KITTEN) </h2>
    <img src="PERSIAN KITTEN.jpg" width="100">
    <p>berfungsi dalam perkembangan bulu ras persia yang lebat dan panjang, membuat bulu halus dan berkilau, serta baik utk pertumbuhan massa otot & tulang..</p>
    <div class="price">Rp70.000</div>
    <div class="buy-button" onclick="selectProduct('ME O kitten (PESIAN KITTEN)', 70000)">Beli</div>
</div>

<div class="product">
    <h2>whiskas (mackerel) </h2>
    <img src="whiskas-3d-1-1kg-fop-senior-2_1721202295778_1723474584107.png" width="100">
    <p>menyediakan protein berkualitas tinggi yang berasal dari makarel asli, serta nutrien esensial seperti asam lemak omega-3 & 6 dan zink untuk mendukung kesehatan bulu dan kulit.</p>
    <div class="price">Rp55.000</div>
    <div class="buy-button" onclick="selectProduct('whiskas (mackerel)', 55000)">Beli</div>
</div>

<div class="product">
    <h2>cat choize (adult tuna) </h2>
    <img src="tuna800_91b11251-4cdd-4272-b36d-be17c25d062a_700x700.jpg" width="100">
    <p>untuk memenuhi kebutuhan nutrisi harian kucing dewasa, termasuk vitamin, mineral, dan protein, serta membantu menjaga kesehatan gigi, pencernaan, kulit, bulu, dan penglihatan kucing</p>
    <div class="price">Rp30.000</div>
    <div class="buy-button" onclick="selectProduct('cat choize (adult tuna)', 30000)">Beli</div>
</div>


    <!-- TAMBAHKAN PRODUK LAINNYA DI SINI -->

    <!-- Form Pemesanan -->
    <form id="order-form" onsubmit="submitOrder(event)">
        <h2>Form Pemesanan</h2>
        <input type="text" id="nama" placeholder="Nama Anda" required>
        <input type="text" id="produk" readonly>
        <input type="number" id="harga" readonly>
        <input type="number" id="jumlah" placeholder="Jumlah" required>
      <label for="metode">Metode Pembayaran:</label>

<select id="metode" required>
    <option value="">-- Pilih Metode --</option>
    <option value="Transfer Bank">Transfer Bank</option>
    <option value="Dana">Dana</option>
    <option value="OVO">OVO</option>
    <option value="GoPay">GoPay</option>
    <option value="COD">Bayar di Tempat (COD)</option>
</select>

        <button type="submit">Pesan</button>
    </form>

    <!-- Ringkasan Pesanan -->
    <div id="order-summary" style="display:none;"></div>
</div>

<script>
    function login() {
        const user = document.getElementById("username").value;
        const pass = document.getElementById("password").value;
        const error = document.getElementById("login-error");

        // Data login valid
        const validUser = "admin";
        const validPass = "12345";

        if (user === validUser && pass === validPass) {
            document.getElementById("login-section").style.display = "none";
            document.getElementById("main-content").style.display = "block";
        } else {
            error.textContent = "Username atau password salah.";
        }
    }

    function selectProduct(namaProduk, hargaProduk) {
        document.getElementById('produk').value = namaProduk;
        document.getElementById('harga').value = hargaProduk;
        document.getElementById('order-form').style.display = 'block';
        window.scrollTo(0, document.body.scrollHeight);
    }

function submitOrder(event) {
    event.preventDefault();
    const produk = document.getElementById('produk').value;
    const harga = parseInt(document.getElementById('harga').value);
    const nama = document.getElementById('nama').value;
    const jumlah = parseInt(document.getElementById('jumlah').value);
    const metode = document.getElementById('metode').value;
    const total = harga * jumlah;

    // Data nomor pembayaran
    const nomorPembayaran = {
        'Dana': '081372115148',
        'OVO': '081372115148',
        'GoPay': '081372115148',
        'Transfer Bank': '1234567890 (BCA a.n. PetCawss)'
    };

    const nomorTujuan = nomorPembayaran[metode];

    const summary = `
        <h2>Pesanan Berhasil!</h2>
        <p><strong>Nama:</strong> ${nama}</p>
        <p><strong>Produk:</strong> ${produk}</p>
        <p><strong>Jumlah:</strong> ${jumlah}</p>
        <p><strong>Total Harga:</strong> Rp${total.toLocaleString('id-ID')}</p>
        <p><strong>Metode Pembayaran:</strong> ${metode}</p>
        <p><strong>Silakan transfer ke:</strong> ${nomorTujuan}</p>
    `;

    document.getElementById('order-summary').innerHTML = summary;
    document.getElementById('order-summary').style.display = 'block';
    document.getElementById('order-form').reset();
    document.getElementById('order-form').style.display = 'none';
}

</script>

</body>
</html>
