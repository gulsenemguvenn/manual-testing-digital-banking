\# Hesap Görüntüleme – Manuel Test Senaryoları



> Kapsam: FG-02 Hesap Görüntüleme



\## Ortak Varsayımlar

\- Kullanıcı sisteme başarılı şekilde giriş yapmıştır.

\- Kullanıcının en az bir adet aktif hesabı bulunmaktadır.



---



\### TS-ACC-001 – Hesap listesinin görüntülenmesi (pozitif)

\- Ön Koşullar: Kullanıcı giriş yapmış

\- Adımlar: Hesap Görüntüleme ekranına git

\- Beklenen Sonuç: Kullanıcıya ait hesaplar listelenmelidir.

\- Öncelik: Yüksek



\### TS-ACC-002 – Hesap bakiyesinin görüntülenmesi (pozitif)

\- Adımlar: Hesap listesine bak

\- Beklenen Sonuç: Her hesabın bakiyesi doğru şekilde gösterilmelidir.

\- Öncelik: Yüksek



\### TS-ACC-003 – IBAN bilgisinin maskelenmesi (pozitif)

\- Adımlar: Hesap bilgilerini incele

\- Beklenen Sonuç: IBAN açık şekilde değil, maskelenmiş formatta gösterilmelidir.

\- Öncelik: Yüksek



\### TS-ACC-004 – Toplam bakiyenin doğru hesaplanması (pozitif)

\- Adımlar: Hesap bakiyelerini ve toplam bakiyeyi karşılaştır

\- Beklenen Sonuç: Toplam bakiye, hesap bakiyelerinin toplamı ile uyumlu olmalıdır.

\- Öncelik: Yüksek



\### TS-ACC-005 – Hesabı olmayan kullanıcı durumu (negatif)

\- Ön Koşullar: Kullanıcının hesabı yok

\- Adımlar: Hesap Görüntüleme ekranına git

\- Beklenen Sonuç: “Gösterilecek hesap bulunamadı” benzeri bilgilendirme mesajı gösterilmelidir.

\- Öncelik: Orta



\### TS-ACC-006 – Hesap bakiyesi 0 olan hesap görüntüleme (edge)

\- Ön Koşullar: En az bir hesabın bakiyesi 0 TL

\- Adımlar: Hesap listesini görüntüle

\- Beklenen Sonuç: 0 TL bakiye doğru şekilde gösterilmelidir.

\- Öncelik: Orta



\### TS-ACC-007 – Sayfa yenilendiğinde hesap bilgilerinin korunması

\- Adımlar: Sayfayı yenile (refresh)

\- Beklenen Sonuç: Hesap bilgileri doğru şekilde tekrar yüklenmelidir.

\- Öncelik: Düşük



\### TS-ACC-008 – Giriş yapılmadan hesap ekranına erişim (negatif)

\- Ön Koşullar: Kullanıcı giriş yapmamış

\- Adımlar: Doğrudan Hesap Görüntüleme URL’ine git

\- Beklenen Sonuç: Kullanıcı login ekranına yönlendirilmelidir.

\- Öncelik: Yüksek



