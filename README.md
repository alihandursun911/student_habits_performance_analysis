# IST3031 Regresyon Çözümlemesi: Student's Habits Performance Analysis

Bu proje, öğrencilerin alışkanlıklarının sınav başarıları üzerindeki etkisini inceleyen kapsamlı bir istatistiksel analiz çalışmasıdır. 

---

## 👥 Proje Ekibi
* **Süleyman Rubar Oral**
* **Ali Han Dursun**
* **Çağan Arın Gürsu** 
* **Gökhan Engör**

---

## 📊 Veri Seti Özeti
* **Gözlem Sayısı:** 1000 adet 
* **Değişken Sayısı:** 15 (9 sayısal, 6 kategorik) 
* **Kritik Bulgular:** Günlük çalışma saati ile sınav puanı arasında **0.83** değerinde çok güçlü bir pozitif korelasyon tespit edilmiştir.

---

## 🛠️ Metodoloji ve Model Performansı
Analiz sürecinde **OLS (En Küçük Kareler)** yöntemi kullanılmış; 
Tam Model, Stepwise Selection ve Best Subset Analysis yöntemleri karşılaştırılmıştır.

### Model Sonuçları
* **R-Kare ($R^2$):** 0.901 
* **Düzeltilmiş R-Kare:** 0.900 
* **Test Seti Hata Payı (RMSE):** 5.5024 
* **F-İstatistiği:** 1291.0 (p-value: 0.00) 

---

## 🔍 İstatistiksel Tanılar ve Varsayım Kontrolleri
Projenin en güçlü yanı, model varsayımlarının titizlikle test edilmiş olmasıdır:

1. **Aykırı Değer Analizi:** Cook's Distance yöntemiyle 41 adet etkin gözlem tespit edilmiştir.
2. **Normallik:** Shapiro-Wilk testi ile hataların normal dağılımı kontrol edilmiştir. Aykırı değerler temizlendikten sonra normallik varsayımı sağlanmıştır ($p=0.4016$).
3. **Varyans Homojenliği:** Breusch-Pagan testi sonucunda varyansın homojen olduğu doğrulanmıştır ($p=0.5697$).
4. **Bağımsızlık:** Durbin-Watson değeri **1.96** olarak hesaplanmış ve otokorelasyon olmadığı saptanmıştır.

---

## 📚 Kaynakça
* Montgomery, D. C., Peck, E. A., & Vining, G. G. (2013). Doğrusal regresyon analizine giriş.
* Gamgam, H., & Altunkaynak, B. (2015). Regresyon Analizi.
