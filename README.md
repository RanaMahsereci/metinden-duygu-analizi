# Arapça Metin Duygu Analizi

Bu proje, Arapça metinleri analiz ederek duygu (pozitif/negatif) belirleme işlemini gerçekleştiren bir yapay zeka modeli geliştirmeyi amaçlamaktadır. Model, Python tabanlı doğal dil işleme (NLP) teknikleri kullanılarak eğitilmiştir.

## 📌 Proje Özeti
- **Dil Desteği:** Arapça
- **Özellikler:**
  - Duygu analizi (pozitif/negatif sınıflandırma)
  - Model eğitimi ve test edilmesi için gerekli altyapı

## 🚀 Kurulum
Bu projeyi yerel ortamınızda çalıştırmak için aşağıdaki adımları takip edebilirsiniz.

### Gereksinimler
- Python 3.x
- pip
- Virtualenv (Opsiyonel, önerilir)

### Adımlar
1. **Depoyu klonlayın:**
   ```bash
   git clone https://github.com/username/projectname.git
   cd projectname
   ```
2. **Sanal ortam oluşturun ve etkinleştirin (Opsiyonel):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows için: venv\Scripts\activate
   ```
3. **Bağımlılıkları yükleyin:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Analiz scriptini çalıştırın:**
   ```bash
   python analyze_text.py --text "Buraya analiz edilecek metni yazın"
   ```

## 📦 Kullanım
1. Komut satırından metin analizi yapılabilir.
2. Kullanıcı metni girdikten sonra model, metnin duygu analizini belirler.
3. Sonuç terminalde görüntülenir.

### Örnek Veri Girişi ve Çıktı Formatı
Girdi (JSON formatında):
```json
{
  "text": "السيارة رائعة ومريحة للغاية"
}
```

Beklenen çıktı:
```json
{
  "sentiment": "positive"
}
```

## 🛠 Teknolojiler
Bu proje aşağıdaki teknolojileri kullanmaktadır:
- **Python** (Komut satırı tabanlı kullanım)
- **NLTK & Transformers** (Doğal Dil İşleme)
- **Pandas & NumPy** (Veri İşleme)
- **Scikit-learn & TensorFlow/PyTorch** (Makine Öğrenmesi)

## 📊 Model Eğitimi
Modeli eğitmek için aşağıdaki adımları uygulayabilirsiniz:

1. **Veriyi hazırlayın** (CSV veya TSV formatında etiketlenmiş veri).
2. **Modeli eğitin:**
   ```bash
   python train_model.py
   ```
3. **Eğitim sonrası modeli kaydedin ve test edin:**
   ```bash
   python test_model.py
   ```

## 📈 Performans ve Doğruluk
Modelin eğitim ve test performansı aşağıdaki gibidir:
- **Duygu analizi doğruluğu:** %89
- **F1-Skoru:** 0.87

## 🛡️ Güvenlik ve Veri Gizliliği
- Kullanıcı verileri şifrelenir ve güvende tutulur.
- Model eğitiminde hassas veriler kullanılmaz.
