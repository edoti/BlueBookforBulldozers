Veri Bilimi 101 Notları
📉 RMSE (Root Mean Squared Error – Kök Ortalama Kare Hatası)

Tanım: Gerçek değerle tahmin arasındaki farkların karesinin ortalamasının kareköküdür.

Küçükse: Tahminlerin gerçek değerlere daha yakındır.

Formül: rmse.png

Özelliği: Büyük hataları daha fazla cezalandırır çünkü karesini alır.

🌲 Decision Tree (Karar Ağacı)

Tanım: Verileri dallara ayırarak karar veren bir makine öğrenmesi algoritmasıdır.

Ne işe yarar?: Sınıflandırma (classification) ve regresyon (regression) problemlerinde kullanılır.

Nasıl çalışır?: Veriyi böle böle (if-else gibi) bir ağaç yapısı oluşturur.

Örn: "Eğer yaş < 18 ise → çocuk sınıfı, değilse → yetişkin"

⛰️ Local Optimum (Yerel En İyi) Tanım: Bir modelin eğitim sırasında ulaştığı, çevresine göre en iyi ama globalde en iyi olmayan sonuç noktasıdır.

Problem nedir?: Model bu noktaya "takılabilir", daha iyi bir sonuç potansiyelini kaçırabilir.

Örnek: Dağlık bir arazide küçük bir tepeye tırmandığını düşün; en yüksek nokta orası olmayabilir ama orada durursun.

🧮 RMSLE (Root Mean Squared Logarithmic Error – Kök Ortalama Logaritmik Kare Hatası)

Tanım: RMSE'nin logaritmalı versiyonudur.

Ne zaman kullanılır?: Hedef değişken çok büyük sayılardan oluşuyorsa ve oransal hataları ölçmek istiyorsan.

Avantajı:Küçük farkları fazla önemsemez, büyük değerlerdeki oransal hataları dikkate alır.

📊 R² (R-kare) Nedir?

R² (Determination Coefficient – Belirleme Katsayısı), bir regresyon modelinin tahminlerinin ne kadar başarılı olduğunu ölçen bir metriktir.

✅ Örnek: Diyelim bir ev fiyatı modelin var ve:

Gerçek fiyatlar: [100k, 150k, 200k]

Model tahminleri: [110k, 140k, 195k]

Modelin hatası düşükse, R² → 1'e yaklaşır. Model rastgele sallıyorsa, R² → 0 hatta negatif olur.

Yüksek R² her zaman iyi bir model anlamına gelmez (özellikle aşırı öğrenmede / overfitting).

Kategorik verilerde R² kullanılmaz, sadece regresyonda geçerlidir.

Kategorik ve Eksik Veri Problemi

❓1. Kategorik problem Nedir?

Makine öğrenmesi algoritmaları genellikle sayısal (numeric) verilerle çalışır.

Ama birçok veri kümesinde kategorik sütunlar vardır: örn. cinsiyet = "Erkek", şehir = "Ankara"

⚠️ Problem: Bu tür verileri doğrudan modele verirsen hata alırsın

❓ 2. Eksik Veri Problemi (Missing Data) Nedir?

Verinin bazı hücreleri boş olabilir: örn. yaş, gelir, maaş eksik vs.

⚠️ Problem: Birçok makine öğrenmesi algoritması boş (NaN) değerlerle çalışamaz.

✅ Sonuç Problem Türü Neden Önemli? Ne Yapmalı?

Kategorik Veri Sayıya çevrilmezse model çalışmaz One-hot / Label encoding

Eksik Veri Model çöker ya da yanılır Sil, doldur ya da tahmin et

🔍 Subsample Nedir?

Subsample, genellikle Boosting algoritmalarında (özellikle Gradient Boosting ve XGBoost gibi) kullanılan bir hiperparametredir. Bu parametre, her ağaç oluşturulurken eğitim verisinin ne kadarının kullanılacağını belirler.

subsample genellikle 0.5–1.0 aralığında seçilir.

Çok düşük bir değer (örn. 0.1) modele yetersiz bilgi verir, underfitting yaşanabilir.

Hyperparameters

Bir makine öğrenmesi modelini eğitmeden önce dışarıdan bizim belirlediğimiz ayarlardır. Modelin nasıl öğrenmesini istediğimizi kontrol ederler.

🎲 Random Feature Selection (Rastgele Özellik Seçimi) Nedir?

Random Feature Selection, bir makine öğrenmesi algoritmasının her karar adımında ya da model kurulumunda tüm özellikler yerine rastgele seçilmiş bazı özellikleri kullanmasıdır.

Proje
Veri setine bu linkten ulaşabilirsiniz:

🔗 https://www.kaggle.com/competitions/bluebook-for-bulldozers/data

Veri setini indirebilmek için kaggle hesabınızın "Settings" kısmından "Phone verification" yapmanız gerekmektedir.
Aksi takdirde veri setini indiremezsiniz.
