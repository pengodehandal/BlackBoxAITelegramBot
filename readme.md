# BlackBox AI Telegram Bot

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)

Bot Telegram asisten AI cerdas yang ditenagai oleh API eksternal. Bot ini mampu merespons pesan pengguna secara dinamis dan mencatat semua interaksi di konsol untuk pemantauan.

## ✨ Fitur

-   **Asisten AI**: Menjawab pesan pengguna dengan respons yang dihasilkan oleh AI.
-   **Setup Mudah**: Proses pengaturan awal melalui konsol untuk memasukkan Token Bot dan Nama Bot.
-   **Simpan Konfigurasi**: Token dan Nama Bot disimpan dalam file `config_ai_bot.json`, jadi Anda tidak perlu memasukkannya setiap kali menjalankan.
-   **Logging Aktivitas**: Setiap pesan yang masuk dan balasan dari bot akan dicatat di konsol, lengkap dengan stempel waktu dan detail pengguna.
-   **Multi-platform**: Dapat dijalankan di Windows, Linux (Ubuntu), dan macOS.

## 📋 Prasyarat

Sebelum memulai, pastikan Anda memiliki:

1.  **Python 3.8 atau lebih baru**.
2.  **Token Bot Telegram**. Jika belum punya, Anda bisa mendapatkannya dari [@BotFather](https://t.me/BotFather) di Telegram dengan mengikuti langkah-langkah berikut:
    -   Kirim `/newbot` ke BotFather.
    -   Ikuti petunjuk untuk memberi nama dan username pada bot Anda.
    -   BotFather akan memberikan Anda sebuah **token API**. Simpan token ini baik-baik.

---

## 🚀 Instalasi dan Penggunaan

Berikut adalah cara menginstal dan menjalankan bot ini di sistem operasi yang berbeda.

### 🖥️ Untuk Pengguna Windows

**1. Instal Python dan Git**
   - Kunjungi [python.org](https://www.python.org/downloads/) dan unduh installer Python terbaru. Saat instalasi, **pastikan Anda mencentang kotak "Add Python to PATH"**.
   - Kunjungi [git-scm.com](https://git-scm.com/download/win) dan unduh Git.

**2. Clone Repositori**
   Buka **Command Prompt** atau **PowerShell** dan jalankan perintah berikut:
   ```bash
   git clone [https://github.com/pengodehandal/BlackBoxAITelegramBot.git](https://github.com/pengodehandal/BlackBoxAITelegramBot.git)
   cd BlackBoxAITelegramBot
   ```

**3. Buat Virtual Environment**
   Sangat disarankan untuk menggunakan virtual environment agar dependensi proyek tidak tercampur.
   ```bash
   python -m venv venv
   .\venv\Scripts\activate
   ```
   Nama terminal Anda sekarang seharusnya diawali dengan `(venv)`.

**4. Instal Dependensi**
   Instal semua library yang dibutuhkan dari file `requirements.txt`.
   ```bash
   pip install -r requirements.txt
   ```

**5. Jalankan Bot**
   ```bash
   python gpt.py
   ```
   - **Pada saat pertama kali menjalankan**: Skrip akan meminta Anda memasukkan **Token Bot** dan **Nama untuk Asisten AI Anda**.
   - **Setelah itu**: Konfigurasi akan tersimpan, dan bot akan langsung berjalan. Semua aktivitas akan tercatat di konsol.

---

### 🐧 Untuk Pengguna Ubuntu

**1. Instal Python, Pip, Venv, dan Git**
   Buka Terminal dan jalankan perintah berikut:
   ```bash
   sudo apt update
   sudo apt install python3 python3-pip python3-venv git -y
   ```

**2. Clone Repositori**
   ```bash
   git clone [https://github.com/pengodehandal/BlackBoxAITelegramBot.git](https://github.com/pengodehandal/BlackBoxAITelegramBot.git)
   cd BlackBoxAITelegramBot
   ```

**3. Buat Virtual Environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
   Nama terminal Anda sekarang seharusnya diawali dengan `(venv)`.

**4. Instal Dependensi**
   Instal semua library yang dibutuhkan.
   ```bash
   pip install -r requirements.txt
   ```

**5. Jalankan Bot**
   ```bash
   python3 gpt.py
   ```
   - **Pada saat pertama kali menjalankan**: Anda akan diminta memasukkan **Token Bot** dan **Nama untuk Asisten AI**.
   - **Untuk selanjutnya**: Bot akan berjalan otomatis menggunakan konfigurasi yang tersimpan.

## 📁 Struktur File

```
.
├── .gitignore         # Mengabaikan file yang tidak perlu di-upload
├── gpt.py             # Kode utama bot
├── requirements.txt   # Daftar dependensi Python
└── README.md          # File yang sedang Anda baca
```

Setelah bot dijalankan pertama kali, file `config_ai_bot.json` akan dibuat secara otomatis untuk menyimpan kredensial Anda.
