# 📱 Birikimim – iOS PWA Kurulum Rehberi

## Uygulamayı iPhone'a Yükleme

### Adım 1: Dosyaları Bir Web Sunucusuna Yükle
Aşağıdaki dosyaları bir web hosting'e yükle:
- `index.html`
- `manifest.json`  
- `sw.js`

> **Ücretsiz seçenekler:**
> - [GitHub Pages](https://pages.github.com) – tamamen ücretsiz
> - [Netlify](https://netlify.com) – dosyaları sürükle bırak
> - [Vercel](https://vercel.com) – ücretsiz hoşting

### Adım 2: iPhone'da Aç
1. iPhone'da **Safari** tarayıcısını aç (Chrome çalışmaz!)
2. Sitenin adresine git (örn: `https://kullaniciadi.github.io/birikim`)
3. Alt menüde **Paylaş** (kare + ok ikonu) butonuna bas
4. **"Ana Ekrana Ekle"** seç
5. Ad olarak **"Birikimim"** yaz → **Ekle**'ye bas

✅ Artık uygulamanı ana ekranda göreceksin!

---

## Yerel Test (Bilgisayarda)

```bash
# Python varsa:
cd birikim-app
python3 -m http.server 8080
# Tarayıcıda: http://localhost:8080
```

---

## Özellikler
- 💵 Dolar / Euro / Sterlin kurları (otomatik, 1 dk güncelleme)
- 🥇 Gram & Ons Altın (canlı metal fiyatları)
- 🥈 Gram Gümüş
- 📈 BIST hisseleri (THYAO, GARAN, vb.)
- 💰 Birden fazla varlık girişi
- 📊 Kâr/zarar hesaplama (alış maliyeti ile)
- 💾 Veriler telefonda saklanır (localStorage)
- 📴 İnternet olmadan son verilerle çalışır

---

## Teknik Detaylar
- **Döviz API:** open.er-api.com (ücretsiz, key gerekmez)
- **Metal API:** api.metals.live (ücretsiz)
- **Borsa:** Yahoo Finance (ücretsiz proxy)
- **Veri saklama:** localStorage (telefon hafızası)
- **PWA:** Service Worker ile offline destek
