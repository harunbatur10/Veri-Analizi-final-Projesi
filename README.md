Kredi Kartı Dolandırıcılık Tespiti (Credit Card Fraud Detection)

Bu proje, veri analizi dersi kapsamında hazırlanmış bir makine öğrenmesi projesidir. Projenin amacı, sentetik bir veri seti kullanarak kredi kartı işlemlerinin dolandırıcılık (fraud) olup olmadığını tespit etmektir.

Veri Seti
Kaggle'dan temin edilen `synthetic_fraud_dataset.csv` kullanılmıştır.
- Satır Sayısı: 10.000
- Problem Türü:Sınıflandırma (Classification)
- Hedef Değişken:`is_fraud` (0: Normal, 1: Dolandırıcılık)

Kullanılan Yöntemler
Proje şu adımları içermektedir:
1. Veri Keşfi (EDA):** Eksik veri analizi, sınıf dağılımı incelemesi ve görselleştirme.
2. Ön İşleme:** Gereksiz sütunların (ID vb.) atılması, One-Hot Encoding uygulanması.
3. Modelleme:** Random Forest Classifier algoritması kullanılmıştır.
4. Değerlendirme:** Accuracy, Confusion Matrix ve F1-Score metrikleri ile model başarısı ölçülmüştür.

Sonuçlar
Model, test veri seti üzerinde %100 doğruluk (Accuracy) oranına ulaşmıştır. Sentetik veri setinin belirgin yapısı nedeniyle model, dolandırıcılık işlemlerini (Fraud) hatasız ayırt edebilmiştir.
- En Önemli Özellik:İşlem Tutarı (Amount) ve Cihaz Risk Skoru.

Kurulum ve Çalıştırma
Gerekli kütüphaneler: pandas, numpy, seaborn, matplotlib, sklearn
Proje dosyasını (`.ipynb`) indirerek Jupyter Notebook veya Google Colab üzerinde çalıştırabilirsiniz.
