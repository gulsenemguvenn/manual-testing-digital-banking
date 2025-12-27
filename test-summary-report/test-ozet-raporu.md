# Test Özet Raporu – Dijital Bankacılık Manuel Test Çalışması

---

## 1️⃣ Amaç

Bu rapor, dijital bankacılık uygulaması için gerçekleştirilen
manuel test çalışmalarının özetini ve test sonuçlarına göre
değerlendirmeyi sunmak amacıyla hazırlanmıştır.

---

## 2️⃣ Test Kapsamı

Manuel test kapsamına alınan modüller:

- Giriş (Login)
- Hesap Görüntüleme
- Para Transferi
- İşlem Geçmişi

---

## 3️⃣ Test Yaklaşımı

Test çalışmaları sırasında:

- Risk analizi baz alınarak **kritik modüllere öncelik** verilmiştir.
- Pozitif, negatif ve **edge case** test senaryoları uygulanmıştır.
- Tespit edilen hatalar standart **hata raporu formatında** dokümante edilmiştir.

---

## 4️⃣ Test Sonuçları (Özet)

| Modül             | Toplam Test | Başarılı | Başarısız |
|-------------------|-------------|----------|-----------|
| Giriş (Login)     | 10          | 9        | 1         |
| Hesap Görüntüleme | 8           | 8        | 0         |
| Para Transferi    | 15          | 13       | 2         |
| İşlem Geçmişi     | 8           | 8        | 0         |
| **TOPLAM**        | **41**      | **38**   | **3**     |

---

## 5️⃣ Bulunan Hatalar

- Yetersiz bakiye kontrolünün bazı senaryolarda atlandığı gözlemlenmiştir.
- Günlük transfer limiti sınır değerlerinde beklenen davranış net değildir.

---

## 6️⃣ Yayına Çıkış Değerlendirmesi

Mevcut test sonuçlarına göre:

❌ **Kritik hatalar giderilmeden yayına çıkılması önerilmemektedir.**  
🔁 Düzeltmeler sonrası regresyon testlerinin tekrar çalıştırılması gerekmektedir.
