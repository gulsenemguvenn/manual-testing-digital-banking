# Giriş (Login) – Manuel Test Senaryoları

> Kapsam: FG-01 Giriş (Login)

## Ortak Varsayımlar
- Kullanıcı giriş ekranına erişebilir.
- Geçerli bir kullanıcı hesabı vardır.

---

### TS-LOG-001 – Geçerli bilgilerle başarılı giriş (pozitif)
- Ön Koşullar: Kullanıcı hesabı aktif
- Adımlar: Email ve şifre gir → Giriş yap
- Test Verisi: Geçerli email / şifre
- Beklenen Sonuç: Giriş başarılı olur ve Hesap Görüntüleme ekranına yönlendirilir.
- Öncelik: Yüksek

### TS-LOG-002 – Yanlış şifre ile giriş (negatif)
- Adımlar: Geçerli email + yanlış şifre gir → Giriş yap
- Beklenen Sonuç: Giriş başarısız olur, hata mesajı gösterilir.
- Öncelik: Yüksek

### TS-LOG-003 – Email alanı boş bırakıldığında giriş yapılmamalı
- Adımlar: Email boş, şifre dolu → Giriş yap
- Beklenen Sonuç: Giriş yapılmaz, “Email zorunludur” mesajı gösterilir.
- Öncelik: Yüksek

### TS-LOG-004 – Şifre alanı boş bırakıldığında giriş yapılmamalı
- Adımlar: Email dolu, şifre boş → Giriş yap
- Beklenen Sonuç: Giriş yapılmaz, “Şifre zorunludur” mesajı gösterilir.
- Öncelik: Yüksek

### TS-LOG-005 – Geçersiz email formatı ile giriş
- Adımlar: Geçersiz email formatı gir → Giriş yap
- Beklenen Sonuç: Giriş yapılmaz, “Geçersiz email formatı” mesajı gösterilir.
- Öncelik: Orta

### TS-LOG-006 – 5 kez hatalı şifre girildiğinde hesap kilitlenmeli
- Adımlar: Aynı hesapla 5 kez yanlış şifre gir
- Beklenen Sonuç: Hesap 15 dakika kilitlenir ve bilgilendirme mesajı gösterilir.
- Öncelik: Yüksek
