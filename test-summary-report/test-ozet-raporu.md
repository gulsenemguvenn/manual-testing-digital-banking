\# Test Özet Raporu – Dijital Bankacılık Manuel Test Çalışması



\## 1. Amaç

Bu rapor, dijital bankacılık uygulaması için gerçekleştirilen manuel test çalışmalarının

özetini ve test sonuçlarına göre değerlendirmeyi sunmak amacıyla hazırlanmıştır.



---



\## 2. Test Kapsamı

Aşağıdaki modüller manuel test kapsamına alınmıştır:

\- Giriş (Login)

\- Hesap Görüntüleme

\- Para Transferi

\- İşlem Geçmişi



---



\## 3. Test Yaklaşımı

Test çalışmaları sırasında:

\- Risk analizi baz alınarak kritik modüllere öncelik verilmiştir.

\- Pozitif, negatif ve edge case test senaryoları uygulanmıştır.

\- Tespit edilen hatalar standart hata raporu formatında dokümante edilmiştir.



---



\## 4. Test Sonuçları (Özet)



| Modül              | Toplam Test | Başarılı | Başarısız |

|--------------------|-------------|----------|-----------|

| Giriş (Login)      | 10          | 9        | 1         |

| Hesap Görüntüleme  | 8           | 8        | 0         |

| Para Transferi     | 15          | 13       | 2         |

| İşlem Geçmişi      | 8           | 8        | 0         |

| \*\*Toplam\*\*         | \*\*41\*\*      | \*\*38\*\*   | \*\*3\*\*     |



---



\## 5. Bulunan Hatalar

\- Yetersiz bakiye kontrolünün bazı senaryolarda atlandığı gözlemlenmiştir.

\- Günlük transfer limiti sınır senaryolarında beklenen davranış net değildir.



> Tespit edilen hatalar `bug-reports` klasörü altında detaylı şekilde raporlanmıştır.



---



\## 6. Risk Değerlendirmesi

Para transferi modülü yüksek riskli olarak değerlendirildiğinden,

bu alandaki hatalar \*\*kritik\*\* kabul edilmiştir ve yayına çıkmadan önce

mutlaka giderilmesi önerilmektedir.



---



\## 7. Yayına Çıkış (Release) Kararı

Mevcut test sonuçlarına göre:

\- Kritik hatalar giderilmeden yayına çıkılması \*\*önerilmemektedir\*\*.

\- İlgili düzeltmeler sonrası regresyon testlerinin tekrar çalıştırılması gerekmektedir.



---



\## 8. Sonuç

Bu test çalışması kapsamında, dijital bankacılık uygulamasının temel fonksiyonları

manuel test ile doğrulanmış ve riskli alanlar net bir şekilde ortaya konmuştur.



