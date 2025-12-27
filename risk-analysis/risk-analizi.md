#  Risk Analizi – Dijital Bankacılık
*(Etki & Olasılık Bazlı)*

Bu doküman, dijital bankacılık uygulamasındaki
**en kritik iş alanlarını** belirlemek ve
manuel test çalışmalarını **önceliklendirmek**
amacıyla hazırlanmıştır.

---

##  Amaç

Bankacılık uygulamalarında özellikle
**para transferi** ve **giriş (login)** akışları
yüksek iş riski taşımaktadır.

Bu analiz ile:
- Kritik fonksiyonlar belirlenmiş
- Risk seviyelerine göre test öncelikleri oluşturulmuştur

---

##  Risk Değerlendirme Ölçeği

- **Etki (1–5):** Hata oluştuğunda kullanıcı / iş üzerindeki etki
- **Olasılık (1–5):** Hatanın gerçekleşme ihtimali
- **Risk Skoru:** Etki × Olasılık
- **Öncelik:** Yüksek / Orta / Düşük

---

##  Risk Matrisi

| Modül / Alan        | Risk Tanımı                                           | Etki | Olasılık | Skor | Öncelik |
|---------------------|--------------------------------------------------------|------|----------|------|----------|
| Para Transferi      | Yanlış alıcıya / yanlış tutarla transfer               | 5    | 3        | 15   | Yüksek   |
| Para Transferi      | Günlük transfer limitinin uygulanmaması                | 5    | 3        | 15   | Yüksek   |
| Para Transferi      | Yetersiz bakiye varken transfer yapılabilmesi           | 5    | 2        | 10   | Yüksek   |
| Para Transferi      | Geçersiz IBAN kontrolünün yapılmaması                   | 4    | 3        | 12   | Yüksek   |
| Giriş (Login)       | Hatalı denemelerde hesap kilitlemenin çalışmaması       | 4    | 3        | 12   | Yüksek   |
| Hesap Görüntüleme   | Toplam bakiyenin yanlış hesaplanması                    | 4    | 2        | 8    | Orta     |
| İşlem Geçmişi       | Başarılı transferin geçmişte görünmemesi                | 3    | 2        | 6    | Orta     |

---

##  Test Önceliklendirme Stratejisi

###  Yüksek Öncelik
- Para Transferi senaryoları (pozitif / negatif / edge)
- Login senaryoları (özellikle güvenlik ve kilitleme)

###  Orta Öncelik
- Hesap görüntüleme hesaplamaları
- İşlem geçmişi doğrulama senaryoları

---

##  Sonuç

Bu risk analizi doğrultusunda:
- Test kapsamı **iş riskine göre** şekillendirilmiştir
- Kritik modüller için daha detaylı ve yoğun test senaryoları oluşturulmuştur
- Test eforu, en yüksek etkiyi yaratacak alanlara yönlendirilmiştir
