# Büyük Veri Teknolojileri – Big Data

Geleneksel yöntemlerle işlenemeyecek kadar büyük, karmaşık ve hızlı veri kümeleridir. Dijital dönüşümün temel taşlarından biridir ve şirketler için yeni fırsatlar sunar.

Tanım Ölçütleri:

Tek bir sunucunun işleyemeyeceği boyutlarda veri

Dağıtık sistemler gerektiren veri hacmi

Geleneksel veritabanı yönetim araçlarıyla yönetilemeyen veriler

## Büyük Veri ve Veri Bilimi İlişkisi

**Ortak Noktalar:**

- Her ikisi de veri analizini temel alır
    
- Karar destek sistemlerinde kullanılır
    
- Yapay zeka ve makine öğrenmesi uygulamalarına destek verir
    

**Farklar:**

|Özellik|Veri Bilimi|Büyük Veri|
|---|---|---|
|Veri Türü|Çoğunlukla statik|Statik + Gerçek zamanlı|
|İşlem Tipi|Batch işlemler|Batch + Stream işlemler|
|Odak|Analiz ve modelleme|Veri işleme ve depolama|


## Geleneksel Yollar Artık Yetmiyor

Geleneksel veri işleme yöntemleri, artık yetmiyor.  
Çünkü veriler çok büyük oldu.  
Çok hızlı üretildi.  
Çok farklı biçimlerde geldi.

Bu yüzden Büyük Veri (Big Data) ortaya çıktı.  
Yeni teknolojiler, yeni sistemler, yeni yaklaşımlar getirdi.

Büyük Veri;  
hacimce büyük,  
hızla üretilen,  
çeşitli kaynaklardan gelen  
verileri ifade eder.

---

## Büyük Veri Ne Kadar Büyük?

Büyük veri, belirli bir boyutla tanımlanmaz.  
10 GB mı? 1 TB mı?  
Değil.  

Eğer bir sunucu bu veriyi işleyemiyorsa,  
ve birden fazla sunucuya ihtiyaç duyuluyorsa,  
bu veri “büyük veri” kategorisine girer.

Ve bu veriler dağıtık sistemlerle işlenir.

---

## Dağıtık Sistem Nedir?

Dağıtık sistem, birkaç bilgisayarın tek bir sistem gibi çalıştığı yapıdır.  
Her bilgisayar bağımsız çalışabilir ama birlikte daha büyük görevler yapar.  

Ex: Bir işlem milyonlarca satır veri içeriyor.  
Bu işlem tek bir makinede yıllar sürebilir.  
Ama onu yüzlerce makineye bölüp yaptırırsanız saniyelerde biter.

Bu sisteme cluster denir.  
Standalone sistemler bir araya gelip cluster oluşturur.  
İşlem kapasitesi artar.

---

## Veri Bilimi ile Büyük Veri Arasında Bağ

Veri Bilimi, Büyük Veri’nin önemli parçasıdır.  
Ancak farkları vardır.

### Veri Bilimi:
- Genellikle batch işlem kullanılır.  
- Veri statiktir.  
- Model kurulur.  
- Tahmin yapılır.

### Büyük Veri:
- Batch + streaming verilerle çalışır.  
- Gerçek zamanlı analiz yapılır.  
- Büyük hacimli veriler işlenir.  
- Veri bilimi süreçleri burada ölçeklenir.

Ex:  
Bir e-ticaret sitesinde milyarlarca işlem varsa,  
bu veri büyük veridir.  
Ve veri bilimi teknikleriyle müşteri davranışları tahmin edilir.

---

## Büyük Verinin Oluşumu

Büyük veri birden fazla yerden gelir:

### Sosyal Medya  
Paylaşımlar, yorumlar, beğeni sayısı her gün milyonlarca satır veri üretir.

### Mobil Uygulamalar  
Konum, aktivite, harcama alışkanlıkları anlık olarak gönderilir.

### Nesnelerin İnterneti (IoT)  
Cihazlar sürekli konuşur.  
Araba, saat, termostat…  
Hepsi veri üretir.

### Log Verileri  
Sistemlerin ne yaptığını gösterir.  
Kim hangi sayfayı açtı?  
Hangi hata oluştu?  
Loglar bunu çözer.

### İşlemsel Veriler  
Finansal işlemler, ödeme geçmişi, transferler  
her saniye yeni veri üretir.

### Multimedya Verileri  
Resim, video, ses gibi yapılandırılmamış verilerdir.  
Geleneksel veri tabanlarında saklamak zordur.

---

## Büyük Verinin 5 V'si

Big Data'nın tanımı, sadece "büyük veri" demek değildir.  
Beş temel özelliği vardır. Bu beş özellik, Büyük Veri’yi tanımlar.

### 1. Hacim (Volume)  
Terabaytlardan petabaytlara kadar veri büyüklüğü
Depolama çözümleri: Data Lakes, Object Storage

Verinin miktarı önemlidir.  
Milyonlarca satır olmalı.  
Bir sunucunun işlemesi zorlaşmalı.  
O zaman veri “büyük” olur.

Örnek: Netflix'in günlük 1 milyar saatlik izleme verisi

### 2. Hız (Velocity)  
Verinin oluşma ve değişme hızı
Gerçek zamanlı veri akışı gereksinimi

Veri üretim hızı yüksektir.  
Her milisaniye yeni veri oluşur.  
Ve bu veri aynı hızla işlenmelidir.

Örnek: Twitter'da her dakika binlerce tweet atılır.  
Onların analizi anında yapılmalıdır.
Canlı borsa verileri, anlık konum takibi

### 3. Çeşitlilik (Variety)  
Yapılandırılmış, yarı yapılandırılmış ve yapılandırılmamış veri türleri
Veri formatları: Metin, görsel, video, JSON, CSV vb.

Veriler farklı biçimlerde gelir.  
Tablolardan metinlere,  
görüntülerden ses dosyalarına kadar  
her şey veri olabilir.

Örnek: Hastane verileri (MR görüntüleri, hasta kayıtları, laboratuvar sonuçları)

### 4. Güvenilirlik/Doğruluk (Veracity)  
Verinin güvenilirliği ve tutarlılığı
Veri kalite yönetimi gereksinimi
İstatistik: İş liderlerinin %33'ü verilerine güvenmiyor

Çözüm: Veri temizleme, doğrulama ve görselleştirme

Veri doğru mu?  
Gerçek mi?  
Doğrulanmış mı?

Veracity, verinin güvenilirliğini ölçer.  
Düşük kaliteli veri kararları bozar.  
Bu yüzden veri önce doğrulanmalıdır.

### 5. Değer (Value)  
Ham veriden türetilen iş değeri
Karar destek sistemlerine katkı

En önemli V budur.  
Veri değerli değilse, büyük olması hiçbir şey ifade etmez.

Eldeki veri,  
karar almayı kolaylaştırıyor mu?  
Stratejiye yön veriyor mu?  
Yararı var mı?

Evet ise, veri değerlidir.

Örnek: Perakendeci için müşteri davranış tahminleri

---

## Karşılaştırmalı Tablo:  
### Büyük Veri vs Veri Bilimi

| Özellik | **Veri Bilimi** | **Büyük Veri** |
|--------|------------------|----------------|
| **Veri Boyutu** | Küçük - Orta | Çok Büyük |
| **İşlem Türü** | Batch | Batch + Streaming |
| **Veri Türü** | Yapılandırılmış | Yapılandırılmış, Yarı Yapılandırılmış, Yapılandırılmamış |
| **Teknoloji** | Excel, SQL, Python | Hadoop, Spark, Kafka |
| **Amacı** | Tahmin ve analiz | Depolama, işlem ve yönetim |
| **Zamanlama** | Statik veriyle çalışma | Anlık veri ile çalışma |

---
## Büyük Veri Teknolojileri

### Dağıtık Sistemler

- **Cluster Yapıları**: Bağımsız sunucuların tek sistem gibi çalışması
    
- **Avantajlar**: Yüksek erişilebilirlik, ölçeklenebilirlik
    
- **Kullanım Senaryoları**: Hadoop, Spark kümeleri
    

### Büyük Veri Ekosistemi

1. **Depolama**: HDFS, Amazon S3
    
2. **İşleme**: Hadoop MapReduce, Spark
    
3. **Veritabanları**: NoSQL (MongoDB, Cassandra)
    
4. **Stream İşleme**: Kafka, Flink
    
5. **Makine Öğrenmesi**: TensorFlow, PyTorch

---
## Son Söz

Büyük Veri, sadece büyük sayılar değildir.  
Sayıların arkasındaki gerçekliği gösterir.  
Yeni fırsatları ortaya çıkarır.  
Stratejileri şekillendirir.

Veri Bilimi bu verilerle anlam üretir.  
Büyük Veri ise bu verilerin taşınmasını,  
işlenmesini,  
ve yönetilmesini sağlar.

İkisi birleştiğinde  
sayılar konuşur.  
ve biz dinleriz.

Büyük veri, doğru şekilde yönetildiğinde kurumlara rekabet avantajı sağlayan stratejik bir varlıktır. Veriden değer üretmek için uygun altyapı, yetenek ve analiz yöntemlerinin bir arada kullanılması gerekir.
---

