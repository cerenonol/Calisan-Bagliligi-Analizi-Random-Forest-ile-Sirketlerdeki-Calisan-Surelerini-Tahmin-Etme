# Çalışan Bağlılığı Analizi: Random Forest ile Şirketlerdeki Çalışan Sürelerini Tahmin Etme

## Proje Açıklaması

Bu proje, şirketlerdeki çalışan bağlılığını analiz etmek amacıyla **Random Forest** algoritmasını kullanır. Çalışanların kişisel ve profesyonel verilerini kullanarak, hangi faktörlerin çalışanların şirketteki kalış sürelerini etkilediğini tahmin eder. Bu model, şirketlerin insan kaynakları stratejilerini geliştirmelerine yardımcı olabilir.

## Amaç

- Çalışanların şirkette ne kadar süre kalacaklarını tahmin etmek.
- Çalışan bağlılığını etkileyen faktörleri analiz etmek.
- İnsan kaynakları stratejilerinin optimize edilmesine katkı sağlamak.

## Veri Seti

Bu projede kullanılan veri seti, çalışanların demografik bilgileri, iş geçmişi, eğitim durumu, çalışma saatleri ve diğer iş performansı verilerini içermektedir. Bu veriler ışığında, çalışanların şirkette kalma süreleri tahmin edilmektedir.

### Veri Seti Özellikleri:
- Çalışanların yaşı
- Eğitim seviyesi
- Çalışma süresi
- İşe geliş-gidiş saatleri
- Performans değerlendirmeleri
- İş tatmini gibi faktörler

## Kullanılan Teknolojiler

- **Python**
- **Pandas** (Veri analizi)
- **Scikit-learn** (Modelleme)
- **Random Forest** (Makine öğrenmesi algoritması)
- **Matplotlib / Seaborn** (Veri görselleştirme)

## Yöntem

- Veriler, ön işleme ve temizleme adımlarından geçtikten sonra **Random Forest** algoritmasıyla modellenmiştir.
- Model, çalışanların bağlılık süresini tahmin etmek için eğitim verilerini kullanır ve doğruluk oranları ölçülür.
- Çalışan bağlılığına etki eden ana faktörler çıkarılarak, şirketlerin bu faktörleri stratejik kararlar alırken kullanması sağlanır.

## Nasıl Çalışır?

1. Verilerinizi hazırlayın ve temizleyin.
2. **Random Forest** modelini eğitin ve tahmin yapın.
3. Modelin doğruluğunu test edin ve sonuçları analiz edin.

## Kurulum

1. **Gerekli Kütüphaneleri Yükleyin:**
```bash
pip install pandas scikit-learn matplotlib seaborn
