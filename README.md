# Hybrid (HB) Segment Raporu

Aylık müşteri portföyü CSV'lerinden (`YYYYMM.csv`) tek dosyalık, paylaşılabilir HTML rapor üreten Jupyter notebook.

## Kullanım
1. `hybrid_rapor.ipynb` dosyasını Jupyter'de açın.
2. **Ayarlar** hücresinde `VERI_KAYNAGI = "csv"` ve `VERI_KLASORU = "klasör_yolu"` yazın (klasörde `202603.csv`, `202604.csv` … bulunmalı).
3. **Run All** → `hybrid_rapor.html` oluşur (internetsiz açılır, e-postayla paylaşılabilir).
4. "Veri doğrulama" çıktısını kontrol edin (eksik kolonlar, cinsiyet/cihaz kolonu eşleşmesi, hareket adetleri).

Gerekli paketler: `numpy`, `pandas` (ve internetsiz HTML için `plotly`). Denemek için `VERI_KAYNAGI = "sentetik"` bırakın.

Kolon adları farklıysa Ayarlar hücresindeki `CINSIYET_KOLONU`, `CIHAZ_KOLONU`, `YAS_KOLONU`, `AKTIF_DURUM_IDS`, `SOZLESME_ISIM` vb. değerleri düzenleyin.
