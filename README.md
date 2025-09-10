# 📊 Tableau Embed Playground

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![Made with HTML](https://img.shields.io/badge/Made%20with-HTML-orange)
![Made with JS](https://img.shields.io/badge/Made%20with-JavaScript-yellow)
![TailwindCSS](https://img.shields.io/badge/Styled%20with-TailwindCSS-38B2AC?logo=tailwindcss)
[![Open in Browser](https://img.shields.io/badge/Open-Index.html-green)](./index.html)

Tableau Embed Playground adalah sebuah **web tool sederhana** untuk:
- Membuat **JWT Token** menggunakan Connected App Secret.
- Menguji coba embed **Tableau Views / Dashboards** secara langsung di browser.

Project ini cocok untuk developer yang ingin memahami alur **Tableau Connected Apps + JWT + Embed API v3**.

---

## 🚀 Fitur

- [x] Generate JWT Token secara langsung di browser menggunakan **jsrsasign**.
- [x] Mode **Generate Token** (pakai secret langsung) atau **I have a Token** (pakai token hasil generate dari backend).
- [x] Embed **Tableau View** menggunakan `<tableau-viz>` (Embed API v3).
- [x] Copy token sekali klik.
- [x] UI responsive sederhana dengan **TailwindCSS**.
- [x] Footer link ke GitHub author.

---

## 🛠️ Teknologi

- **HTML + TailwindCSS** (UI/Styling).
- **JavaScript**.
- **[jsrsasign](https://github.com/kjur/jsrsasign)** untuk generate JWT.
- **Tableau Embedding API v3**.

---

## 📂 Struktur Project

```

index.html        # Halaman utama
README.md         # Dokumentasi

````

---

## 📖 Cara Menggunakan

1. Clone repository:
   ```bash
   git clone https://github.com/misterdevs/tableau-embed-playground.git
   cd tableau-embed-playground

2. Buka langsung `index.html` di browser (tidak perlu server tambahan).

3. Pilih mode:

   * **Generate Token** → masukkan Tableau User, Client ID, Secret ID, Secret Value, Scope, Embed URL → klik **Generate**.
   * **I have a Token** → masukkan Embed URL dan Token yang sudah ada → klik **Try Now**.

4. Jika berhasil, Tableau View akan muncul di area embed.

---

## ⚠️ Catatan Penting

* **Jangan gunakan secret asli di public repo / environment browser** ⚠️.
  Playground ini hanya untuk **eksperimen & pembelajaran**.
  Untuk production, selalu generate JWT di server (backend), bukan di frontend.

* Token yang di-generate hanya berlaku sebentar (`exp = 5 menit`).

---

## 📌 Referensi

* [Tableau Embedding API v3](https://help.tableau.com/current/api/embedding_api/en-us/index.html)
* [Connected Apps - Tableau](https://help.tableau.com/current/server/en-us/security_connected_apps.htm)
* [jsrsasign](https://kjur.github.io/jsrsasign/)

---

## 👨‍💻 Author

Made with ❤️ by [Misterdevs](https://github.com/misterdevs)
