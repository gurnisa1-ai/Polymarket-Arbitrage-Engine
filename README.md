# 🚀 Polymarket Arbitrage Engine & Position Sizer

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Finance](https://img.shields.io/badge/Domain-Quant_Finance-success)
![Risk](https://img.shields.io/badge/Risk_Model-Kelly_Criterion-orange)

## 📌 Proje Özeti (Project Overview)
Bu proje, Polymarket tahmin piyasalarındaki (prediction markets) anlık fiyat uyuşmazlıklarını tespit eden ve **Kelly Kriteri (Kelly Criterion)** kullanarak istatistiksel portföy optimizasyonu yapan algoritmik bir motordur. Sistem sadece brüt arbitraj fırsatlarını bulmakla kalmaz; işlem komisyonlarını, fiyat kaymalarını (slippage) ve emrin gerçekleşmeme risklerini hesaba katarak gerçek dünya (real-world) senaryolarını simüle eder.

## ⚙️ Temel Özellikler (Core Features)
* **Canlı Veri Akışı:** Polymarket API üzerinden açık ve aktif piyasa verilerinin (Order Book) eşzamanlı çekilmesi.
* **Maliyet Odaklı Filtreleme (Execution Costs):** %1 işlem komisyonu ve %0.5 fiyat kayması (slippage) varsayımlarıyla net (Net Edge) kâr hesaplaması.
* **Risk Yönetimi (Kelly Kriteri):** Beklenen değeri (Expected Value) negatif olan işlemleri matematiksel olarak reddederek kasanın iflas riskini (Risk of Ruin) sıfıra indiren sermaye tahsis algoritması.
* **Stres Testi (Backtest):** Algoritmanın yüksek riskli ve düşük kârlı senaryolardaki defansif davranışını kanıtlayan simülasyon modülü.

## 🛠️ Kullanılan Teknolojiler
* **Dil:** Python
* **Kütüphaneler:** `requests`, `json`, `math`
* **Ortam:** Jupyter Notebook (`.ipynb`)

## 💡 Neden Bu Proje? (Kantitatif Yaklaşım)
Piyasalarda "EVET" ve "HAYIR" kontratlarının toplamı teorik olarak her zaman 1.00$ olmalıdır. Bu motor, saniyelik haber akışlarında oluşan uyuşmazlıklarda "ne kadar kâr edileceğini" değil, "hangi fırsatların işlem maliyetleri düşüldüğünde istatistiksel olarak sürdürülemez olduğunu" kanıtlamak için geliştirilmiştir. Algoritmanın sıfır yatırım (`%0.0` allocation) kararı verebilmesi, defansif risk yönetiminin bir kanıtıdır.

---
*Bu proje, istatistiksel altyapı ile algoritmik finans prensiplerinin birleşimi olarak geliştirilmiştir.*
