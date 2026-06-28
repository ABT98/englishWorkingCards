# YDS Temel Kelime Kartları

Tek sayfalık (bağımlılıksız) flashcard uygulaması. 3088 temel (kırmızı) kelime,
sabit ve benzersiz 30'arlık 103 destede. Öğrenme ilerlemesi cihazda (localStorage) saklanır.

## Klasör içeriği
- `index.html` — uygulama
- `apple-touch-icon.png` — iOS ana ekran ikonu (180×180)
- `icon-192.png`, `icon-512.png` — manifest/Android ikonları
- `manifest.webmanifest` — "Ana Ekrana Ekle" / standalone ayarları

## iPhone'da Safari ile açıp ana ekrana eklemek

Ana ekrana ikon eklemek için dosyaların gerçek bir `https://` adresinde olması gerekir
(`file://` ile "Ana Ekrana Ekle" çıkmaz). En pratik yol GitHub Pages:

1. GitHub'da yeni bir repo oluştur (ör. `kelime`).
2. Bu klasördeki TÜM dosyaları reponun köküne yükle
   (`index.html` mutlaka kökte olsun).
3. Repo → **Settings → Pages**.
4. **Build and deployment → Source: Deploy from a branch**, Branch: `main`, klasör: `/ (root)` → **Save**.
5. 1–2 dakika sonra adresin hazır olur: `https://KULLANICI_ADIN.github.io/kelime/`
6. Bu adresi iPhone'da **Safari** ile aç (Quick Look değil, gerçek Safari).
7. Alttaki **Paylaş** ikonu → **Ana Ekrana Ekle** → **Ekle**.

Artık ikona dokununca tam ekran, adres çubuğu olmadan uygulama gibi açılır.

### Alternatif (repo açmadan)
Bu klasörü `https://app.netlify.com/drop` sayfasına sürükle-bırak → anında bir
`https://...netlify.app` adresi verir. Aynı şekilde Safari'den ana ekrana ekleyebilirsin.

## Sadece hızlıca denemek
Dosyayı iPhone'a (AirDrop / iCloud Drive / e-posta) atıp **Dosyalar** uygulamasından
`index.html`'e dokunarak da çalışır; sadece "Ana Ekrana Ekle" ikonu bu modda çıkmaz.

## Kullanım
- Üstten **deste** seç (1–103).
- Karta **dokun**: İngilizce ↔ Türkçe çevirir.
- **Kaydır**: ←→ gezin, ↑ öğrendim, ↓ tekrar. (Masaüstünde ok tuşları + Boşluk + S.)
- **✓ Öğrendim**: kelime bir daha gelmez. **✕ Tekrar gelsin**: aynı oturumda tekrar döner.
- Üst sağdaki halka toplam ilerlemeyi gösterir; **sıfırla** ile tüm kayıt silinir.

> Not: İlerleme tarayıcıya/cihaza özeldir. `file://` ve `https://` sürümleri ayrı sayılır.
