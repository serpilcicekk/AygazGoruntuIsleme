# AygazGoruntuIsleme

# Aygaz Görüntü İşleme Bootcamp Projesi

## Proje Amacı
Bu proje, **Convolutional Neural Network (CNN)** kullanarak 10 farklı hayvan sınıfını sınıflandırmayı hedeflemektedir. Ayrıca, modelin manipüle edilmiş test seti ve renk sabitliği algoritması uygulanmış görseller üzerindeki dayanıklılığı test edilmiştir.

## Proje İçeriği
- **Veri Seti:** [Animals with Attributes 2 (AwA2)](https://www.kaggle.com/datasets/rrebirrth/animals-with-attributes-2) veri seti kullanılmıştır.
- **Sınıflar:** Aşağıdaki 10 hayvan sınıfı seçilmiştir:
  - `collie, dolphin, elephant, fox, moose, rabbit, sheep, squirrel, giant panda, polar bear`

- **Proje Adımları:**
  1. Veri setinin hazırlanması (boyutlandırma, normalizasyon, sınıf dengesi).
  2. CNN modelinin tasarlanması ve eğitilmesi.
  3. Modelin orijinal test seti üzerinde doğruluk değerlendirmesi.
  4. Manipüle edilmiş görsellerle model dayanıklılığının ölçülmesi.
  5. Renk sabitliği algoritması uygulanmış test seti ile model performansı.

## Kullanılan Teknolojiler ve Kütüphaneler
- **Python**
- **TensorFlow/Keras** (Derin öğrenme için)
- **OpenCV** (Görüntü işleme)
- **Scikit-learn** (Veri ayrımı ve etiketleme)
- **Matplotlib** (Görselleştirme)

## Proje Yapısı
```plaintext
📂 proje-dizini/
├── 📁 datasets/
│   ├── collie/
│   ├── dolphin/
│   └── ... (diğer hayvan sınıfları)
├── 📄 main.ipynb (Projenin Jupyter Notebook dosyası)
├── 📄 README.md (Proje açıklamaları)
└── 📄 requirements.txt (Gerekli kütüphaneler)



---

## Sonuç Raporu

**Başarıların Karşılaştırılması**

| Test Durumu                  | Test Doğruluğu (%) | Kaybedilen Performans |
|------------------------------|--------------------|------------------------|
| Orijinal Test Seti           | 66.82             | -                      |
| Manipüle Edilmiş Test Seti   | 9.74              | -57.08                |
| Renk Sabitliği Uygulanmış    | 63.28             | -3.54                 |

**Analiz ve Yorum**
1. **Orijinal Test Seti:**
   - Model, orijinal test setinde %66.82 doğruluk oranına ulaşarak temel bir başarı sergilemiştir.
2. **Manipüle Edilmiş Test Seti:**
   - Manipülasyon işlemleri model doğruluğunu ciddi ölçüde düşürmüştür. Bu, modelin manipüle edilmiş verilere karşı genelleme kapasitesinin yetersiz olduğunu göstermektedir.
3. **Renk Sabitliği Uygulanmış Test Seti:**
   - Renk sabitliği algoritması, modelin manipüle edilmiş verilere karşı doğruluğunu önemli ölçüde artırmıştır. Bu, algoritmanın veri manipülasyonlarına dayanıklılığı artırabileceğini göstermektedir.

**Öneriler**
- **Manipüle Edilmiş Veriler İçin:** Eğitim setine manipüle edilmiş veri artırma teknikleri eklenmelidir.
- **Renk Sabitliği Algoritması:** Eğitim verilerine renk sabitliği algoritması uygulanarak model dayanıklılığı artırılabilir.
- **Daha Karmaşık Modeller:** Daha karmaşık mimariler (ör. ResNet, EfficientNet) kullanılarak doğruluk oranı artırılabilir.

---

Kaggle Link : https://www.kaggle.com/code/serpiliek/aygazbootcamp
