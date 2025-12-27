\# İşlem Geçmişi – Manuel Test Senaryoları



> Kapsam: FG-04 İşlem Geçmişi



\## Ortak Varsayımlar

\- Kullanıcı sisteme giriş yapmıştır.

\- Kullanıcının daha önce gerçekleştirilmiş işlemleri bulunmaktadır.



---



\### TS-HIS-001 – İşlem geçmişinin listelenmesi (pozitif)

\- Adımlar: İşlem Geçmişi ekranına git

\- Beklenen Sonuç: Kullanıcıya ait işlemler listelenmelidir.

\- Öncelik: Yüksek



\### TS-HIS-002 – Son yapılan işlemin listede görünmesi (pozitif)

\- Ön Koşullar: Yeni bir transfer yapılmış

\- Adımlar: İşlem Geçmişi ekranını aç

\- Beklenen Sonuç: En son yapılan işlem listede görünmelidir.

\- Öncelik: Yüksek



\### TS-HIS-003 – İşlem detay bilgilerinin doğruluğu (pozitif)

\- Adımlar: Bir işlem kaydını incele

\- Beklenen Sonuç: Tutar, tarih ve işlem tipi doğru olmalıdır.

\- Öncelik: Yüksek



\### TS-HIS-004 – Tarih filtresi ile işlem listeleme (pozitif)

\- Adımlar: Belirli bir tarih aralığı seç

\- Beklenen Sonuç: Seçilen tarih aralığındaki işlemler listelenmelidir.

\- Öncelik: Orta



\### TS-HIS-005 – Tarih filtresi boşken arama (edge)

\- Adımlar: Tarih seçmeden filtrele

\- Beklenen Sonuç: Sistem varsayılan olarak son 90 günü göstermelidir.

\- Öncelik: Orta



\### TS-HIS-006 – İşlemi olmayan kullanıcı durumu (negatif)

\- Ön Koşullar: Kullanıcının hiç işlemi yok

\- Adımlar: İşlem Geçmişi ekranına git

\- Beklenen Sonuç: “Gösterilecek işlem bulunamadı” mesajı gösterilmelidir.

\- Öncelik: Orta



\### TS-HIS-007 – Çok sayıda işlemde performans kontrolü (edge)

\- Ön Koşullar: Kullanıcının çok sayıda işlemi var

\- Adımlar: İşlem Geçmişi ekranını aç

\- Beklenen Sonuç: Liste kabul edilebilir sürede yüklenmelidir.

\- Öncelik: Düşük



\### TS-HIS-008 – Giriş yapılmadan işlem geçmişine erişim (negatif)

\- Ön Koşullar: Kullanıcı giriş yapmamış

\- Adımlar: Doğrudan İşlem Geçmişi URL’ine git

\- Beklenen Sonuç: Kullanıcı login ekranına yönlendirilmelidir.

\- Öncelik: Yüksek



