# Veri Analizi

Ön işlemeden geçmiş verileri inceleyerek anlamlı bilgi ve iç görüler elde etme sürecidir.

## Sayıların Anlattığı Hikâyeyi Dinlemek

Veri gelir.  
Temizlenir.  
İşlenir.  
Ve sonra sıra gelir onu anlamaya.  
Sayıların içinde saklı olan hikâyeyi bulmaya.

Veri analizi, işlenmiş veriyi inceleyerek anlamlı bilgi ve içgörüler çıkarmaktır.  
Geçmişe bakar.  
Şimdiyi tanımlar.  
Yarını tahmin eder.

Her kararın arkasında bir analiz vardır.  
Her trendin altında bir sayı gizlidir.

---

## 1. Tanımlayıcı Analiz – Descriptive Analysis

Ne olmuş?  
Geçmişte neler olmuş?  
Sayılar bize ne diyor?

Tanımlayıcı analiz, verilerin mevcut ve geçmiş durumlarını özetler.  
Merkezi eğilim ölçüleri (ortalama, medyan, mod), Dağılım ölçüleri (varyans, standart sapma, çeyreklikler) gibi ölçümler kullanılır.  
Verinin genel yapısını gösterir.

### Örnek:
Bir şirketin aylık satış ortalaması nedir?  
En yüksek ve en düşük değerler hangi ayda olmuş?  
Satışlardaki değişkenlik nasıl?

Bu sorulara cevap ararsın.  
Verileri toplarsın.  
Sayıları özetlersin.  
Grafikleri çizersin.

Tanımlayıcı analiz, başlangıçtır.  
Gerçekleri anlatır.

---

## 2. Keşifsel (Exploratory) Analiz - Eğilim ve Desenleri Belirleme

Veriler rastgele değildir.  
Bazı desenler tekrar eder.  
Bazı eğilimler zamanla şekillenir.

Bu yüzden verilerdeki kalıpları (patterns) ararız.  
Grafiğe bakarız.  
Zamana göre değişimleri inceleriz.  
Kategoriler arasında farkları ararız.

Yöntemler:

Görselleştirme teknikleri (histogram, box plot, scatter plot)

Korelasyon matrisleri

Veri gruplama (segmentasyon)

### Örnek:
Bir ürünün satış grafiğine bakarsın.  
Mevsimlik yükselişler görürsün.  
Hafta sonlarında artış olduğunu fark edersin.

Bu eğilimleri bulmak, strateji oluşturmanın temelidir.

---

## 3. Korelasyon ve Regresyon Analizi

### Korelasyon Nedir?

- **Korelasyon Analizi**:
    
    - Pearson, Spearman korelasyon katsayıları
        
    - -1 ile +1 arası değerler
        
    - "Reklam harcamaları ile satışlar arasında 0.78 güçlü pozitif korelasyon var"

İki şey birlikte değişiyor mu?  
Biri artarken diğeri düşüyor mu?  
Yoksa ikisi de aynı yönde mi hareket ediyor?

Korelasyon, iki değişken arasındaki ilişkiyi ölçer.  
Değeri -1 ile +1 arasındadır.  
+1 güçlü pozitif ilişki, -1 güçlü negatif ilişki, 0 ise ilişki yok demektir.

### Regresyon Nedir?

- **Regresyon Analizi**:
    
    - Doğrusal ve lojistik regresyon modelleri
        
    - Tahmin denklemleri oluşturma
        
    - "Reklam bütçesindeki her 1000 TL artış, 23 birimlik satış artışı sağlıyor"

Korelasyon ilişkiden bahseder.  
Regresyon ise bu ilişkiyi model haline getirir.  
Birini kullanarak diğerini tahmin etmek için kullanılır.

Ex: Reklam harcamaları arttıkça satışlar artıyor mu?  
Eğer evetse, yeni bir reklam bütçesiyle gelecek ay kaç ürün satacağını tahmin edebilirsin.

---

## 4. Tahminsel Analiz – Predictive Analysis

Geçmiş verilerden yola çıkar.  
Yarını görmek isteriz.  
Belirsizliği azaltmak için çalışır.

Tahminsel analiz, makine öğrenmesi ve istatistiksel modellerle yapılır.  
Verilerden öğrenebilir.  
Yeni veriler üzerinde tahmin yapabilir.

- **Yöntemler**:
    
    - Zaman serisi analizi (ARIMA, Prophet)
        
    - Makine öğrenmesi algoritmaları
        
    - Ensemble yöntemler

### Örnek:
Geçmiş satış verilerini alırsın.  
Model kurarsın.  
Gelecek ay ne kadar satabileceğini tahmin edersin.

Bu analiz, riskleri yönetmede, fırsatları yakalamada, kararları desteklemektedir.

---

## Veri Analizinde Karşılaşılan Zorluklar

### 1. Veri Kalitesi  
Veri doğru muydu?  
Eksik değil miydi?  
Yanlış mıydı?

Kalitesiz veri, yanlış sonuçlar üretir.  
Analiz bozulur.  
Kararlar yanıltıcı olur.


- **Eksik veri** (% kaçın kabul edilebilir olduğu)
    
- **Aykırı değerler** (veri giriş hatası mı, gerçek değer mi?)
    
- **Ölçüm hataları** (sensör kalibrasyon problemleri)


### 2. Veri Büyüklüğü  
Veri çok büyükse ne olur?  
Yavaş çalışır.  
Daha fazla işlem gücü gerekir.  
Daha uzun süre analiz sürer.

Büyük veri yönetilmelidir.  
Ama yönetilemezse, analiz zorlaşır.

- **Ölçeklenebilirlik** (milyonlarca kaydın işlenmesi)
    
- **Hesaplama maliyeti** (bulut bütçesi yönetimi)
    
- **Dağıtık sistemler** (Spark, Hadoop entegrasyonu)


### 3. Yorumlama ve Anlamlandırma  
Sayılar her zaman açık konuşmaz.  
Onları doğru anlamak gerekir.  
Yanlış yorum, yanlış karar demektir.

- **Korelasyon ≠ Nedensellik** (yanlış yorumlama tuzağı)
    
- **Model aşırı uydurma** (overfitting) riski
    
- **İş birimlerine anlatabilme** (teknik olmayan paydaşlara aktarma)

---

## Analiz Sürecini İyileştirme Yolları

1. **Veri Kalite Kontrolleri**:
    
    - Otomatik validasyon kuralları
        
    - Veri profil raporları oluşturma
        
2. **Modüler Analiz Pipelineları**:
    
    - Yeniden kullanılabilir kod blokları
        
    - Versiyon kontrollü analiz süreçleri
        
3. **Görselleştirme Best Practiceleri**:
    
    - Hikaye anlatımına dayalı dashboardlar
        
    - Etkileşimli raporlar (Power BI, Tableau)
        
4. **Model Validasyonu**:
    
    - A/B testing uygulamaları
        
    - Gerçek dünya performans izleme

---

## Son Söz

Veri analizi, sayılara kulak vermekten ibarettir.  
Sayılar sessizdir ama konuşurlar.  
Yalnızca onları dinleyen kişiler duyar.

Veri analizi ile geçmişe bakarız.  
Şimdiyi anlarız.  
Yarını planlarız.

Ama bunu yapabilmek için:  
Veri kaliteli olmalı.  
Veri anlaşılmış olmalı.  
Veri doğru şekilde analiz edilmiş olmalı.

Çünkü veri bilimi;  
sayıların anlatmak istediği hikâyeyi  
dinlemeyi öğretir.

Veri analizi, organizasyonların veriye dayalı karar alma yetkinliğini doğrudan etkileyen kritik bir süreçtir. Doğru tekniklerin uygulanması ve zorlukların aşılması, rekabet avantajı yaratmada belirleyici rol oynar.

---



