# damla

Tek dosyalık (`index.html`) bir sayfa. Kurulum, derleme, kütüphane yok.

## GitHub Pages'e koymak

1. GitHub'da yeni bir repo aç (örn. `damla`). Public olsun.
2. `index.html` ve `icon.png` dosyalarını repoya yükle ("Add file → Upload files" yeter).
3. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: **main** / **(root)** → Save.
4. 1-2 dakika sonra adres: `https://KULLANICI_ADIN.github.io/damla/`

Terminalden:

```
cd damla
git init
git add .
git commit -m "damla"
git branch -M main
git remote add origin https://github.com/KULLANICI_ADIN/damla.git
git push -u origin main
```

## Metinleri değiştirmek

`index.html` içinde `<script>` etiketinin hemen altındaki `CONFIG` bloğu. Her sahnenin (`cloud`, `fall`, `window`, `beads`, `sea`, `end`)
bir ipucu (`hint`) ve notları (`caps`) var. `t`: sahne başladıktan kaç milisaniye sonra görünsün. `pos`: konum
(bl sol-alt, br sağ-alt, tl sol-üst, tr sağ-üst, ml sol-orta, c orta, bc orta-alt). `<em>…</em>` kehribar renkli vurgu.
`fogWord`: buğuya yazılan yazı (`|` yeni satır), `fogWordNarrow`: telefonda satır bölümü. `name`: cama suyla yazılan isim.

## Nasıl ilerliyor (kaydırma yok, o yapıyor)

1. **Bulut.** Ekrana basılı tutunca sis toplanıp damla oluşuyor; damla parmağı takip ediyor. Dolunca düşüyor.
2. **Düşüş.** Yağmurla şehrin üstüne iniş (~27 sn). Fare/parmak rüzgârı yönlendiriyor, tıklayınca şimşek + gök gürültüsü.
3. **Pencere.** Buğuya "hayatımda gördüğüm en güzel kız" yazılıyor. Camın en az dörtte birini kendisi silince devam ediyor.
4. **Cam.** Buğu dağılınca ıslak parmakla yazılmış gibi "damla" beliriyor, ışıkları kırıyor. Sonra "cama dokun" → dokununca denize düşüyor.
5. **Deniz.** Ay, yıldızlar, şehir ışıkları ve yansımaları. Her dokunuş dalga yapıyor ve sabahı biraz daha yaklaştırıyor (yaklaşık 10 dokunuş).
6. **Sabah.** Güneş doğuyor. "günaydın damla."

Renkler: Damla pembe sevdiği için bütün sahne gül pembesi tonlarında (bulut, şehir ışıkları, buğu, ay, gün doğumu). Vurgu rengi `--amber` değişkeninde.

Ses: ilk dokunuşta yağmur başlar (Web Audio ile üretilir), sağ alttan kapatılır. Yazı tipi: Caveat (el yazısı).
iPhone notları: Safari'de lastik kaydırma, çift dokunma yakınlaştırması ve uzun basınca çıkan menü kapalı.
Çentik ve ana ekran çubuğu için güvenli alanlar ayarlı. Telefon zorlanırsa çözünürlük kendiliğinden düşüyor.
Safari'de paylaş → "Ana Ekrana Ekle" yapınca tam ekran, ikonlu bir uygulama gibi açılıyor.

Masaüstü ve iPhone emülasyonunda baştan sona test edildi.
