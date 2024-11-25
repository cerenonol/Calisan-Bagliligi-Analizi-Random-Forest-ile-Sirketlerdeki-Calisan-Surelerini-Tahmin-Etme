# Çalışan İşten Ayrılma Tahmini: Random Forest ve Karmaşıklık Matrisi ile Değerlendirme

## Proje Açıklaması

Bu proje, bir şirketin çalışanlarının işten ayrılma olasılıklarını tahmin etmek amacıyla geliştirilmiştir. Çalışanların işten ayrılma (attrition) kararlarını etkileyen çeşitli faktörler göz önünde bulundurularak, **Random Forest** algoritması kullanılarak bir makine öğrenmesi modeli oluşturulmuştur. Modelin performansı, **karmaşıklık matrisi (confusion matrix)** ve diğer metriklerle (precision, recall, f1-score) değerlendirilmiştir.

Projenin amacı, özellikle düşük memnuniyet seviyeleri, yüksek iş yükü gibi faktörlerin işten ayrılma kararları üzerindeki etkisini analiz etmek ve bu bilgilerle şirketlerin iş gücü yönetimi stratejilerini geliştirmelerine yardımcı olmaktır.

## Veri Kümesi

Veri kümesi, Kaggle'dan alınan **HR Employee Attrition** verilerini içermektedir. Bu veri kümesi, 35 farklı özelliği ve 294 örneği içeren çalışan bilgilerini barındırmaktadır. Özellikler arasında çalışanların yaşları, eğitim düzeyleri, iş tatminleri, aylık gelirleri, çalıştıkları departmanlar gibi faktörler bulunmaktadır. 

Veri seti, çalışanın işten ayrılıp ayrılmadığını (Attrition) tahmin etmeyi amaçlayan bir sınıflandırma problemini çözmek için kullanılmaktadır.

## Kullanılan Yöntemler

1. **Veri Ön İşleme**:
   - Eksik veriler kontrol edilip, gereksiz sütunlar çıkarılmıştır.
   - Kategorik veriler sayısal verilere dönüştürülmüştür.
   - Veriler, eğitim ve test setlerine ayrılmıştır.

2. **Modelleme**:
   - **Random Forest** algoritması kullanılmıştır. Random Forest, birden fazla karar ağacının birleşiminden oluşan ve sınıflandırma problemlerinde güçlü bir performans gösteren bir makine öğrenmesi modelidir.
   - Modelin eğitiminde 100 ağaç kullanılmıştır.

3. **Model Değerlendirme**:
   - Modelin performansı, **karmaşıklık matrisi (Confusion Matrix)**, **precision**, **recall**, **F1 skoru** gibi metriklerle değerlendirilmiştir.
   - Karmaşıklık matrisi ile doğru ve yanlış sınıflandırmalar görselleştirilmiştir.
   - ROC eğrisi ile modelin sınıflandırma başarısı görselleştirilmiştir.

## Sonuçlar

- Modelin **doğruluk oranı** %86.7 olarak bulunmuştur. 
- **Precision** ve **Recall** değerlerine göre, modelin işten ayrılacak çalışanları (Attrition = 1) doğru tahmin etme konusunda bazı zorluklar yaşadığı gözlemlenmiştir. Recall değeri 0.10 iken, precision 0.50'dir.
- **Feature Importance** analizine göre, bazı özelliklerin modelin kararlarını daha fazla etkilediği gözlemlenmiştir.

## Görselleştirmeler

- **Karmaşıklık Matrisi**: Modelin doğru ve yanlış sınıflandırmalarını gösteren bir ısı haritası.
- **ROC Eğrisi**: Modelin sınıflandırma başarısını gösteren bir grafik.
- **Özellik Önem Dereceleri (Feature Importance)**: Modelin kararlarını en fazla etkileyen özelliklerin görselleştirilmesi.

## Kullanılabilirlik

Bu projeyi çalıştırmak için aşağıdaki adımları takip edebilirsiniz:

### Gereksinimler

- Python 3.x
- Pandas
- Numpy
- Scikit-learn
- Matplotlib
- Seaborn

### Kurulum

1. Gerekli kütüphaneleri yüklemek için:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
