# Curhat-Aja
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pesan Anonim</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }
        .container {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        textarea {
            width: 100%;
            height: 150px;
            padding: 10px;
            margin-bottom: 20px;
            border-radius: 5px;
            border: 1px solid #ccc;
            resize: none;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Kirim Pesan Anonim</h2>
        <textarea id="message" placeholder="Tulis pesanmu di sini..."></textarea>
        <br>
        <button onclick="sendMessage()">Kirim</button>
    </div>

    <script>
        function sendMessage() {
            var message = document.getElementById("message").value;
            if (message.trim() === "") {
                alert("Pesan tidak boleh kosong!");
                return;
            }
            // Simpan pesan atau kirim ke server
            alert("Pesan terkirim: " + message);
            document.getElementById("message").value = ""; // Kosongkan textarea
        }
    </script>
</body>
</html>
