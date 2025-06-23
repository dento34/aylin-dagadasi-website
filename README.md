# Av. Aylin Dağadası Ünal Hukuk & Danışmanlık Website

Modern, responsive ve SEO optimizasyonlu hukuk bürosu web sitesi. Decap CMS ile entegre admin panel.

## 🌟 Özellikler

- ✅ **Responsive Design** - Tüm cihazlarda mükemmel görünüm
- ✅ **SEO Optimized** - Arama motorları için optimize edilmiş
- ✅ **Admin Panel** - Decap CMS ile kolay makale yönetimi
- ✅ **Fast Loading** - Optimizasyonlu performans
- ✅ **Modern UI/UX** - Kullanıcı dostu arayüz
- ✅ **Contact Forms** - EmailJS entegrasyonu
- ✅ **GitHub Pages** - Ücretsiz hosting

## 📁 Proje Yapısı

```
aylin-dagadasi-website/
├── index.html              # Ana sayfa
├── makaleler.html          # Makaleler sayfası
├── admin/                  # Admin panel (Decap CMS)
│   ├── index.html         # Admin arayüzü
│   └── config.yml         # CMS konfigürasyonu
├── _articles/             # Makale dosyaları (Markdown)
├── images/                # Görseller
│   └── articles/         # Makale görselleri
├── .github/workflows/     # GitHub Actions
│   └── deploy.yml        # Deployment konfigürasyonu
├── sitemap.xml           # SEO sitemap
├── robots.txt            # SEO robots dosyası
└── README.md             # Bu dosya
```

## 🚀 Kurulum

### 1. Repository Oluştur
```bash
# GitHub'da yeni repository oluştur: aylin-dagadasi-website
# Dosyaları bu repository'e yükle
```

### 2. GitHub Pages Aktifleştir
1. Repository → Settings → Pages
2. Source: "GitHub Actions" seç
3. Deploy olmasını bekle

### 3. Decap CMS Kurulumu

#### A. Config dosyasını güncelle
`admin/config.yml` dosyasında şu satırları değiştir:
```yaml
backend:
  repo: KULLANICI_ADI/aylin-dagadasi-website  # GitHub kullanıcı adınız
site_url: https://KULLANICI_ADI.github.io/aylin-dagadasi-website/
display_url: https://KULLANICI_ADI.github.io/aylin-dagadasi-website/
```

#### B. Netlify Identity Kurulumu (Ücretsiz)
1. [Netlify.com](https://netlify.com)'da hesap oluştur
2. "Add new site" → "Import from Git" → GitHub repo'nu seç
3. Site Settings → Identity → Enable Identity
4. Settings → Identity → External providers → GitHub'ı aktifleştir
5. Registration → "Invite only" seç
6. Site Settings → Identity → Services → Git Gateway'i aktifleştir

#### C. Admin Panel Erişimi
1. `https://KULLANICI_ADI.github.io/aylin-dagadasi-website/admin/` adresine git
2. "Login with GitHub" ile giriş yap
3. Makale eklemeye başla! 🎉

## 📝 Admin Panel Kullanımı

### Yeni Makale Ekleme
1. Admin panel → "📝 Makaleler" → "New 📝 Makale"
2. Makale bilgilerini doldur:
   - **Başlık**: SEO için net başlık
   - **Kategori**: Hukuk alanını seç
   - **Kapak Görseli**: Görsel yükle (opsiyonel)
   - **Özet**: Google'da görünecek açıklama
   - **İçerik**: Makale metnini yaz
3. "Save" butonuna tıkla
4. Publish et

### Markdown Kullanımı
```markdown
## Ana Başlık
### Alt Başlık

**Kalın metin** ve *italik metin*

- Liste öğesi 1
- Liste öğesi 2

[Link metni](https://example.com)
```

## 🎨 Özelleştirme

### Renkleri Değiştirme
`index.html` ve `makaleler.html` dosyalarında:
```css
:root {
    --primary: #0f3460;  /* Ana renk */
    --secondary: #6b7280; /* İkincil renk */
}
```

### İletişim Bilgilerini Güncelleme
`index.html` dosyasında #contact bölümünü düzenle.

### Logo Değiştirme
`images/` klasörüne logo yükle ve HTML'de yolu güncelle.

## 📞 İletişim Formu (EmailJS)

### Kurulum:
1. [EmailJS.com](https://emailjs.com)'da hesap oluştur
2. Gmail servisini bağla
3. Template oluştur
4. `index.html`'de API anahtarlarını güncelle:
   ```javascript
   emailjs.init("YOUR_PUBLIC_KEY");
   emailjs.send('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', templateParams)
   ```

## 📈 SEO İyileştirmeleri

### Yapılan Optimizasyonlar:
- ✅ Meta tags (title, description, keywords)
- ✅ Open Graph tags (sosyal medya)
- ✅ Structured data (JSON-LD)
- ✅ Sitemap.xml
- ✅ Robots.txt
- ✅ Fast loading
- ✅ Mobile-first design

### Google Search Console Ekleme:
1. [Google Search Console](https://search.google.com/search-console)'a git
2. Property ekle → URL prefix
3. Ownership doğrula
4. Sitemap submit et

## 🔧 Bakım

### Düzenli Yapılması Gerekenler:
- Makaleleri düzenli güncelle
- Broken linkleri kontrol et
- Site hızını test et
- Backup al

### Sorun Giderme:
- **Admin panel açılmıyor**: GitHub Pages aktif mi kontrol et
- **Makaleler gözükmüyor**: _articles klasöründe .md dosyaları var mı?
- **Form çalışmıyor**: EmailJS anahtarları doğru mu?

## 🆘 Destek

Sorun yaşıyorsanız:
1. GitHub Issues'da konu aç
2. Hata mesajını paylaş
3. Browser console loglarını kontrol et

## 📄 Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

---

**© 2025 Av. Aylin Dağadası Ünal Hukuk & Danışmanlık**

**🌐 Website:** https://KULLANICI_ADI.github.io/aylin-dagadasi-website/
**📧 E-posta:** aylindagadasi@gmail.com
**📞 Telefon:** 0533 412 31 39