# Test Planı – Dijital Bankacılık (Manuel Test)

---

## 1️⃣ Amaç

Bu test planının amacı, mini kapsamlı dijital bankacılık uygulamasının
kritik fonksiyonlarının manuel test ile doğrulanmasını sağlamaktır.

Test kapsamına alınan ana modüller:
- Giriş (Login)
- Hesap Görüntüleme
- Para Transferi
- İşlem Geçmişi

---

## 2️⃣ Kapsam (In Scope)

- Giriş (Login)
- Hesap Görüntüleme  
  *(Hesap listesi, bakiye ve toplam bakiye)*
- Para Transferi
- İşlem Geçmişi  
  *(Listeleme ve tarih filtresi)*

---

## 3️⃣ Kapsam Dışı (Out of Scope)

- Performans testleri
- Gerçek ödeme / banka entegrasyonları
- Mobil native uygulama testleri
- Penetrasyon testleri  
  *(Security test kapsam dışıdır, sadece temel kontroller yapılacaktır)*

---

## 4️⃣ Test Yaklaşımı

Test çalışmaları sırasında:

- Risk analizi baz alınarak **yüksek riskli alanlara öncelik** verilecektir.
- Kritik iş akışları için **Smoke test** uygulanacaktır.
- Pozitif, negatif ve **edge case** testleri yürütülecektir.
- Bulunan hatalar **bug report formatında** raporlanacaktır.

---

## 5️⃣ Test Türleri

- **Smoke Test**  
  Kritik akışların hızlı kontrolü

- **Fonksiyonel Test**  
  Gereksinimlere uygunluk kontrolü

---

## 6️⃣ Giriş & Çıkış Kriterleri

### Giriş Kriterleri
- Gereksinimlerin netleştirilmiş olması
- Test ortamının hazır olması

### Çıkış Kriterleri
- Kritik hataların kapatılmış olması
- Test özet raporunun hazırlanması
