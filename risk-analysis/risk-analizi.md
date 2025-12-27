\# Risk Analizi – Dijital Bankacılık (Etki x Olasılık)



\## Amaç

Bu dokümanın amacı, dijital bankacılık uygulamasındaki en kritik alanları belirleyerek test çalışmalarını

önceliklendirmektir. Bankacılık uygulamalarında para transferi ve giriş akışları genellikle en yüksek riskli

alanlardır.



\## Ölçek

\- Etki (1-5): Hata olursa kullanıcı/iş açısından oluşacak zarar

\- Olasılık (1-5): Hatanın gerçekleşme ihtimali

\- Risk Skoru = Etki x Olasılık

\- Öncelik: Yüksek / Orta / Düşük



\## Risk Matrisi



| Modül / Alan         | Risk Tanımı                                           | Etki | Olasılık | Skor | Öncelik |

|----------------------|--------------------------------------------------------|------|----------|------|---------|

| Para Transferi       | Yanlış alıcıya / yanlış tutarla transfer               | 5    | 3        | 15   | Yüksek  |

| Para Transferi       | Günlük limitin uygulanmaması                           | 5    | 3        | 15   | Yüksek  |

| Para Transferi       | Yetersiz bakiye varken transferin gerçekleşmesi        | 5    | 2        | 10   | Yüksek  |

| Para Transferi       | Geçersiz IBAN kontrolünün yapılmaması                  | 4    | 3        | 12   | Yüksek  |

| Giriş (Login)        | Hatalı denemelerde hesap kilitlemenin çalışmaması      | 4    | 3        | 12   | Yüksek  |

| Hesap Görüntüleme    | Toplam bakiyenin yanlış hesaplanması                   | 4    | 2        | 8    | Orta    |

| İşlem Geçmişi        | Başarılı transferin geçmişte görünmemesi               | 3    | 2        | 6    | Orta    |



\## Test Öncelik Stratejisi

\- Yüksek öncelik: Para Transferi + Login senaryoları (pozitif/negatif/edge)

\- Orta öncelik: Hesap görüntüleme hesaplamaları ve işlem geçmişi doğrulama



