\# Test Planı – Dijital Bankacılık (Manuel Test)



\## 1. Amaç

Bu test planının amacı, mini kapsamlı dijital bankacılık uygulamasının kritik fonksiyonlarının

( Login, Hesap Görüntüleme, Para Transferi, İşlem Geçmişi ) manuel test ile doğrulanmasını sağlamaktır.



\## 2. Kapsam (In Scope)

\- Giriş (Login)

\- Hesap Görüntüleme (Hesap listesi, bakiye ve toplam bakiye)

\- Para Transferi

\- İşlem Geçmişi (listeleme ve tarih filtresi)



\## 3. Kapsam Dışı (Out of Scope)

\- Performans testleri

\- Gerçek ödeme/banka entegrasyonları

\- Mobil native uygulama testleri

\- Penetrasyon testi (security testing kapsam dışı; sadece temel kontroller yapılacaktır)



\## 4. Test Yaklaşımı

\- Risk analizi baz alınarak yüksek riskli alanlara öncelik verilecektir.

\- Kritik akışlar için Smoke test uygulanacaktır.

\- Pozitif, negatif ve edge case testleri yürütülecektir.

\- Bulunan hatalar bug report formatında raporlanacaktır.



\## 5. Test Türleri

\- Smoke Test: Kritik akışların hızlı kontrolü

\- Fonksiyonel Test: Gereksinimlere uygunluk

\- Negatif Test: Hatalı giriş ve beklenen hata mesajları

\- Edge Case: Sınır değerler (limitler, 0, maksimum vb.)



\## 6. Giriş Kriterleri (Entry Criteria)

\- Gereksinim dokümanı hazır olmalı

\- Test ortamına erişim sağlanmalı

\- Test verileri (ör. bakiye, günlük limit) tanımlanmalı



\## 7. Çıkış Kriterleri (Exit Criteria)

\- Yüksek öncelikli testlerin tamamlanması

\- Kritik/Yüksek şiddetli açık hata kalmaması veya risk kabulünün raporlanması

\- Test özet raporunun hazırlanması



\## 8. Test Ortamı

\- Tarayıcı: Chrome (güncel)

\- OS: Windows

\- Test Verisi: Örnek hesaplar, bakiye değerleri, alıcı IBAN’lar



\## 9. Rollerin Tanımı

\- QA (Sen): Test planı, test senaryoları, hata raporları, test özeti



