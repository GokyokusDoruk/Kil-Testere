# Kıl Testere

Rahatlatıcı kıl testere bulmacası: ahşabı bıçağa doğru it, döndür, hedef şekli çizgisinden kes.
Tek dosya (`index.html`), harici kütüphane yok — HTML5 Canvas + Web Audio. Mouse ve dokunmatik uyumlu.

- **127 bölüm**: 7 klasik + 100 yeni şekil + 20 tablo (geometrik, yıldızlar, oklar, doğa, hayvanlar, nesneler). Şekiller işaretli uzaklık fonksiyonlarıyla (SDF) tanımlanır ve bloğa otomatik sığdırılır.
- **Testere ucu keser**: ahşap bir piksel maskesidir; testerenin ucunun değdiği her yer kesilir. Bağlantısı kopan bölgeler parça olarak sağa sola savrulur.
- **Zikzak**: ileri-geri ters dönüşte iki kolun arasındaki ahşap da kesilip atılır.
- **Sipariş**: her bölüm bir şekil ve renk(ler) ister; sağ üstteki panelde görünür.
- **Boyama**: kesimden sonra fırçayı boya kutularına daldırıp boyarsın. 3 fırça boyu (`1` `2` `3`), fırçadaki boya azaldıkça soluklaşır.
- **Renk karıştırma**: kutularda yalnızca kırmızı, sarı, mavi, beyaz ve siyah var. Karıştırma tabağına boya koyup karıştırarak turuncu, yeşil, mor, pembe, lacivert, kahve, gri, turkuaz, lila… elde edilir. Dolu fırçayı başka kutuya daldırmak da karıştırır; su kabı fırçayı temizler. Sipariş panelinde her rengin tarifi görünür. Boya puanı, istenen renge olan renk farkına (CIELAB ΔE) göre verilir.
- **Tablolar**: 20 çok renkli resim bölümü (gün batımı, deniz feneri, kır evi, karpuz…). 5. bölüm bitince açılır.
- Menüde **Geri** butonu (veya `Esc`) ve **dorukplays.com**'a dönüş bağlantısı.

Canlı: https://kiltestere.dorukplays.com

## Yerelde bakmak
```powershell
python -m http.server 8090
```
Sonra tarayıcıda http://localhost:8090 adresini aç.

## Yayın
Cloudflare Pages bu depoya bağlı. `main`'e birleşen her değişiklik siteyi kendiliğinden günceller.
Derleme komutu yok, çıktı klasörü deponun kökü.
