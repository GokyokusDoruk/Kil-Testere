# Kıl Testere

Rahatlatıcı kıl testere bulmacası: ahşabı bıçağa doğru it, döndür, hedef şekli çizgisinden kes.
Tek dosya (`index.html`), harici kütüphane yok — HTML5 Canvas + Web Audio. Mouse ve dokunmatik uyumlu.

Canlı: https://kiltestere.dorukplays.com

## Yerelde bakmak
```powershell
python -m http.server 8090
```
Sonra tarayıcıda http://localhost:8090 adresini aç.

## Yayın
Cloudflare Pages bu depoya bağlı. `main`'e birleşen her değişiklik siteyi kendiliğinden günceller.
Derleme komutu yok, çıktı klasörü deponun kökü.
