# P9-API-Integration-23104040205

Project ini adalah implementasi **Backend Node.js Modular** untuk Praktikum #9 mata kuliah Web Service Engineering. Proyek ini mengintegrasikan dua API eksternal (REST Countries & OpenWeatherMap) dengan penerapan Caching, Logging, dan Dokumentasi Swagger.

## 👤 Author
* **Name:** Hujan (Rain) Ivan Dwika Bagaskara
* **NIM:** 23104040205
* **Role:** IT Student

## 🚀 Fitur Utama
1.  **Arsitektur Modular:** Pemisahan logic yang jelas (Routes, Controllers, Services, Utils).
2.  **Integrasi API Eksternal:**
    * [REST Countries](https://restcountries.com/): Data negara.
    * [OpenWeatherMap](https://openweathermap.org/): Data cuaca realtime.
3.  **Caching (NodeCache):** Mengurangi request berulang ke API eksternal untuk performa lebih cepat.
4.  **Logging (Morgan):** Mencatat setiap aktivitas request di terminal.
5.  **Dokumentasi API (Swagger UI):** Antarmuka interaktif untuk testing endpoint.
6.  **Error Handling:** Penanganan error terpusat yang rapi.

## 🛠️ Teknologi yang Digunakan
* Node.js & Express.js
* Axios (HTTP Client)
* Node-Cache (Caching Strategy)
* Morgan (Logger)
* Swagger UI Express (API Documentation)
* Dotenv (Environment Variables)

## 📦 Cara Install & Menjalankan

1.  **Clone Repository**
    ```bash
    git clone [https://github.com/Rainyday404/P9-API-Integration-23104040205.git](https://github.com/Rainyday404/P9-API-Integration-23104040205.git)
    cd P9-API-Integration-23104040205
    ```

2.  **Install Dependencies**
    ```bash
    npm install
    ```

3.  **Konfigurasi Environment Variable**
    Buat file `.env` di root folder dan isi dengan API Key OpenWeatherMap Anda:
    ```env
    PORT=3000
    OWM_API_KEY=masukkan_api_key_anda_disini
    ```

4.  **Jalankan Server**
    ```bash
    npm start
    ```

## 🔗 Dokumentasi API
Setelah server berjalan, buka browser dan akses:
`http://localhost:3000/docs`

## 🧪 Endpoint Tersedia
| Method | Endpoint | Deskripsi |
| :--- | :--- | :--- |
| `GET` | `/api/countries` | Ambil semua negara |
| `GET` | `/api/countries/region/:region` | Ambil negara berdasarkan region (ex: asia) |
| `GET` | `/api/countries/name/:name` | Cari negara spesifik (ex: indonesia) |
| `GET` | `/api/weather?city=NamaKota` | Cek cuaca kota (Default: Palangkaraya) |

---
**Note:** Pastikan Anda memiliki API Key OpenWeatherMap yang aktif agar fitur cuaca berfungsi.
