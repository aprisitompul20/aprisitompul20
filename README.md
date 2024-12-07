<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Website bisnis yang profesional dan mudah diakses.">
    <title>Website Bisnis</title>
    <style>
        /* Reset dasar */
        body, h1, h2, p, ul, li {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
        }

        body {
            line-height: 1.6;
            color: #333;
        }

        /* Header */
        header {
            background: #0078D4;
            color: white;
            padding: 1rem 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
        }

        header nav ul {
            list-style: none;
            padding: 0;
        }

        header nav ul li {
            display: inline;
            margin: 0 10px;
        }

        header nav ul li a {
            color: white;
            text-decoration: none;
        }

        /* Section */
        .section {
            padding: 2rem 0;
            background: #f4f4f4;
        }

        .section:nth-child(even) {
            background: white;
        }

        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }

        /* Formulir Kontak */
        form {
            display: flex;
            flex-direction: column;
        }

        form label {
            margin-top: 10px;
        }

        form input, form textarea {
            margin-top: 5px;
            padding: 10px;
            font-size: 1rem;
        }

        form button {
            margin-top: 10px;
            padding: 10px;
            background: #0078D4;
            color: white;
            border: none;
            cursor: pointer;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 1rem 0;
            background: #333;
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Makanan</h1>
            <nav>
                <ul>
                    <li><a href="#about">Tentang Kami</a></li>
                    <li><a href="#services">Layanan</a></li>
                    <li><a href="#contact">Kontak</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="about" class="section">
        <div class="container">
            <h2>Tentang Kami</h2>
            <p>Kami adalah perusahaan yang menyediakan Kuliner makanan terbaik untuk Anda. Kepercayaan dan kesenangan adalah prioritas kami.</p>
        </div>
    </section>

    <section id="services" class="section">
        <div class="container">
            <h2>Layanan Kami</h2>
            <ul>
                <li>Konsultasi Bisnis</li>
                <li>Pengembangan Website</li>
                <li>Strategi Digital Marketing</li>
            </ul>
        </div>
    </section>

    <section id="contact" class="section">
        <div class="container">
            <h2>Hubungi Kami</h2>
            <form id="contactForm">
                <label for="name">Nama:</label>
                <input type="text" id="name" name="name" required>
                
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                
                <label for="message">Pesan:</label>
                <textarea id="message" name="message" rows="4" required></textarea>
                
                <button type="submit">Kirim</button>
            </form>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 Nama Bisnis Anda. Semua Hak Dilindungi.</p>
        </div>
    </footer>

    <script>
        document.getElementById('contactForm').addEventListener('submit', function (e) {
            e.preventDefault();
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const message = document.getElementById('message').value;

            alert(Terima kasih, ${name}! Pesan Anda telah dikirim.);
            this.reset();
        });
    </script>
</body>
</html>
