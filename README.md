# 🍕 Pizza Sales Analysis

Proyek ini menganalisis data penjualan pizza untuk menemukan insight bisnis, tren penjualan, serta peluang promosi berdasarkan pola pemesanan. Data ini diambil dari Kaggle (terima kasih kepada [shilongzhuang](https://www.kaggle.com/datasets/shilongzhuang/pizza-sales)).

## 📊 Tujuan Proyek

Tujuan dari analisis ini adalah:  

- Mengeksplorasi tren penjualan berdasarkan kategori, ukuran, dan waktu  
- Menemukan pola waktu penjualan tertinggi (jam dan hari)  
- Mengidentifikasi pizza terpopuler  
- Melakukan *market basket analysis* (apriori) untuk melihat kombinasi menu yang sering dipesan bersama  
- Memberikan rekomendasi bisnis berbasis data  
- Mengeksplorasi potensi penerapan AI (seperti IBM Granite) untuk insight tambahan dan summarization

Dengan insight ini, bisnis dapat mengoptimalkan strategi promosi, memperbaiki pengelolaan stok, dan merancang menu bundling yang menarik.

---

## 📁 Dataset

Dataset dapat diunduh di [Kaggle - Pizza Sales](https://www.kaggle.com/datasets/shilongzhuang/pizza-sales).

**Dataset memiliki 12 fitur utama:**  

| Fitur              | Deskripsi |
|---------------------|-----------|
| `order_id`          | ID unik untuk setiap transaksi meja |
| `order_details_id`  | ID unik untuk setiap pizza di dalam satu order (pizzas dengan tipe/ukuran sama disatukan di baris yang sama, quantity bertambah) |
| `pizza_id`          | ID unik pizza berdasarkan detail ukuran dan harga |
| `quantity`          | Jumlah pizza yang dipesan |
| `order_date`        | Tanggal pesanan dicatat |
| `order_time`        | Waktu pesanan dicatat |
| `unit_price`        | Harga satuan pizza dalam USD |
| `total_price`       | Harga total (unit_price × quantity) |
| `pizza_size`        | Ukuran pizza (S, M, L, XL, XXL) |
| `pizza_type`        | Tipe pizza unik berdasarkan bahan & resep |
| `pizza_ingredients` | Daftar bahan pizza (Mozzarella Cheese selalu ada, Tomato Sauce kecuali jika tercantum saus lain) |
| `pizza_name`        | Nama menu pizza sesuai di daftar menu restoran |

---

## 🔍 Hasil Analisis Singkat

- **Total revenue** sekitar **$817,860.05**  
- **Pizza paling populer:** The Classic Deluxe Pizza  
- **Kategori terlaris:** Classic  
- **Ukuran paling sering dipesan:** L  
- **Puncak penjualan jam:** 12 siang  
- **Hari tersibuk:** Jumat  
- **Pola kombinasi menu:** Terdeteksi banyak pelanggan memesan beberapa pizza premium bersama, cocok dibuatkan promosi bundling  

---

## 💡 Rekomendasi Bisnis

- Fokus promosi di jam 12 siang, terutama hari Jumat  
- Buat bundling menu berdasarkan kombinasi pizza terpopuler (hasil market basket analysis)  
- Kembangkan variasi baru di kategori Classic, ukuran L  
- Manfaatkan insight AI (seperti summarization dari IBM Granite) untuk laporan manajemen

---

## ⚙️ Struktur Project

```plaintext
pizza-sales-analysis/
│
├── data/
│   └── pizza_sales.xlsx
│
├── images/
│   └── wordcloud.png (opsional)
│
├── pizza_sales_analysis.ipynb
├── README.md
└── requirements.txt
```

---

## 🚀 Jalankan Sendiri

1. Pastikan Anda sudah menginstall:
   - pandas
   - matplotlib
   - mlxtend
   - langchain
   - replicate (opsional, jika mencoba Granite AI)

2. Clone repo ini:
```bash
git clone https://github.com/IqbalIbrahim112/pizza-sales-analysis.git
```

3. Buka notebook:
   Anda bisa membuka file **pizza_sales_analysis.ipynb** menggunakan:
   - Jupyter Notebook / JupyterLab
   - Google Colab (upload manual atau gunakan badge Colab jika ada)

4. Jalankan seluruh sel untuk mereproduksi analisis.

---

## ✉️ Kontak

Jika ada pertanyaan atau masukan, silakan hubungi:
- **Iqbal Triwicaksono Ibrahim**
- [GitHub Profile](https://github.com/IqbalIbrahim112)

---
