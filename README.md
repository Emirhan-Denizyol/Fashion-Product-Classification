# Fashion-Product-Classification

## 👗 Fashion Intelligence System (Giyim Görüntü Analizi)

Bu proje, görsel veriler üzerinden giysi türünü, mevsimini, kullanım amacını ve baskın rengini tahmin eden **entegre bir derin öğrenme sistemidir**. Kullanıcı, kameradan çekilen bir görüntüyle giysi analizi başlatabilir ve modelin tahminleri anında alınabilir.

## 👥 Katkıda Bulunanlar

Bu proje, **Emirhan Bey** ve **Fatih Kaya (https://github.com/fth2745)** tarafından birlikte geliştirilmiştir.  
Her iki geliştirici de görüntü işleme, modelleme ve sistem mimarisi alanlarında aktif katkı sağlamıştır.

## 🚀 Özellikler

- 📷 **Kamera ile Canlı Görüntü Alma**
- 🧼 **Arka Plan Temizleme (rembg ile)**
- 🧠 **ResNet50 Tabanlı Giysi Türü Sınıflandırma**
- 🔖 **Çoklu Etiket Tahmini (Mevsim, Yıl, Kullanım)**
- 🎨 **Ortalama Renk Hesaplama ve Adlandırma**
- 🛠️ **LAB Renk Uzayında Normalize Edilmiş Görüntü İşleme**
- 🛑 **Early Stopping ile Akıllı Model Eğitimi**

## 📂 Proje Yapısı

fashion_model_final/
│
├── fashion_model_final.py # Ana Python betiği (model ve tüm fonksiyonlar)
├── apperal_type_pred_model.pth # Giysi türü modeli ağırlıkları
├── [kagglehub veri dizini] # Moda görselleri ve etiket verisi

## 🧪 Kullanılan Teknolojiler

| Teknoloji     | Açıklama                              |
|---------------|----------------------------------------|
| PyTorch       | Derin öğrenme modelleri               |
| ResNet50      | Görüntü sınıflandırma tabanı          |
| Rembg         | Arka plan temizleyici                 |
| OpenCV        | LAB renk uzayı işlemleri              |
| Matplotlib    | Renk ismi tahmini (CSS4 renk eşleme)  |
| Google Colab  | Kamera erişimi ve demo çalışması      |

## 📈 Eğitim Performansı

Model, `Early Stopping` ile doğrulama kaybına göre otomatik olarak durur. Eğitim ve doğrulama başarıları kaydedilir ve çıktı olarak verilir.

## ▶️ Kullanım

1. Gereken Python ortamını hazırlayın
2. Veri setini `kagglehub` ile indirin
3. `fashion_model_final.py` dosyasını çalıştırarak kameradan görüntü alın
4. Tahminleri çıktı olarak alın

Bu projede kullanılan veri seti:

Param Aggarwal, Fashion Product Images Dataset, Kaggle

🔗 https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset

📄 Lisans: CC0: Public Domain
