# Metrion 3D e.U. — Web Sitesi

## Bu ne?
Tamamen statik (sunucu tarafı kod yok, veritabanı yok) tek sayfalık bir kurumsal site.
EN / DE / TR dil desteği var (sağ üstteki düğmelerle değişiyor, seçim tarayıcıda hatırlanıyor).

**Neden güvenli:** Sitede giriş formu, veritabanı, kullanıcı hesabı ya da sunucu tarafında
çalışan kod yok. "Hacklenecek" bir arka uç yok — sadece HTML/CSS/JS dosyaları servis ediliyor.
İletişim formu bile bir sunucuya veri göndermiyor; ziyaretçinin kendi e‑posta uygulamasını
"mailto:" ile açıyor. Bu, saldırı yüzeyini pratikte sıfıra indiriyor.

## Dosya yapısı
```
index.html          → tüm site (HTML + CSS + JS tek dosyada)
assets/logo.jpg      → hero bölümündeki büyük logo
assets/logo-nav.jpg   → menü ve footer'daki küçük logo
assets/favicon.png / favicon-32.png → sekme ikonu
```

## GitHub Pages ile yayınlama (ücretsiz, ~5 dakika)

1. GitHub'da yeni bir **public** repo oluştur (örn. `metrion3d-website`).
2. Bu klasördeki tüm dosyaları (index.html + assets/ klasörü) repoya yükle
   ("Add file → Upload files", sürükle-bırak yeterli).
3. Repo içinde **Settings → Pages** sekmesine git.
4. "Branch" altında `main` / `master` seç, klasör olarak `/ (root)` seç, **Save**.
5. Birkaç dakika içinde site şu adreste yayında olacak:
   `https://<kullanıcı-adın>.github.io/metrion3d-website/`
6. **Kendi domainini bağlamak istersen** (örn. `metrion3d.at`):
   - Settings → Pages → "Custom domain" alanına domaini yaz.
   - Domain sağlayıcında (nereden aldıysan) bir `CNAME` kaydı oluşturup
     GitHub'ın verdiği adrese yönlendir (GitHub bu adımı ekranda gösterecek).
   - "Enforce HTTPS" kutucuğunu işaretle.

## Sonraki güncellemeler
Bana "şunu değiştir / şu ürünü ekle" dediğinde dosyayı güncelleyip sana yeni halini
veririm; sen de GitHub'daki dosyanın üzerine aynı isimle tekrar yüklersin
(Add file → Upload files, otomatik üzerine yazar). İstersen bunu tamamen
otomatikleştiren bir bağlantı (git entegrasyonu) da kurabiliriz — daha önce
konuştuğumuz seçenek.

## Yayınlamadan önce doldurman gerekenler (yasal zorunluluk)
Avusturya'da ticari bir web sitesinin **Impressum (yasal bildirim)** içermesi zorunlu
(§ 5 ECG). Footer'da bu iki alanı gerçek bilgilerinle değiştirmen gerekiyor —
şu an placeholder olarak bırakıldı, gerçek verini bilmediğim için:

- `index.html` içinde `[Owner full name — required]` / `[Full business address — required]`
  (ve DE/TR karşılıkları) yazan yerleri bul, kendi adın ve tam iş adresinle değiştir.
  (Ctrl+F ile "required" ara, 6 yer var — EN/DE/TR × ad/adres.)
- `contact@metrion3d.at` e‑posta adresini gerçek adresinle değiştir (şu an placeholder).
- İstersen bir telefon numarası da ekleyebiliriz — şu an sitede yok.

Bu üç şey dışında site yayına hazır.
