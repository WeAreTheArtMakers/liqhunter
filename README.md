# Liq Hunter Desktop

Liq Hunter, Pine Script tarafındaki çalışma süresi limitini aşmak için likidite + probability motorunu masaüstüne taşıyan Electron uygulamasıdır.

## Bu Yayında Olanlar (v1)

- Binance Spot + Binance Futures + CoinGecko + CoinMarketCap birleşik market tarama
- Futures-only coin görünürlüğü (`SIRENUSDT`, `ARIAUSDT` gibi)
- Token Scanner filtreleri (search/source/volume/market cap/sort)
- Liq Hunter blokları + Liq Price Ladder + Probability Dashboard
- WebSocket canlı kline akışı
- Desktop Notification + Sound Alert + Preview butonları
- Preset profilleri (kurumsal preset seti + custom kayıt)
- Gelişmiş chart araçları (zoom/pan/fullscreen/engine-chart hide)
- Üst alanda büyük anlık fiyat göstergesi

## Release v1

- Release sayfası: [v1](https://github.com/WeAreTheArtMakers/liqhunter/releases/tag/v1)
- macOS (Apple Silicon): `Liq.Hunter-1.0.0-arm64-mac.zip`
- Windows x64: `Liq.Hunter-1.0.0-win.zip`

## Local Build

```bash
npm install
npm run build
npx electron-builder --mac zip
npx electron-builder --win zip --x64
```

## Dağıtım Modeli

Bu sürüm test dağıtımıdır. Ürün modeli:

1. İlk 30 gün deneme
2. Sonrasında üyelik/lisans aktivasyonu
3. Plan bazlı özellik açma (Starter / Pro / Team)

## Not

- CMC free plan key uygulama içinde kullanılabilir; istenirse `CMC_API_KEY` ile override edilebilir.
- Kaynak kod bu depoda paylaşılmadan, yalnızca README + binary release dağıtımı hedeflenmiştir.
