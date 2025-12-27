# Hesap Görüntüleme – Manuel Test Senaryoları

**Kapsam:** FG-02 Hesap Görüntüleme

---

## Ortak Varsayımlar
- Kullanıcı sisteme giriş yapmıştır.
- Kullanıcının en az bir aktif hesabı bulunmaktadır.

---

## TS-ACC-001 – Hesap listesinin görüntülenmesi (pozitif)
- **Ön Koşullar:** Kullanıcı hesabı aktif
- **Adımlar:** Hesap Görüntüleme ekranına git
- **Beklenen Sonuç:** Kullanıcıya ait hesaplar listelenmelidir.
- **Öncelik:** Yüksek

---

## TS-ACC-002 – Hesap bakiyelerinin görüntülenmesi
- **Adımlar:** Hesap listesini incele
- **Beklenen Sonuç:** Her hesabın bakiyesi doğru şekilde gösterilmelidir.
- **Öncelik:** Yüksek

---

## TS-ACC-003 – IBAN bilgisinin maskelenmesi
- **Adımlar:** Hesap detaylarını incele
- **Beklenen Sonuç:** IBAN bilgisi maskelenmiş formatta gösterilmelidir.
- **Öncelik:** Yüksek

---

## TS-ACC-004 – Toplam bakiyenin doğru hesaplanması
- **Adımlar:** Hesap bakiyeleri ile toplam bakiyeyi karşılaştır
- **Beklenen Sonuç:** Toplam bakiye doğru hesaplanmalıdır.
- **Öncelik:** Yüksek

---

## TS-ACC-005 – Hesabı olmayan kullanıcı durumu (negatif)
- **Ön Koşullar:** Kullanıcının hesabı yok
- **Adımlar:** Hesap Görüntüleme ekranına git
- **Beklenen Sonuç:** Bilgilendirici mesaj gösterilmelidir.
- **Öncelik:** Orta

---

## TS-ACC-006 – Bakiyesi 0 TL olan hesabın görüntülenmesi (edge)
- **Ön Koşullar:** Hesap bakiyesi 0 TL
- **Adımlar:** Hesap listesini görüntüle
- **Beklenen Sonuç:** 0 TL bakiye doğru şekilde gösterilmelidir.
- **Öncelik:** Orta

---

## TS-ACC-007 – Sayfa yenilendiğinde hesap bilgilerinin korunması
- **Adımlar:** Sayfayı yenile
- **Beklenen Sonuç:** Hesap bilgileri tekrar doğru şekilde yüklenmelidir.
- **Öncelik:** Düşük

---

## TS-ACC-008 – Giriş yapılmadan erişim kontrolü (negatif)
- **Ön Koşullar:** Kullanıcı giriş yapmamış
- **Adımlar:** Hesap Görüntüleme URL’ine git
- **Beklenen Sonuç:** Kullanıcı giriş ekranına yönlendirilmelidir.
- **Öncelik:** Yüksek
