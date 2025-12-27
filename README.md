# Manuel Test – Dijital Bankacılık Projesi

Bu repo, bir **dijital bankacılık uygulaması** için uçtan uca  
**manuel test yaklaşımını** göstermektedir.

Proje kapsamında; gereksinim analizi, risk tabanlı test yaklaşımı, test planı,
test senaryosu yazımı, hata raporlama ve test özet raporu çalışmaları
yer almaktadır.

---

## 📌 Proje Özeti

Alan (Domain): **Dijital Bankacılık / Fintech**  
Test Türü: **Manuel Test**  
Yaklaşım: **Risk Tabanlı Test**

Bu proje, manuel test alanında aşağıdaki yetkinlikleri göstermek amacıyla oluşturulmuştur:

- Analitik test bakış açısı
- Risk önceliklendirme
- Düzenli ve anlaşılır test dokümantasyonu
- Profesyonel hata raporlama
- Test sonuçlarına göre değerlendirme yapabilme

---

## 🧩 Uygulama Kapsamı (Mini Bankacılık Sistemi)

Aşağıdaki temel bankacılık modülleri test kapsamına alınmıştır:

- Giriş (Login)
- Hesap Görüntüleme
- Para Transferi
- İşlem Geçmişi

Her modül, iş kritikliği ve risk seviyesine göre analiz edilerek test edilmiştir.

---

## 🧠 Uygulanan QA Yaklaşımı

Bu proje kapsamında aşağıdaki manuel test adımları izlenmiştir:

- **Gereksinim Analizi**  
  Fonksiyonel gereksinimler incelenmiş ve test edilebilir hâle getirilmiştir.

- **Risk Tabanlı Test**  
  Para transferi gibi kritik modüller, etki ve olasılık kriterlerine göre önceliklendirilmiştir.

- **Test Planlama**  
  Test kapsamı, test yaklaşımı ile giriş ve çıkış kriterleri belirlenmiştir.

- **Test Senaryosu Tasarımı**  
  Pozitif, negatif ve edge case test senaryoları hazırlanmıştır.

- **Hata Raporlama**  
  Tespit edilen hatalar standart hata raporu formatında dokümante edilmiştir.

- **Test Özeti ve Yayın Kararı**  
  Test sonuçları değerlendirilmiş ve yayına çıkış için öneri sunulmuştur.

---

## 📂 Proje Klasör Yapısı

```text
manual-testing-digital-banking
 ┣ requirements/          → Fonksiyonel gereksinimler
 ┣ risk-analysis/         → Risk analizi ve önceliklendirme
 ┣ test-plan/             → Test planı
 ┣ test-cases/            → Manuel test senaryoları
 ┣ bug-reports/           → Hata raporu şablonu ve örnekler
 ┣ test-summary-report/   → Test sonuç özeti ve yayın kararı
 ┗ README.md
