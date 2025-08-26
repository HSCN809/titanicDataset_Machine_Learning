# 🚢 Titanic Hayatta Kalma Tahmini - Makine Öğrenmesi Modeli

Bu proje, **Titanic yolcularının hayatta kalma olasılığını** tahmin etmek için geliştirilmiş kapsamlı bir **Makine Öğrenmesi** uygulamasıdır. Projede **veri ön işleme**, **özellik mühendisliği**, **farklı sınıflandırma algoritmalarının karşılaştırılması**, **cross-validation analizi**, **hiperparametre optimizasyonu** ve **interaktif tahmin sistemi** yer almaktadır. Kullanıcı, isterse kendi bilgilerini girerek Titanic’te hayatta kalıp kalamayacağını model üzerinden test edebilir.  

---

## 📂 İçerik
- Veri yükleme, inceleme ve eksik değer işlemleri  
- One-Hot Encoding ve **family_size** gibi yeni özellik oluşturma  
- Eğitim/Test ayrımı ve **StandardScaler** ile ölçekleme  
- Farklı sınıflandırma algoritmaları:  
  - Lojistik Regresyon  
  - Random Forest  
  - Karar Ağacı  
  - K-En Yakın Komşu (KNN)  
  - Naive Bayes  
  - Destek Vektör Makinesi (SVM)  
- Cross Validation ile model karşılaştırması  
- Overfitting/Underfitting analizi  
- Hiperparametre optimizasyonu (**GridSearchCV**)  
- Confusion Matrix ve detaylı sınıflandırma raporu  
- Korelasyon analizi ve heatmap görselleştirmesi  
- Özellik önemleri (Lojistik Regresyon katsayıları)  
- **Interaktif tahmin sistemi** (konsol üzerinden oyun formatında)  

---

## requirements.txt içeriği:
pandas
numpy
matplotlib
seaborn
scikit-learn

---

## Program çalıştırıldığında şu akış gerçekleşir:
1. Titanic veri seti yüklenir ve temizlenir.
2. Farklı ML algoritmaları denenir, doğruluk oranları karşılaştırılır.
3. Cross Validation ve hiperparametre optimizasyonu yapılır.
4. En iyi model seçilir ve test edilir.
5. Kullanıcıya “Titanic tahmin oyunu oynamak ister misiniz?” sorusu sorulur.
- Hayır (H) cevabı → Program kapanır.
- Evet (E) cevabı → Kullanıcı kendi bilgilerini girerek (yaş, cinsiyet, sınıf, bilet ücreti vb.) hayatta kalma ihtimalini öğrenir.

---

🎮 Interaktif Tahmin Sistemi

Örnek giriş senaryosu:

--- Lütfen bilgilerinizi giriniz ---
- Bilet Sınıfı (1=Birinci sınıf, 2=İkinci sınıf, 3=Üçüncü sınıf): 3
- Yaşınız: 22
- Gemideki kardeş/eş sayısı: 1
- Gemideki ebeveyn/çocuk sayısı: 0
- Bilet ücreti (dolar): 7.25
- Cinsiyetiniz (E/erkek veya K/kadın): E
- Bindiği liman: 3 (Southampton)


Model çıktısı örneği:

🚢 TİTANİC HAYATTA KALMA TAHMİNİ
Model: Random Forest
Model Doğruluğu: 83.1%

📊 Tahmin Sonuçları:
Hayatta Kalma Şansı: %12.4
Ölüm Riski: %87.6

❌ TAHMİN: HAYATTA KALAMAZSINIZ
😰 Yüksek risk altındasınız.

---
