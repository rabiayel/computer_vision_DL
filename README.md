# Bilgisayarlı Görü & Derin Öğrenme

Veri ön işlemeden sinir ağı eğitimine ve bilgisayarlı görü uygulamalarına kadar temel makine öğrenmesi ve derin öğrenme konularını kapsayan Jupyter notebook koleksiyonu.

---

## Notebook'lar

### 🧠 DeepLearning.ipynb
**Pima Indians Diyabet Veri Seti** kullanılarak tam bağlantılı sinir ağı ile ikili sınıflandırma.

- **Veri Seti:** 768 örnek, 8 özellik (Glukoz, BMI, Yaş vb.), ikili hedef değişken
- **Model:** Sıralı ANN — `giriş → 80 → 120 → 64 → 30 → 8 → 1`
- **Aktivasyonlar:** ReLU (gizli katmanlar), Sigmoid (çıkış)
- **Eğitim:** Adam optimizer, Binary Crossentropy kayıp fonksiyonu, 100 epoch, batch boyutu 32
- **Kütüphaneler:** TensorFlow / Keras, pandas

---

### 👁️ Computer_vision_with_DL.ipynb
Bilgisayarlı görü görevlerine uygulanan derin öğrenme teknikleri.

- **Kütüphaneler:** TensorFlow / Keras
- **Konu:** Sinir ağları ile görüntü işleme ve sınıflandırma

---

### 🔧 DataImputation.ipynb
Eksik veri doldurma yöntemlerinin karşılaştırmalı incelemesi.

| Yöntem | Açıklama |
|---|---|
| Ortalama ile Doldurma | Sütun ortalamasıyla eksik değerleri doldurma |
| KNN ile Doldurma | En yakın komşulardan tahmin etme |
| Yinelemeli / Doğrusal Regresyon | Tahmin modeli tabanlı doldurma |
| MICE | Zincirleme Denklemlerle Çok Değişkenli Doldurma |
| İleri / Geri Doldurma | Pandas yayma yöntemleri |

- **Veri Seti:** `ExampleData.csv` — Boy, Deneyim Yılı, Maaş (kasıtlı NaN değerleri içeren 25 satır)
- **Kütüphaneler:** pandas, scikit-learn, miceforest

---

### 📊 Normalization-PCA.ipynb
Kodlama, ölçekleme ve boyut indirgeme ön işleme hattı.

- **Veri Seti:** `PastHires.csv` — Karma kategorik/sayısal özellikler içeren 13 işe alım kaydı
- **Adımlar:**
  1. Kategorik kodlama (E/H, eğitim seviyeleri → sayısal)
  2. L2 normalizasyonu
  3. Standardizasyon (ortalama merkezleme + varyans ölçekleme)
  4. PCA: 7 özellik → 3 ana bileşen
- **Kütüphaneler:** pandas, scikit-learn (`normalize`, `scale`, `PCA`)

---

## Veri Setleri

| Dosya | Açıklama |
|---|---|
| `pima-indians-diabetes.csv` | Diyabet sınıflandırması için tıbbi veri seti |
| `ExampleData.csv` | Eksik değerler içeren Boy / Deneyim / Maaş verisi |
| `PastHires.csv` | İş geçmişi ve eğitim verisi |
| `kc_house.pkl` | King County konut verisi (serileştirilmiş) |

---

## Kullanılan Teknolojiler

- Python 3
- Jupyter Notebook
- TensorFlow / Keras
- scikit-learn
- pandas
- miceforest

---
