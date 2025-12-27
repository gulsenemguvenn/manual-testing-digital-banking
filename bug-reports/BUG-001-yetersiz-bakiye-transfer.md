#  BUG-001 – Yetersiz bakiye varken transfer yapılabiliyor

---

##  Özet (Summary)
Kullanıcının bakiyesi yetersiz olmasına rağmen para transferi işlemi başarılı şekilde tamamlanmaktadır.

---

##  Ortam (Environment)
- **İşletim Sistemi:** Windows
- **Tarayıcı:** Chrome (güncel)
- **Uygulama:** Dijital Bankacılık – Test Ortamı

---

##  Ön Koşullar
- Kullanıcı sisteme giriş yapmış olmalıdır.
- Kaynak hesap bakiyesi **100 TL**’dir.

---

##  Yeniden Üretme Adımları (Steps to Reproduce)
1. Para Transferi ekranına gir.
2. Geçerli bir alıcı IBAN gir.
3. Tutar alanına **500 TL** gir.
4. **Gönder** butonuna tıkla.

---

##  Gerçek Sonuç (Actual Result)
Transfer başarılı mesajı gösterilmekte ve işlem geçmişine kayıt düşmektedir.

---

##  Beklenen Sonuç (Expected Result)
Transfer işlemi reddedilmeli ve kullanıcıya  
**“Yetersiz bakiye”** hata mesajı gösterilmelidir.

---

##  Şiddet & Öncelik
- **Şiddet (Severity):** Kritik (Critical)
- **Öncelik (Priority):** Yüksek (High)

---

##  Kanıt / Ek (Screenshot, video, log)
