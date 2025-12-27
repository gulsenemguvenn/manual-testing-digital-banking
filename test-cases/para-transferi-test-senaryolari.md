# Para Transferi – Manuel Test Senaryoları

**Kapsam:** FG-03 Para Transferi

---

## Ortak Varsayımlar
- Kullanıcı sisteme giriş yapmıştır.
- Kaynak hesap aktiftir.
- Günlük transfer limiti tanımlıdır.

---

## TS-TRF-001 – Geçerli bilgilerle para transferi (pozitif)
- **Adımlar:** Geçerli IBAN ve tutar gir → Gönder
- **Beklenen Sonuç:** Transfer başarıyla tamamlanır.
- **Öncelik:** Yüksek

---

## TS-TRF-002 – Yetersiz bakiye ile transfer (negatif)
- **Adımlar:** Bakiyeden yüksek tutar gir → Gönder
- **Beklenen Sonuç:** Transfer reddedilir, hata mesajı gösterilir.
- **Öncelik:** Yüksek

---

## TS-TRF-003 – Geçersiz IBAN ile transfer (negatif)
- **Adımlar:** Geçersiz IBAN gir → Gönder
- **Beklenen Sonuç:** Transfer yapılmaz, IBAN hatası gösterilir.
- **Öncelik:** Yüksek

---

## TS-TRF-004 – Transfer tutarı 0 TL girilmesi (edge)
- **Adımlar:** Tutar alanına 0 gir → Gönder
- **Beklenen Sonuç:** Transfer yapılmaz, uyarı mesajı gösterilir.
- **Öncelik:** Orta

---

## TS-TRF-005 – Günlük transfer limitinin aşılması (edge)
- **Adımlar:** Günlük limitten yüksek tutar gir → Gönder
- **Beklenen Sonuç:** Transfer reddedilir, limit uyarısı gösterilir.
- **Öncelik:** Yüksek

---

## TS-TRF-006 – Başarılı transferin işlem geçmişine yansıması
- **Ön Koşullar:** Transfer başarılı
- **Adımlar:** İşlem Geçmişi ekranına git
- **Beklenen Sonuç:** Transfer kaydı görüntülenir.
- **Öncelik:** Orta
