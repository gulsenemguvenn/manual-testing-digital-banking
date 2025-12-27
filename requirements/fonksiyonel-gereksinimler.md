# Fonksiyonel Gereksinimler – Dijital Bankacılık

Bu doküman, dijital bankacılık uygulamasının
**manuel test çalışmaları kapsamında** ele alınan
fonksiyonel gereksinimlerini içermektedir.

---

## FG-01 – Giriş (Login)

### Açıklama
Kullanıcının sisteme güvenli şekilde giriş yapabilmesini sağlayan fonksiyonlardır.

### Gereksinimler
- Kullanıcı, **e-posta ve şifre** ile giriş yapabilmelidir.
- Kullanıcı **5 kez üst üste hatalı şifre** girerse hesap **15 dakika kilitlenmelidir**.
- Başarılı giriş sonrası kullanıcı **Hesap Görüntüleme** ekranına yönlendirilmelidir.

---

## FG-02 – Hesap Görüntüleme

### Açıklama
Kullanıcının kendisine ait hesap bilgilerini görüntüleyebilmesini sağlayan fonksiyonlardır.

### Gereksinimler
- Kullanıcı, kendisine ait **hesap listesini** görüntüleyebilmelidir.
- **IBAN bilgisi**, maskeleme yöntemi ile gösterilmelidir.
- Kullanıcının **toplam bakiyesi**, doğru şekilde hesaplanarak gösterilmelidir.

---

## FG-03 – Para Transferi

### Açıklama
Kullanıcının başka bir hesaba para transferi yapabilmesini sağlayan fonksiyonlardır.

### Gereksinimler
- Kullanıcı, **alıcı IBAN** ve **tutar bilgilerini** girerek para transferi yapabilmelidir.
- Transfer tutarı **0’dan büyük** olmalıdır.
- **Günlük transfer limiti 50.000 TL** olmalıdır.
- **Yetersiz bakiye** durumunda işlem reddedilmeli ve kullanıcıya uygun hata mesajı gösterilmelidir.
- Başarılı transfer işlemi **İşlem Geçmişi** ekranında görüntülenmelidir.

---

## FG-04 – İşlem Geçmişi

### Açıklama
Kullanıcının geçmişte yaptığı işlemleri görüntüleyebilmesini sağlayan fonksiyonlardır.

### Gereksinimler
- Kullanıcı, **son 90 güne ait** işlem geçmişini görüntüleyebilmelidir.
- Kullanıcı, işlem geçmişini **tarih aralığına göre filtreleyebilmelidir**.
