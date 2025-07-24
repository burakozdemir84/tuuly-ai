# tuuly-ai
AI-powered social media assistant for SMEs.
# Tuuly AI – MVP Proje Planı

**Amaç:**  
KOBİ’lerin sosyal medya hesaplarını yapay zeka ile yöneten, içerik üreten ve paylaşan bir SaaS ürünü inşa etmek. Kullanıcılar ayrıca WhatsApp üzerinden komut verebilir, kayıt olabilir ve bildirim alabilir.

---

## 🔧 MVP Özellik Listesi

### 1. Sosyal Medya Hesap Bağlama
- [ ] Kullanıcı, Instagram, LinkedIn ve/veya Facebook hesabını bağlayabilmeli
- [ ] Bağlı hesaplar listelenebilmeli
- [ ] Bağlantı güvenliği ve izin onayı alınmalı (OAuth)

### 2. Yapay Zeka ile İçerik Üretimi
- [ ] Kullanıcıdan kısa brief alınır (ör: “yeni gelen ürün”)
- [ ] AI bu bilgiye göre 3 farklı sosyal medya postu (metin + görsel açıklaması) üretir
- [ ] İçerikler düzenlenebilir ve onay bekleme statüsünde tutulur

### 3. Otomatik Paylaşım
- [ ] Kullanıcı içerikleri planlayabilir (ör: Pazartesi 10:00)
- [ ] Otomatik paylaşım gerçekleşir
- [ ] Yayınlanan içerikler “Geçmiş Gönderiler” ekranında listelenir

### 4. WhatsApp Entegrasyonu
- [ ] Kullanıcı, WhatsApp üzerinden “Kayıt Ol” yazabilir → hesap açılır
- [ ] Yeni içerik önerileri WhatsApp’a bildirim olarak gider
- [ ] Kullanıcı “Paylaş”, “Yeniden Yaz”, “Sil” gibi komutlar verebilir

---

## 📌 Test Senaryoları (Test Cases)

### Test Case 1 – İçerik Üretimi
- **Senaryo:** Kullanıcı, “yeni ürün: kahveli sabun” şeklinde brief girer
- **Beklenen Sonuç:**
  - AI 3 farklı post üretir: (bilgilendirici, tanıtıcı, mizahi)
  - Her biri başlık + metin + görsel önerisi içerir

### Test Case 2 – WhatsApp Kayıt
- **Senaryo:** Kullanıcı WhatsApp'tan "Merhaba" yazar
- **Beklenen Sonuç:**
  - Sistem kullanıcıyı tanır, kayıt başlatır ve formu tamamlamasını ister
  - İlk içerik önerisi akışına yönlendirir

### Test Case 3 – Otomatik Paylaşım
- **Senaryo:** Kullanıcı AI ile oluşturduğu postu “Salı 09:30” için zamanlar
- **Beklenen Sonuç:**
  - Belirtilen saatte ilgili sosyal medya kanalında paylaşım yapılır
  - WhatsApp üzerinden “Paylaştım 🎉” bildirimi gider

---

## 🧱 Kullanılacak Araçlar

| Amaç | Araç |
|------|------|
| UI | Framer, Tailwind UI, Figma |
| Kodlama | Cursor (GPT destekli IDE), Replit |
| Backend | Supabase (veritabanı), Clerk (giriş) |
| AI | OpenAI GPT-4 + DALL·E API |
| Otomasyon | Zapier veya Make |
| Mesajlaşma | WhatsApp Business API (Twilio, Ultramsg gibi sağlayıcılar) |

---

## 🔜 Roadmap (Sonraki Versiyonlar İçin)

- AI ile web sitesi oluşturma (v1.1)
- E-ticaret ürün listeleme + sipariş alma (v1.2)
- WhatsApp üzerinden müşteri sorularını yanıtlama (v1.3)
