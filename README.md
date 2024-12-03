# Water Quality Clustering Project 🌊

Bu proje, su kalitesini etkileyen çevresel faktörlerin incelenmesi ve çeşitli kümeleme algoritmaları kullanılarak veri analizinin gerçekleştirilmesini amaçlamaktadır. Su ekosistemlerinin korunması ve izlenmesi için analitik araçlar sunar.

## 🔍 Projenin Hedefi
- **Su kalitesini etkileyen faktörlerin analizi**
- **Farklı kümeleme yöntemlerinin karşılaştırılması**
- **Kümelerin görselleştirilmesi ve yorumlanması**

Bu çalışma, **Python** ve **KNIME** kullanılarak gerçekleştirilmiştir.

---

## 📊 Kullanılan Veriler
Veri seti, aşağıdaki parametreleri içermektedir:
- **Salinity (ppt):** Tuzluluk oranı
- **Dissolved Oxygen (mg/L):** Çözünmüş oksijen
- **pH:** Asitlik/bazlık seviyesi
- **Secchi Depth (m):** Görüş mesafesi
- **Water Depth (m):** Su derinliği
- **Water Temperature (°C):** Su sıcaklığı
- **Air Temperature (°C):** Hava sıcaklığı

---

## ⚙️ Kullanılan Yöntemler ve Araçlar
### KNIME Workflows:
1. **Eksik Veri İşleme:** Eksik değerlerin tespit edilmesi ve uygun yöntemlerle doldurulması
2. **Veri Normalizasyonu:** Algoritmaların performansını artırmak için min-max ölçeklendirme
3. **Kümeleme Algoritmaları:**
   - **K-Means**: Veri noktalarını belirli sayıda kümeye ayırır.
   - **Hierarchical Clustering**: Veriler arasında hiyerarşik ilişkiler kurarak kümeler oluşturur.
   - **DBSCAN**: Yoğunluk tabanlı kümeleme algoritması

### Python Uygulamaları:
1. **Eksik Veri Tamamlama:** Ortalama, ileri veya geri doldurma yöntemleri
2. **Veri Normalizasyonu:** Algoritmalar için ölçek farkını ortadan kaldırma
3. **Algoritmaların Performans Karşılaştırması:**
   - K-Fold Cross Validation ile Silhouette Skorları
4. **Boyut İndirgeme ve Görselleştirme:** PCA kullanarak iki boyutlu grafiklerde kümelerin incelenmesi

---

## 📈 Sonuçlar
- **Silhouette Skorları:**
  - **K-Means:** 0.2349 (Orta düzeyde başarı)
  - **DBSCAN:** -0.2790 (Düşük başarı)
  - **Hierarchical Clustering:** 0.2127 (Orta düzeyde başarı)

- **Görselleştirme:** Kümeler, renk kodları ve dağılım grafikleri ile detaylı bir şekilde incelenmiştir.

---

## 🔧 Projeyi Çalıştırmak
### Gereksinimler:
- **Python 3.x**
- Gerekli kütüphaneler:
  ```bash
  pip install numpy pandas matplotlib scikit-learn
