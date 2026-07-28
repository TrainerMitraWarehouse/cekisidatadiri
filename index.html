<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cek Data Onboarding Peserta</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f6f9;
            margin: 0;
            padding: 15px;
            color: #333;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        h2 {
            font-size: 1.25rem;
            text-align: center;
            color: #007bff;
            margin-top: 0;
        }
        .search-box {
            display: flex;
            gap: 8px;
            margin-bottom: 20px;
        }
        input[type="text"] {
            flex: 1;
            padding: 10px;
            font-size: 1rem;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        button {
            padding: 10px 15px;
            font-size: 1rem;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:active {
            background-color: #0056b3;
        }
        .card {
            background: #fff;
            border: 1px solid #ddd;
            border-left: 5px solid #28a745;
            padding: 12px;
            margin-bottom: 10px;
            border-radius: 4px;
            font-size: 0.9rem;
        }
        .card p {
            margin: 6px 0;
        }
        .loading, .no-result {
            text-align: center;
            color: #666;
            font-style: italic;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Cek Data Onboarding</h2>
    <div class="search-box">
        <input type="text" id="searchInput" placeholder="Ketik Nama / Email peserta...">
        <button onclick="cariData()">Cari</button>
    </div>

    <div id="resultContainer">
        <p class="loading">Masukkan nama peserta untuk mulai mengecek.</p>
    </div>
</div>

<script>
    // MASUKKAN URL WEB APP GOOGLE SCRIPT KAMU DI SINI
    const WEB_APP_URL = "https://script.google.com/macros/s/AKfycbzwQBFixw3elichTUZ1dxDhn4-FanJPIGdFSsXB-PI6XQBU1uhjvgPzc6_QRXhkhUTE/exec";

    // Agar bisa cari otomatis saat tekan "Enter"
    document.getElementById("searchInput").addEventListener("keypress", function(event) {
        if (event.key === "Enter") {
            cariData();
        }
    });

    function cariData() {
        const query = document.getElementById("searchInput").value.trim();
        const container = document.getElementById("resultContainer");
        
        container.innerHTML = `<p class="loading">Sedang mencari data...</p>`;

        fetch(`${WEB_APP_URL}?q=${encodeURIComponent(query)}`)
            .then(response => response.json())
            .then(data => {
                container.innerHTML = "";
                
                if (data.length === 0) {
                    container.innerHTML = `<p class="no-result">Data peserta tidak ditemukan.</p>`;
                    return;
                }

                data.forEach(item => {
                    let card = document.createElement("div");
                    card.className = "card";
                    
                    let contentHTML = "";
                    // Menampilkan semua kolom secara dinamis dari Google Sheet
                    for (let key in item) {
                        contentHTML += `<p><strong>${key}:</strong> ${item[key]}</p>`;
                    }
                    
                    card.innerHTML = contentHTML;
                    container.appendChild(card);
                });
            })
            .catch(error => {
                console.error("Error:", error);
                container.innerHTML = `<p class="no-result" style="color:red;">Gagal memuat data. Coba lagi.</p>`;
            });
    }
</script>

</body>
</html>
