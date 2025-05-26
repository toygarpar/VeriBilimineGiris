# Veri Ön İşleme ve Veri Depolama

## Ham Veriyi Anlamlı Hale Getirmek

Veri bilimcilerin zamanının %95’i ön işleme, analiz ve EDA (keşifsel veri analizi) ile geçer.  
Ham veri gelir.  
Ama bu veri işlenmeden model kurulmaz.  
Analiz yapılamaz.  
Karar alınamaz.

Veri ön işlemesi, veriyi anlamlı hale getirir.  
Temizler.  
Düzenler.  
Zenginleştirir.  
Azaltır.  
Standartlaştırır.  

Ve sonunda veri, analiz için hazır olur.

---

## 1. Veri Temizleme

Ham veri her zaman temiz değildir.  
Eksik satırlar olabilir.  
Yanlış değerler olabilir.  
Gürültülü veriler olabilir.

Eksik veriler: Boş hücrelerin doldurulması veya uygun şekilde işaretlenmesi

Hatalı veriler: Yanlış girilmiş değerlerin düzeltilmesi

Aykırı değerler: Normal dağılımdan uzak veri noktalarının tespiti

Gürültülü veri: Ölçüm hatalarının ve tutarsızlıkların giderilmesi

Bu yüzden ilk adım budur: **veri temizliği**.

### Yapılacaklar:
- **Eksik verileri bulmak:** Kimi hücre boş kalmış olabilir. Neden? Bilinmez. Ama bunları ya doldururuz, ya sileriz.
- **Yanlış verileri düzeltmek:** Bir kişinin yaşı 200 yazılmışsa, bu hatalıdır. Düzeltilmelidir.
- **Gereksiz verileri çıkarmak:** Gerekmediğini düşündüğün sütun varsa, ondan kurtul.

Veri temizliği, veriye saygı göstermektir.  
Çünkü kirli veriyle doğru karar alınamaz.

---

## 2. Veri Standardizasyonu

Farklı kaynaklardan gelen veriler farklı biçimde olabilir.  
Bazılarında "Erkek", bazılarında "E", bazılarında "Male".  
Bazılarında fiyat TL cinsinden, bazılarında USD.

Bu nedenle veri standardize edilir.  
Tüm veri tek bir formatta olur.  
Herkes aynı dilde konuşur.


### Ne Yapılır?
- Tarih formatları eşitlenir.  
- Fiyat birimleri düzenlenir.  
- Sütun isimleri sabitlenir.  
- Sayısal veriler normalize edilir.  

Standardizasyon, verinin tutarlılığını sağlar.  
Analiz etmek kolaylaşır.

Birim uyumluluğu: Tüm verilerin aynı ölçü birimlerine dönüştürülmesi

Format standartizasyonu: Tarih, saat gibi verilerin ortak formata getirilmesi

Normalizasyon: Sayısal değerlerin belirli aralıklara (örn. 0-1) ölçeklenmesi

---

## 3. Veri Zenginleştirme

Veri azsa ne yaparsın?  
Başka veriyle zenginlet.  
Kaynaklar farklıysa bile, verileri birleştir.  

Örneğin:  
Müşteri verisiyle satış verisini birleştirebilirsin.  
Ya da dışarıdan hava durumu verisi ekleyebilirsin.  
Çünkü tüm bu veriler, daha iyi tahminler için gerekli olabilir.

Veri birleştirme: Farklı kaynaklardan gelen verilerin entegrasyonu

Özellik mühendisliği: Mevcut verilerden yeni anlamlı sütunlar türetme

Referans veri ekleme: Harici veri kaynaklarıyla zenginleştirme

### Nasıl Yapılır?
- **Join işlemleri:** İki tabloyu ortak anahtarla birleştirirsin.  
- **Merge işlemleri:** Birden fazla veri kümesini tek bir veri haline getirirsin.  

Zengin veri, güçlü analiz demektir.

---

## 4. Veri Azaltma

Veri çok büyükse işlenebilirlik zorlaşır.  
Büyük veri yavaş çalışır.  
İşlem gücü tüketir.

Bu yüzden veri azaltılır.  
Gereksiz sütunlar çıkarılır.  
Önemsiz özellikler atılır.  
Boyut indirgenir.

### Hangi Yöntemler Kullanılır?
- **Feature Selection:** En önemli,bilgilendirici sütunlar seçilir.  
- **PCA (Principal Component Analysis):** Çok boyutlu veriler azaltılır.  
- **Sampling (Örnekleme):** Büyük veriden küçük örnek alınır, veri setlerinden temsili alt kümeler oluşturulur.  

Az veri, hızlı sonuç demektir.  
Ama bilgi kaybı minimum olmalıdır.

---

## 5. Veri Kalitesi

Veri kalitesi olmadan hiçbir şey işe yaramaz.  
Kaliteli veri, doğru karar demektir.  
Kalitesiz veri ise yanlış yöne götürür.

### Veri Kalitesinin Beş Kuralı:

Doğruluk: Verilerin gerçek değerleri yansıtması

Tamlık: Gerekli tüm alanların dolu olması

Tutarlılık: Farklı kaynaklar arasında uyum

Zamanlılık: Verilerin güncelliği

Geçerlilik: Standartlara ve kurallara uygunluk

#### 1. Doğruluk – Accuracy  
Veri gerçeği yansıtmalıdır. Yanlış veri kullanılmamalıdır.

#### 2. Tamlık – Completeness  
Tüm gerekli veriler mevcut olmalıdır. Eksik olmamalıdır.

#### 3. Tutarlılık – Consistency  
Farklı sistemler arasındaki veri çelişmemelidir.

#### 4. Zamanlılık – Timeliness  
Veri güncel olmalıdır. Eski veri geçmişte kalır.  
Geçmişten gelecek karar, bugünü yanıltabilir.

#### 5. Geçerlilik – Validity  
Veriler belirlenen kurallara uygun olmalıdır.  
Geçersiz veri sistemi bozar.

---

## 6. Veri Depolama

Veri işlendi mi?  
Şimdi sıra geldi saklanmasına.  
Veri yaşam döngüsünde depolama kritik adımdır.  
Hem ham veri hem işlenmiş veri saklanmalıdır.

Veri güvenli olmalı.  
Erişilebilir olmalı.  
Uygun teknolojide saklanmalı.

### Depolama Yaklaşımları

Ham veri deposu: İşlenmemiş orijinal veriler

İşlenmiş veri deposu: Temizlenmiş ve dönüştürülmüş veriler

Yedekleme stratejileri: Düzenli arşivleme ve felaket kurtarma planları

### Üç Ana Aşaması Vardır:

#### 1. Veri Saklama  
Veriler fiziksel sunucularda veya bulutta saklanır.  
SQL ya da NoSQL veritabanlarında yer alır.

#### 2. Veri Yönetimi  
Depolanan veriler düzenlenir.  
Yeni gelen veriler yönetilir.  
Veri yaşam döngüsü planlanır.

#### 3. Veri Yedekleme  
Veri kaybolursa ne olur?  
Hiçbir şey kalmaz.  
Bu yüzden yedekleme yapılır.  
Belirli aralıklarla yedek alınır.  
Veri korunur.  
Veri güvende olur.

---

## Veri Tabanları

Verilerin saklandığı yerdir.  
Ama her veri aynı yapıda değildir.  
Bu yüzden farklı veritabanları vardır.

### 1. İlişkisel Veritabanları (RDBMS)  
Veriler tablolarda saklanır.  
Tablolar arasında ilişki vardır.  
SQL ile sorgulanır.

Tablo yapısı, SQL sorgulama, ACID uyumluluğu

Ex:  
- MySQL  
- PostgreSQL  
- Oracle

### 2. NoSQL Veritabanları  
Veriler yapılandırılmamış olabilir.  
Esnek yapıya sahiptir.  
JSON gibi çalışır.

Türleri:

Belge tabanlı: MongoDB (JSON benzeri yapılar)

Sütun tabanlı: Cassandra (büyük ölçekli veriler)

Anahtar-değer: Redis (yüksek performanslı önbellekleme)

Graf tabanlı: Neo4j (ilişkisel veri modelleri)

Ex:  
- MongoDB  
- Cassandra  
- Redis

---

## Depolama Altyapıları

Şirket içi çözümler: Yerel sunucular ve depolama sistemleri

Bulut depolama:

AWS (S3, RDS, DynamoDB)

Google Cloud (BigQuery, Cloud SQL)

Azure (Blob Storage, Cosmos DB)

Hibrit çözümler: Bulut ve şirket içi sistemlerin kombinasyonu

## Son Söz

Veri bilimi, temiz veriyle başlar.  
Bozuk veriyle ileri gidilemez.  
Bu yüzden veri önceden hazırlanmalıdır.

Veri temizlenir.  
Standardize edilir.  
Zenginleştirilir.  
Azaltılır.  
Kalitesi kontrol edilir.  
Sonra saklanır.

Bu adımlar atlanamaz.  
Atlanırsa, veri değil, kaos oluşur.

Veri bilimciler, veriyle dans eder.  
Ama önce veriyle tanışır.  
Sonra onu anlamaya çalışır.  
Ve en sonunda onunla konuşur.

Veri ön işleme ve depolama stratejileri, veri miktarına, proje gereksinimlerine ve kurumsal altyapıya göre özelleştirilmelidir. Doğru yaklaşım, veri yönetimi maliyetlerini düşürürken analiz kalitesini artıracaktır.

---

