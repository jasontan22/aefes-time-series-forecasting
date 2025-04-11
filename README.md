# Anadolu Efes Biracılık ve Malt Sanayii A.Ş. (AEFES) Verilerinin Makine Öğrenimi Yöntemleri ile Tahmini

Bu proje, Anadolu Efes Biracılık ve Malt Sanayii A.Ş. (AEFES) piyasa verilerini kullanarak kapanış fiyatlarının gelecekteki değerlerini tahmin etmek amacıyla geliştirilmiştir. Projede, LSTM, BiLSTM ve CNN+LSTM modelleri kullanılarak zaman serisi tahminleri gerçekleştirilmiştir.

## Kullanılan Kütüphaneler

- `numpy`: Matematiksel işlemler için.
- `pandas`: Veri analizi ve işleme için.
- `matplotlib` ve `seaborn`: Verilerin görselleştirilmesi için.
- `tensorflow`: Derin öğrenme modellerini oluşturmak için.
- `scikit-learn`: Veri ön işleme ve model değerlendirme için.

## Veri Seti

Proje, 6 Mart 2023 tarihinden itibaren günümüze kadar olan tarihsel verileri içeren bir CSV dosyası (`stock_data.csv`) kullanmaktadır. Bu veri seti, şirketin borsa performansını analiz etmek ve tahmin yapmak amacıyla işlenmiştir.

## Adımlar

1. **Veri Yükleme ve Ön İşleme**
   - Veriler pandas kullanılarak yüklenir ve tarih, kapanış fiyatı, açılış fiyatı, en yüksek ve en düşük fiyat, işlem hacmi gibi bilgilerin düzenlenmesi sağlanır.
   - Boş değerler ve hatalı veriler temizlenir.

2. **Veri Normalizasyonu**
   - Kapanış fiyatları, Min-Max ölçekleme yöntemi ile [0, 1] aralığına normalize edilir.

3. **Zaman Serisi Verisi Oluşturma**
   - Belirli bir süre boyunca (örneğin, 60 gün) kapanış fiyatları kullanılarak özellikler ve etiketler oluşturulur.

4. **Eğitim ve Test Setlerine Ayırma**
   - Veri seti %80 eğitim ve %20 test olarak ayrılır.

5. **Model Oluşturma**
   - LSTM, BiLSTM ve CNN+LSTM modelleri tanımlanır ve her bir model eğitim verisi üzerinde eğitilir.

6. **Model Değerlendirme**
   - Test verisi üzerinde tahminler yapılır ve sonuçlar değerlendirilir.
   - Gerçek değerler ile tahminler karşılaştırılır ve görselleştirilir.

## Kullanım

1. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install tensorflow matplotlib scikit-learn
