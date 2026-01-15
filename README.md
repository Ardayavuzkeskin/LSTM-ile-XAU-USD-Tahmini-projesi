# LSTM ile XAU/USD (Altın) Fiyat Tahmini 📈

Bu proje, Derin Öğrenme (Deep Learning) yöntemlerinden biri olan **Long Short-Term Memory (LSTM)** ağlarını kullanarak XAU/USD (Ons Altın) paritesinin gelecekteki fiyat hareketlerini tahmin etmeyi amaçlamaktadır.

Finansal zaman serileri üzerindeki karmaşık ve doğrusal olmayan (non-linear) kalıpları yakalamak için Recurrent Neural Networks (RNN) mimarisinin gelişmiş bir versiyonu olan LSTM tercih edilmiştir.

## 🚀 Proje Hakkında

* **Amaç:** Geçmiş fiyat verilerini analiz ederek gelecek kapanış fiyatlarını (Close Price) tahmin etmek.
* **Yöntem:** Zaman Serisi Analizi ve Denetimli Öğrenme (Supervised Learning).
* **Model:** TensorFlow/Keras tabanlı LSTM Sinir Ağı.

## 🛠️ Kullanılan Teknolojiler

Proje **Python** dili ile geliştirilmiştir ve aşağıdaki kütüphaneler kullanılmıştır:

* **Veri İşleme:** Pandas, NumPy
* **Görselleştirme:** Matplotlib, Seaborn
* **Derin Öğrenme:** TensorFlow, Keras (Sequential, LSTM, Dense, Dropout)
* **Ön İşleme:** Scikit-learn (MinMaxScaler)

## 📊 Veri Seti ve Yöntem

* **Veri Kaynağı:** Projede XAU/USD paritesine ait geçmiş finansal veriler kullanılmıştır.
* **Normalizasyon:** Modelin daha hızlı ve doğru öğrenmesi için veriler `MinMaxScaler` ile 0-1 aralığına ölçeklendirilmiştir.
* **Zaman Penceresi:** Model, belirli bir geçmiş zaman aralığını (Time Steps) inceleyerek bir sonraki adımı tahmin edecek şekilde yapılandırılmıştır.

## 🧠 Model Mimarisi

Model, overfitting'i (aşırı öğrenme) engellemek için **Dropout** katmanları ile güçlendirilmiş, birden fazla **LSTM** katmanından oluşan bir sıralı (Sequential) yapıya sahiptir. Modelin başarısı Mean Squared Error (MSE) kayıp fonksiyonu ile ölçülmüştür.

## 💻 Kurulum

Projeyi kendi bilgisayarınızda incelemek isterseniz:

1.  Repoyu klonlayın:
    ```bash
    git clone [https://github.com/Ardayavuzkeskin/LSTM-ile-XAU-USD-Tahmini-projesi.git](https://github.com/Ardayavuzkeskin/LSTM-ile-XAU-USD-Tahmini-projesi.git)
    ```
2.  Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install pandas numpy matplotlib tensorflow scikit-learn
    ```
3.  Notebook dosyasını çalıştırın.

---
**Geliştirici:** Arda Yavuzkeskin
