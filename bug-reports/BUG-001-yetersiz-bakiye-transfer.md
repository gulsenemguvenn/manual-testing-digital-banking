\# BUG-001 – Yetersiz bakiye varken transfer yapılabiliyor



\## Özet (Summary)

Kullanıcının bakiyesi yetersiz olmasına rağmen para transferi işlemi başarılı oluyor.



\## Ortam (Environment)

\- OS: Windows

\- Browser: Chrome (güncel)

\- Uygulama: Dijital Bankacılık – Test Ortamı



\## Ön Koşullar

\- Kullanıcı giriş yapmış olmalı.

\- Kaynak hesap bakiyesi: 100 TL



\## Yeniden Üretme Adımları (Steps to Reproduce)

1\. Para Transferi ekranına gir.

2\. Geçerli alıcı IBAN gir.

3\. Tutar alanına 500 TL gir.

4\. “Gönder” butonuna tıkla.



\## Gerçek Sonuç (Actual Result)

Transfer başarılı mesajı gösteriliyor ve işlem geçmişine kayıt düşüyor.



\## Beklenen Sonuç (Expected Result)

Transfer reddedilmeli ve kullanıcıya “Yetersiz bakiye” hata mesajı gösterilmelidir.



\## Şiddet (Severity)

Kritik (Critical)



\## Öncelik (Priority)

Yüksek (High)



\## Kanıt / Ek (Screenshot, video, log)

\- Ekran görüntüsü eklenecek



