# goldPriceTurkey
Multi-feature regression model for gold price prediction — built with Python, LazyPredict, and ExtraTreesRegressor.

# 🏆 Gold Price Prediction (2020–2025) — Türkiye Perspektifi

Bu proje, altın fiyatını (ons) makroekonomik göstergelere (USD/TRY, Brent, DXY, US10Y) dayanarak tahmin eden bir makine öğrenmesi uygulamasıdır.  
Amaç sadece tahmin yapmak değil, fiyatı etkileyen faktörleri anlamak.

---

## 📊 Kullanılan Değişkenler
| Değişken | Açıklama |
|-----------|-----------|
| USDTRY | Dolar / TL kuru |
| Brent | Brent petrol fiyatı |
| DXY | Dolar endeksi |
| US10Y | ABD 10 yıllık tahvil faizi |
| Gold | Altın (XAU/USD) – hedef değişken |

Veri kaynağı: **Yahoo Finance (yfinance)**  
Zaman aralığı: **2020 - 2025**

---

## ⚙️ Süreç
1. Veri temizleme (`ffill`, `bfill`)
2. Korelasyon ve EDA analizi
3. LazyPredict ile model karşılaştırması
4. En iyi modeller:  
   - ExtraTreesRegressor  
   - RandomForestRegressor  
   - BaggingRegressor
5. GridSearchCV ile hiperparametre optimizasyonu
6. Feature Importance ve Residual analizleri

---

## 🧮 Sonuçlar
- R² (test): **0.98**
- RMSE: **≈ 2.0**
- En güçlü değişken: **USD/TRY**
- Model bias göstermiyor (hatalar sıfır civarında dengeli)

---

## 🛠 Kullanılan Araçlar
- Python  
- pandas, numpy, seaborn, matplotlib  
- scikit-learn, LazyPredict  
- yfinance  

---

> “Veri sadece sayı değildir, geleceğin ipuçlarını saklar.”
