\# Para Transferi – Manuel Test Senaryoları



> Kapsam: FG-03 Para Transferi gereksinimleri



\## Ortak Varsayımlar / Test Verisi

\- Günlük transfer limiti: 50.000 TL

\- Kullanıcı giriş yapmış olmalı

\- Kullanıcının seçilebilir bir “kaynak hesabı” olmalı



---



\### TS-TRF-001 – Başarılı para transferi (pozitif)

\- Ön Koşullar: Kullanıcı giriş yapmış, bakiye yeterli (ör. 10.000 TL)

\- Adımlar:

&nbsp; 1. Para Transferi ekranına gir.

&nbsp; 2. Geçerli alıcı IBAN gir.

&nbsp; 3. 1.000 TL tutar gir.

&nbsp; 4. “Gönder” butonuna tıkla.

\- Test Verisi: IBAN=TR12 \*\*\*\* \*\*\*\* \*\*\*\* 1234, Tutar=1000

\- Beklenen Sonuç: Transfer başarılı olmalı, kullanıcıya başarı mesajı gösterilmeli, işlem geçmişine kayıt düşmeli.

\- Öncelik: Yüksek



\### TS-TRF-002 – Tutar alanı boş bırakıldığında hata (negatif)

\- Ön Koşullar: Kullanıcı giriş yapmış

\- Adımlar:

&nbsp; 1. Para Transferi ekranına gir.

&nbsp; 2. Geçerli IBAN gir.

&nbsp; 3. Tutar alanını boş bırak.

&nbsp; 4. “Gönder” butonuna tıkla.

\- Test Verisi: IBAN=geçerli, Tutar=boş

\- Beklenen Sonuç: Transfer yapılmamalı, “Tutar zorunludur” benzeri hata mesajı gösterilmeli.

\- Öncelik: Yüksek



\### TS-TRF-003 – IBAN alanı boş bırakıldığında hata (negatif)

\- Ön Koşullar: Kullanıcı giriş yapmış

\- Adımlar:

&nbsp; 1. Para Transferi ekranına gir.

&nbsp; 2. IBAN alanını boş bırak.

&nbsp; 3. 500 TL tutar gir.

&nbsp; 4. “Gönder” butonuna tıkla.

\- Test Verisi: IBAN=boş, Tutar=500

\- Beklenen Sonuç: Transfer yapılmamalı, “IBAN zorunludur” benzeri hata mesajı gösterilmeli.

\- Öncelik: Yüksek



\### TS-TRF-004 – Tutar 0 girildiğinde transfer reddedilmeli (negatif)

\- Ön Koşullar: Kullanıcı giriş yapmış

\- Adımlar:

&nbsp; 1. Geçerli IBAN gir.

&nbsp; 2. Tutar alanına 0 gir.

&nbsp; 3. “Gönder” butonuna tıkla.

\- Test Verisi: Tutar=0

\- Beklenen Sonuç: Transfer yapılmamalı, “Tutar 0’dan büyük olmalıdır” hatası gösterilmeli.

\- Öncelik: Yüksek



\### TS-TRF-005 – Negatif tutar girildiğinde transfer reddedilmeli (negatif)

\- Ön Koşullar: Kullanıcı giriş yapmış

\- Adımlar:

&nbsp; 1. Geçerli IBAN gir.

&nbsp; 2. -10 tutar gir.

&nbsp; 3. “Gönder” butonuna tıkla.

\- Test Verisi: Tutar=-10

\- Beklenen Sonuç: Transfer yapılmamalı, uygun hata mesajı gösterilmeli.

\- Öncelik: Yüksek



\### TS-TRF-006 – Bakiye yetersizken transfer reddedilmeli (negatif)

\- Ön Koşullar: Kullanıcının bakiyesi 100 TL

\- Adımlar:

&nbsp; 1. Geçerli IBAN gir.

&nbsp; 2. 500 TL tutar gir.

&nbsp; 3. “Gönder” butonuna tıkla.

\- Test Verisi: Bakiye=100, Tutar=500

\- Beklenen Sonuç: Transfer yapılmamalı, “Yetersiz bakiye” mesajı gösterilmeli.

\- Öncelik: Yüksek



\### TS-TRF-007 – Günlük limitin altında transfer yapılabilmeli (pozitif)

\- Ön Koşullar: Kullanıcının günlük toplam transferi 0 TL

\- Adımlar:

&nbsp; 1. Geçerli IBAN gir.

&nbsp; 2. 49.999 TL tutar gir.

&nbsp; 3. “Gönder” butonuna tıkla.

\- Beklenen Sonuç: Transfer başarılı olmalı.

\- Öncelik: Yüksek



\### TS-TRF-008 – Günlük limit aşıldığında transfer reddedilmeli (negatif)

\- Ön Koşullar: Kullanıcının günlük toplam transferi 0 TL

\- Adımlar:

&nbsp; 1. Geçerli IBAN gir.

&nbsp; 2. 50.001 TL tutar gir.

&nbsp; 3. “Gönder” butonuna tıkla.

\- Beklenen Sonuç: Transfer yapılmamalı, “Günlük limit aşıldı” mesajı gösterilmeli.

\- Öncelik: Yüksek



\### TS-TRF-009 – Günlük limit tam sınırda transfer (edge)

\- Ön Koşullar: Kullanıcının günlük toplam transferi 0 TL

\- Adımlar:

&nbsp; 1. Geçerli IBAN gir.

&nbsp; 2. 50.000 TL tutar gir.

&nbsp; 3. “Gönder” butonuna tıkla.

\- Beklenen Sonuç: Gereksinime göre (limit dahilse) transfer başarılı olmalı.

\- Öncelik: Yüksek



\### TS-TRF-010 – IBAN formatı geçersiz (negatif)

\- Ön Koşullar: Kullanıcı giriş yapmış

\- Adımlar:

&nbsp; 1. IBAN alanına geçersiz format gir (ör. “12345”).

&nbsp; 2. 100 TL tutar gir.

&nbsp; 3. “Gönder” butonuna tıkla.

\- Beklenen Sonuç: Transfer yapılmamalı, “Geçersiz IBAN” mesajı gösterilmeli.

\- Öncelik: Yüksek



\### TS-TRF-011 – IBAN başında/sonunda boşluk ile giriş (edge)

\- Ön Koşullar: Kullanıcı giriş yapmış

\- Adımlar:

&nbsp; 1. IBAN alanına başında/sonunda boşluk olan geçerli IBAN gir.

&nbsp; 2. 100 TL tutar gir.

&nbsp; 3. “Gönder” butonuna tıkla.

\- Beklenen Sonuç: Sistem boşlukları trimlemeli; transfer başarılı olmalı veya doğrulama mesajı göstermeli (beklenen davranış netleştirilmeli).

\- Öncelik: Orta



\### TS-TRF-012 – Açıklama alanı boşken transfer (pozitif)

\- Ön Koşullar: Kullanıcı giriş yapmış, bakiye yeterli

\- Adımlar:

&nbsp; 1. Geçerli IBAN gir.

&nbsp; 2. 200 TL tutar gir.

&nbsp; 3. Açıklama alanını boş bırak.

&nbsp; 4. “Gönder” butonuna tıkla.

\- Beklenen Sonuç: Transfer başarılı olmalı.

\- Öncelik: Orta



\### TS-TRF-013 – Çok uzun açıklama girildiğinde kontrol (edge)

\- Ön Koşullar: Kullanıcı giriş yapmış

\- Adımlar:

&nbsp; 1. Geçerli IBAN gir.

&nbsp; 2. 200 TL tutar gir.

&nbsp; 3. 300 karakterlik açıklama gir.

&nbsp; 4. “Gönder” butonuna tıkla.

\- Beklenen Sonuç: Sistem maksimum uzunluk kuralına göre davranmalı (sınırlama/hata).

\- Öncelik: Orta



\### TS-TRF-014 – Transfer sonrası işlem geçmişinde görünürlük (pozitif)

\- Ön Koşullar: Başarılı bir transfer yapılmış olmalı

\- Adımlar:

&nbsp; 1. İşlem Geçmişi ekranına git.

&nbsp; 2. Son işlemlere bak.

\- Beklenen Sonuç: Transfer kaydı listede görünmeli (tutar, tarih, alıcı).

\- Öncelik: Yüksek



\### TS-TRF-015 – Aynı alıcıya art arda transfer (edge)

\- Ön Koşullar: Kullanıcı giriş yapmış, bakiye yeterli

\- Adımlar:

&nbsp; 1. Aynı IBAN’a 100 TL transfer yap.

&nbsp; 2. Hemen tekrar aynı IBAN’a 100 TL transfer yap.

\- Beklenen Sonuç: Her iki işlem de kurallara uygunsa başarılı olmalı, işlem geçmişinde iki kayıt görünmeli.

\- Öncelik: Orta



