# İşlem Geçmişi – Manuel Test Senaryoları

**Kapsam:** FG-04 İşlem Geçmişi

---

## Ortak Varsayımlar
- Kullanıcı sisteme giriş yapmıştır.
- Kullanıcının daha önce gerçekleştirilmiş işlemleri bulunmaktadır.

---

## TS-HIS-001 – İşlem geçmişinin listelenmesi (pozitif)
- **Adımlar:** İşlem Geçmişi ekranına git
- **Beklenen Sonuç:** İşlemler listelenmelidir.
- **Öncelik:** Yüksek

---

## TS-HIS-002 – Son yapılan işlemin listede görünmesi
- **Ön Koşullar:** Yeni bir transfer yapılmış
- **Adımlar:** İşlem Geçmişi ekranını aç
- **Beklenen Sonuç:** Son işlem listede görünmelidir.
- **Öncelik:** Yüksek

---

## TS-HIS-003 – İşlem bilgilerinin doğruluğu
- **Adımlar:** Bir işlem kaydını incele
- **Beklenen Sonuç:** Tutar, tarih ve işlem tipi doğru olmalıdır.
- **Öncelik:** Yüksek

---

## TS-HIS-004 – Tarih filtresi ile işlem listeleme
- **Adımlar:** Belirli bir tarih aralığı seç
- **Beklenen Sonuç:** Seçilen tarihteki işlemler listelenmelidir.
- **Öncelik:** Orta

---

## TS-HIS-005 – Tarih filtresi boşken listeleme (edge)
- **Adımlar:** Filtrele butonuna tıkla
- **Beklenen Sonuç:** Varsayılan olarak son 90 gün gösterilmelidir.
- **Öncelik:** Orta

---

## TS-HIS-006 – İşlemi olmayan kullanıcı durumu (negatif)
- **Ön Koşullar:** Kullanıcının işlemi yok
- **Adımlar:** İşlem Geçmişi ekranına git
- **Beklenen Sonuç:** Bilgilendirici mesaj gösterilmelidir.
- **Öncelik:** Orta

---

## TS-HIS-007 – Çok sayıda işlemde performans kontrolü (edge)
- **Ön Koşullar:** Kullanıcının çok sayıda işlemi var
- **Adımlar:** İşlem Geçmişi ekranını aç
- **Beklenen Sonuç:** Liste kabul edilebilir sürede yüklenmelidir.
- **Öncelik:** Düşük

---

## TS-HIS-008 – Giriş yapılmadan erişim kontrolü (negatif)
- **Ön Koşullar:** Kullanıcı giriş yapmamış
- **Adımlar:** İşlem Geçmişi URL’ine git
- **Beklenen Sonuç:** Kullanıcı giriş ekranına yönlendirilmelidir.
- **Öncelik:** Yüksek
