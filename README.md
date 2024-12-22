# Hayvanların Sınıflandırılması

# **Test Seti Performanslarının Karşılaştırılması ve Raporlanması**

## **Amaç**
Amaç, modelin performansını üç farklı test veri setinde değerlendirmekti:
1. **Orijinal Test Seti**
2. **Manipüle Edilmiş Test Seti**
3. **Beyaz Dengeli Test Seti**

## **Sonuç Özeti**
| Test Seti | Doğruluk | Kayıp |
|---------------------------|-----------|----------|
| **Orijinal Test Seti** | **%94,92** | 0,4589 |
| **Manipüle Edilmiş Test Seti** | **%98,95** | 0,3466 |
| **Beyaz Dengeli Test Seti** | **%99,66** | 0,3308 |

## **Görüşler**
1. **Orijinal Test Seti**:
- Model, orijinal veri setinde iyi performans göstererek **%94,92** doğruluk elde ediyor.
- Bu, modelin eğitim dağılımından verileri doğru şekilde sınıflandırma yeteneğini gösteriyor.

2. **İşlenmiş Test Seti**:
- Parlaklık ve kontrast ayarlamalarıyla model, **%98,95** oranında iyileştirilmiş bir doğruluk elde ediyor.
- Bu, modelin sağlam özellikleri öğrendiğini ve görsel olarak değiştirilmiş verilere iyi genelleme yaptığını gösteriyor.

3. **Beyaz Dengeli Test Seti**:
- Beyaz dengesi düzeltmesi için Gri Dünya varsayımının uygulanması, doğruluğu **%99,66**'ya çıkarıyor.
- Bu, normalizasyonun modelin görüntü özelliklerinin yorumlanabilirliğini artırmadaki etkinliğini gösteriyor.

## **İyileştirme Önerileri**
### **Farklı Yapılabilecek Şeyler**
Bu boru hattını geliştirdiğimden beri (veya biz geliştirdiğimizden beri), alternatif yaklaşımların keşfedilebileceği birkaç alan şunlardır:

1. **Model Geliştirmeleri**:
- ResNet veya EfficientNet gibi önceden eğitilmiş modeller kullanmak eğitimi hızlandırabilir ve sonuçları daha da iyileştirebilirdi.
- Modele SE blokları veya CBAM gibi dikkat mekanizmaları eklemek, özellik çıkarmayı iyileştirebilirdi.

2. **Veri Hazırlama**:
- Rastgele gürültü enjeksiyonu veya afin dönüşümler gibi daha çeşitli artırma tekniklerinin uygulanması, gerçek dünya değişkenliğini daha iyi simüle edebilirdi.
- Diğer renk düzeltme algoritmalarıyla (örneğin, Histogram Eşitleme) test etmek ek içgörüler sağlayabilirdi.

3. **Hiperparametre Optimizasyonu**:
- Optuna veya HyperOpt gibi kütüphanelerle sistematik hiperparametre ayarlaması yapmak daha iyi yapılandırmalar sağlayabilirdi. - Momentumlu SGD veya uyarlanabilir optimize ediciler (örn. AdamW) gibi optimize edicilerle denemeler yapmak performansı daha da iyi ayarlayabilirdi.

4. **Değerlendirme**:
- Çapraz doğrulama, sonuçların veri kümesinin farklı bölümlerinde tutarlı olduğundan emin olmak için kullanılabilirdi.
- Modeli tamamen görülmemiş veri kümelerinde test etmek, gerçek dünyadaki uygulanabilirliği hakkında daha iyi bir anlayış sağlayabilirdi.

### **Puanlar Düşük Olsaydı (<%50)**
Doğruluk önemli ölçüde daha düşük olsaydı, atılabilecek adımlar şunlardır:
- **Model Basitleştirme**: Mimariyi basitleştirerek veya bırakma katmanları ekleyerek aşırı uyumu azaltma.
- **Arttırma**: Aşırı uyumu önlemek ve genellemeyi iyileştirmek için daha agresif artırmalar sunma.
- **İnce Ayar**: Transfer öğrenimi kullanılarak daha küçük bir veri kümesinde eğitim vermek, daha güçlü bir temel oluşturmaya yardımcı olabilirdi.

## **Sonuç**
Model, tüm test setlerinde yüksek doğruluk elde ederek olağanüstü bir genelleme gösteriyor. Ancak mimari, veri ön işleme ve hiperparametre ayarlamalarındaki iyileştirmeler, performansı daha da ileriye taşıyabilirdi. Beyaz dengesi düzeltmesinin etkili bir iyileştirme olduğu kanıtlandı ve test doğruluğunu önemli ölçüde artırdı. Bu deney, benzer görevlerin gelecekteki yinelemeleri için sağlam bir temel oluşturuyor.
