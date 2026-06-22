# Kablo Avcısı – İHA'lar için Otonom Engel Tespit ve Kaçınma Sistemi

Kırşehir AR-GE Proje Pazarı – Finalist (2026)

## Proje Özeti
İnsansız Hava Araçları (İHA) uçuşları sırasında karşılaştığı kablo ve benzeri 
ince engelleri gerçek zamanlı tespit ederek otonom kaçınma rotası üreten bir 
derin öğrenme tabanlı sistem.

## Teknik Yaklaşım
- **Tespit:** YOLO mimarisi, ince ve doğrusal nesneleri (kablo) arka plandaki 
  karmaşık yapılardan (ağaç, direk, bina) ayırt edecek şekilde özelleştirildi
- **Veri Seti:** Farklı hava/ışık koşullarında zenginleştirilmiş, kontrast ve 
  kenar belirginleştirme (edge enhancement) ile veri artırımı yapıldı
- **Optimizasyon:** Model, uçbirim (edge) donanımda gerçek zamanlı çalışacak 
  şekilde TensorRT/ONNX formatına dönüştürüldü
- **Donanım Entegrasyonu:** Companion computer üzerinde çalışan model, tespit 
  ettiği engel koordinatlarını MAVLink protokolü ile otopilot kartına iletir
- **Kaçınma Algoritması:** Mesafe/açı analizi → tehlike sınırı kontrolü → 
  otonom kaçış rotası (waypoint) üretimi

## Ekip
Proje Yürütücüsü: Sıla Taşan · Akademik danışman desteğiyle, 2 kişilik ekip
