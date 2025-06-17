# 📘 Bluebook for Bulldozers – Regresyon Projesi

Bu proje, Kaggle üzerindeki [Bluebook for Bulldozers](https://www.kaggle.com/competitions/bluebook-for-bulldozers/data) veri seti kullanılarak, ikinci el iş makinelerinin satış fiyatlarının tahmin edilmesini amaçlayan bir regresyon analizidir. Proje boyunca temel veri bilimi kavramları, hata metrikleri ve makine öğrenmesi algoritmaları uygulanmıştır.

---

## 🎯 Proje Amacı

- Eksik ve kategorik verilerle çalışmayı öğrenmek
- Regresyon problemleri için uygun modelleri seçmek
- Model başarısını değerlendirmek için uygun metrikleri kullanmak
- RMSE, RMSLE, R² gibi regresyon metriklerini anlamak
- Decision Tree gibi algoritmaları uygulamak

---

## 📊 Kullanılan Kavramlar

### 🔹 RMSE (Root Mean Squared Error)
Gerçek değer ile tahmin arasındaki farkların karesinin ortalamasının kareköküdür.  
**Özelliği:** Büyük hataları daha fazla cezalandırır.

### 🔹 RMSLE (Root Mean Squared Logarithmic Error)
Tahmin ve gerçek değerlerin logaritmalarının farklarının karesinin ortalamasının kareköküdür.  
**Ne zaman kullanılır?** Değerler çok büyükse ve oransal hata önemliyse tercih edilir.

### 🔹 R² (R-Kare)
Regresyon modelinin başarı oranını gösterir. 1'e yaklaştıkça model daha iyidir.  
**Not:** Kategorik problemler için geçerli değildir.

---

## 🌳 Kullanılan Algoritmalar

### ✅ Decision Tree Regressor
- Veriyi if-else blokları gibi dallara ayırarak öğrenir.
- Hem regresyon hem sınıflandırma problemlerinde kullanılır.
- Aşırı öğrenmeye (overfitting) meyilli olabilir.

---

## 🔧 Veri Ön İşleme

- `SalesID`, `MachineID` gibi tahmin için gereksiz sütunlar çıkarıldı.
- Eksik veriler analiz edilerek dolduruldu veya çıkarıldı.
- Kategorik veriler label encoding veya one-hot encoding ile dönüştürüldü.
- Tarih formatları (örn. `saledate`) zaman bileşenlerine ayrıldı (yıl, ay, gün).

---

## ⚙️ Modelleme Adımları

1. Veriyi Train/Validation/Test olarak böldüm.
2. Decision Tree modelini `max_depth` hiperparametresiyle eğittim.
3. Modeli RMSE ve RMSLE metrikleri ile değerlendirdim.
4. R² skoru ile genel başarıyı inceledim.
5. Kategorik değişken dönüşümleri ve eksik veri stratejileri denedim.

---

## 🧠 Öğrenilenler

| Konsept | Açıklama |
|--------|----------|
| **Subsample** | Her modellemede verinin sadece belli bir oranını kullanarak aşırı öğrenmeyi önlemek |
| **Random Feature Selection** | Her dalda tüm değişkenler yerine rastgele alt küme seçimi |
| **Hyperparameters** | Modelin dış ayarları – kullanıcı tarafından belirlenir (örn. `max_depth`, `n_estimators`) |
| **Local Optimum** | Modelin iyi ama globalde en iyi olmayan noktaya takılması |

---

## 🔗 Veri Setine Erişim

👉 [Bluebook for Bulldozers – Kaggle](https://www.kaggle.com/competitions/bluebook-for-bulldozers/data)

> ⚠️ Not: Kaggle'dan veri indirebilmek için hesabınızdan **Phone Verification** yapmanız gerekmektedir.

---

## 📎 Kullanılan Araçlar

- Python 3.x
- Jupyter Notebook
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## 📈 Devam İçin Öneriler

- XGBoost veya LightGBM ile performansı karşılaştır
- Hiperparametre optimizasyonu için `GridSearchCV` uygula
- Outlier analizi ve veri standardizasyonu ile sonuçları iyileştir

---

## 🗃️ Not Defteri

Bu projede ayrıca aşağıdaki temel kavramlara dair kişisel notlarımı tuttum:

- RMSE, RMSLE, R² açıklamaları
- Decision Tree algoritma mantığı
- Kategorik ve eksik veriyle başa çıkma yolları
- Subsampling ve rastgele özellik seçimi gibi teknikler

---

