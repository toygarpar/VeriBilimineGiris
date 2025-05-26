# Veri Bilimi ve Popüler Teknolojiler

## Sayıların Arasındaki Gizli Hikâyeleri Bulmak

Büyük veriler sessizdir.  
Ama içinde bir şeyler saklarlar.  
Desenler, ilişkiler, anlamlar...  

Ve bu anlamları bulmak için veri madenciliğini kullanırız.

Veri madenciliği, büyük ve karmaşık veri setlerinden anlamlı bilgiler çıkarma sanatıdır.  
Sayılar arasında gizlenmiş olanı bulur.  
Göremediğimizi gösterebilir.

---

## Hangi Alanlarla İlgilidir?

Veri madenciliği, farklı teknolojilerle el ele yürür:

- **Yapay Zeka (AI)** – Öğrenen makineler  
- **Makine Öğrenmesi (ML)** – Veriden öğrenme  
- **Derin Öğrenme (DL)** – Çok katmanlı yapay sinir ağları  
- **Büyük Veri (Big Data)** – Büyük hacimli verilerle çalışma  
- **Veri Bilimi** – Veriyi anlamlandırmak  

Tüm bu alanlar birbiriyle ilişkilidir.  
AMA her biri farklı iş yapar.

---

## Veri Madenciliği Nedir?

Veri Madenciliği, büyük veri kümelerindeki örüntüleri, eğilimleri ve ilişkileri ortaya çıkarmak için kullanılan analitik bir süreçtir.

Amacı basittir:  
**Verinin içinde saklı olanı bulmak.**

Ex:  
Müşterilerin alışveriş alışkanlıklarını çözmek  
Ya da spam e-postaları tespit etmek.

Veri Madenciliği geçmişe bakar.  
Şimdiyi gösterir.  
Yarına ipucu verir.

---

## Kısa Tarih: Veri Madenciliğinin Gelişimi

Veri madenciliği yeni değildir.  
Uzun bir geçmişi vardır.  
Yavaş yavaş şekillendi.

### 1763 – Bayes Teoremi  
Olasılık teorisinin temeli atıldı.

### 1805 – Regresyon Analizi  
Sayılar arasındaki ilişki ilk defa modellendi.

### 1936 – Turing Makinesi  
Bilgisayarların mantığı tanımlandı.

### 1943 – Sinir Ağları  
İnsan beyni taklit edilmeye çalışıldı.

### 1970 – Veritabanları  
Veriler sistematik şekilde saklanmaya başlandı.

### 1975 – Genetik Algoritmalar  
Doğal seçilim ilkesine dayanan yöntemler geliştirildi.

### 1980 – SQL  
Veritabanlarında sorgulama başladı.

### 2000 – İnternet  
Veri miktarı arttı.  
Erişim kolaylaştı.

### 2008 – Sosyal Medya  
Veri üretimi patladı.  
Her paylaşım bir veriydi artık.

### 2011 – Akıllı Telefonlar  
Veri üretimi taşındı cebimize.

### 2013 – Nesnelerin İnterneti (IoT)  
Cihazlar konuştu.  
Veri her yerdeydi.

### 2018 – Üretken Yapay Zeka  
Yapay zeka, insan gibi konuşmaya başladı.

---

## Veri Bilimi mi? Veri Madenciliği mi?

İkisi benzer ama farklıdır.

### Veri Bilimi  

Veri Bilimi daha geniş bir alandır:

Veri toplama ve temizleme

Analiz ve yorumlama

Veri madenciliğini de kapsar

Mühendislik ve yazılım boyutları var

Daha geniştir.  
Veri toplamaktan başlar.  
Temizlemeye geçer.  
Analize devam eder.  
Sonunda yorumlamayla biter.

Veri bilimi, tüm süreci kapsar.  
Veri madenciliği de içinde yer alır.

### Veri Madenciliği  

Veri Madenciliği daha odaklıdır:

Örüntü keşfi ve analiz teknikleri

Belirli problemlere çözüm üretme

Veri biliminin bir parçası

Daha dar ama güçlüdür.  
Verilerdeki desenleri bulmayı amaçlar.  
Model kurmadan önce ya da sonra uygulanır.

Veri madenciliği, veri biliminin bir parçasıdır.  
Ama ondan daha odaklıdır.

---

## Veri Madenciliği Teknikleri

### 1. Sınıflandırma (Classification)  
Verileri belirli sınıflara, önceden belirli lategorilere ayırır.  
Hangi müşteri sipariş verecek?  
Hangi mail spam?

#### Kullanılan Yöntemler:
- Karar Ağaçları  
- k-En Yakın Komşu (k-NN)  
- Destek Vektör Makineleri (SVM)  
- Naive Bayes  
- Yapay Sinir Ağları (ANN)

Ex: E-postalar ikiye ayrılır: spam mı değil mi?

### Senaryo:

Bir banka, müşterilerinin kredi başvurularında riskli olup olmadıklarını tahmin etmek istiyor.  
Müşteriler ikiye ayrılıyor: “Kabul” veya “Reddilir”.

### Nasıl Çalışır?

Algoritma geçmiş verilerdeki örüntüleri öğrenir.  
Gelir, borç durumu, kredi skoru gibi değişkenlere bakar.  
Yeni bir müşteri geldiğinde onu sınıflandırır.

### Grafik Açıklaması:

- X ekseni: Gelir
- Y ekseni: Borç miktarı
- Noktaların rengi: Kredi kabul durumu (“kabul” / “red”)

> Bir karar sınırı çizilir. Bu sınır sayesinde yeni bir müşterinin nerede yer aldığına göre karar verilir.
---

### 2. Regresyon  
Bir değişkenin başka bir değişkene bağlılığını modellemek için kullanılır.  Değişkenler arasındaki ilişkiyi modeller.
Sayısal tahminler yapmak için idealdir.

#### Kullanılan Yöntemler:
- Doğrusal Regresyon  
- Çoklu Regresyon  
- Polinomsal Regresyon

Ex: Bir ürünün fiyatı, reklam harcamalarına bağlı olarak nasıl değişiyor?

### Senaryo:

E-ticaret sitesi yönetimi, reklam harcamalarına bağlı olarak satışların nasıl değiştiğini modellemek istiyor.

### Nasıl Çalışır?

Reklam bütçesi arttıkça satışlar nasıl değişiyor?  
Bu ilişki doğrusal mı? Yoksa eğrisel mi?

Regresyon bu ilişkiyi matematiksel olarak tanımlar.  
Ex: Satış = 0.8 × Reklam Harcaması + 500

### Grafik Açıklaması:

- X ekseni: Reklam harcamaları
- Y ekseni: Toplam satış
- Noktalar: Gerçek veri noktaları
- Çizgi: Regresyon modelinden çıkan tahmini ilişki

> Model, gelecekte ne kadar harcama yaparsak ne kadar satacağımızı tahmin eder.
---

### 3. Kümeleme (Clustering)  
Benzer verileri aynı gruba, farklı verileri ayrı gruba ayırır.  
Hiçbir etiket yoktur.  
Algoritma kendisi gruplar.

#### Kullanılan Yöntemler:
- K-Means  
- Hiyerarşik Kümeleme  
- DBSCAN

Ex: Müşteriler satın alma alışkanlıklarına göre segmentlere ayrılır.

### Senaryo:

Bir perakende şirketi müşterilerini segmentlere ayırmak istiyor.  
Ama hangi ölçüye göre ayrılacak bilmiyor.  
Veriden kendisi çıkarılsın.

### Nasıl Çalışır?

Müşteriler alışveriş alışkanlıklarına göre gruplandırılır.  
Bazıları sık alışveriş yapanlar, bazıları seyrek ama yüksek değerli alışveriş yapanlar olur.

Algoritma hiçbir etiket kullanmadan bunları kendi başına bulur.

### Grafik Açıklaması:

- X ekseni: Ortalama alışveriş miktarı
- Y ekseni: Alışveriş sıklığı
- Farklı renkler: Oluşan küme sayısı (örneğin 3 küme)

> Her nokta bir müşteriyi temsil eder. Benzer olanlar aynı gruba çekilir.

---

### 4. Anomali Tespiti (Anomaly Detection)  
Normalden sapmış olanı, olağan dışı veri noktalarını bulur.  
Anormal şeyleri tespit eder.

#### Kullanılan Yöntemler:
- Z-Score  
- Mahalanobis Mesafesi  
- İzolasyon Ormanı (Isolation Forest)  
- LOF (Local Outlier Factor)

Ex: Kredi kartı dolandırıcılığı tespiti

### Senaryo:

Bir banka, dolandırıcılık tespiti için işlem verilerini analiz ediyor.  
Normal işlemlerden farklı olanları bulmak hedef.

### Nasıl Çalışır?

İşlem miktarı, zamanı ve konumu gibi veriler incelenir.  
Anormal davranışlar tespit edilir.  
Ve bu davranışlar izole edilir.

### Grafik Açıklaması:

- X ekseni: İşlem saati
- Y ekseni: İşlem tutarı
- Normal işlemler: Mavi noktalar
- Anomali (dolandırıcılık): Kırmızı nokta

> Kırmızı nokta diğerlerinden çok uzakta → anomali!
---

### 5. Zaman Serisi (Time Series)  
Zamana bağlı verilerde trend tahmini yapar, zaman içinde değişen verileri analiz eder.  
Gelecekte ne olacağını tahmin eder.

#### Kullanılan Yöntemler:
- ARIMA  
- Holt-Winters Yöntemi

Ex: Gelecek ay kaç ürün satılacağı tahmini yapılır.

### Senaryo:

Bir mağaza, her ayki satış verisini kullanarak gelecek ayki satışları tahmin etmek istiyor.

### Nasıl Çalışır?

Zaman içindeki veriler trend, mevsimsellik ve rassallık içerir.  
ARIMA veya Holt-Winters yöntemiyle bu desenler modellenir.  
Gelecek değerler tahmin edilir.

### Grafik Açıklaması:

- X ekseni: Zaman (ay bazında)
- Y ekseni: Satış miktarı
- Mavi çizgi: Geçmiş satış verisi
- Kırmızı çizgi: Tahmin edilen gelecek değerler

> Mavi ile kırmızı birleşince, geçmişten geleceğe bağlantı kurulmuş olur.
---

## Karşılaştırmalı Tablo:

### Sınıflandırma – Regresyon – Kümeleme

|Özellik|**Sınıflandırma**|**Regresyon**|**Kümeleme**|
|---|---|---|---|
|**Amacı**|Veriyi sınıflara ayırma|Sayısal tahmin yapma|Gruplandırma|
|**Çıktı Türü**|Kategorik (Evet/Hayır)|Sayısal (500 TL, 3 gün sonra vs.)|Etiketsiz gruplar|
|**Yöntem Türü**|Gözetimli öğrenme|Gözetimli öğrenme|Gözetimsiz öğrenme|
|**Kullanım Alanı**|Spam tespiti, müşteri reddi|Fiyat tahmini, satış tahmini|Müşteri segmentasyonu|
|**Örnek Soru**|Bu müşteri ödeme yapar mı?|Kaç ürün satılır?|Müşteriler kaç gruba ayrılır?|

---

## Ekstra: Hangi Tekniği Ne Zaman Kullanırım?

|Durum|Uygun Teknik|
|---|---|
|Evet-Hayır kararı vermem gerek|Sınıflandırma|
|Sayısal tahmin yapmam gerek|Regresyon|
|Gruplamaya ihtiyacım var ama etiket yok|Kümeleme|
|Anormal şeyleri bulmam gerek|Anomali Tespiti|
|Geleceği tahmin etmem gerek|Zaman Serisi|



## Son Söz

Veri madenciliği, sayıların arasına girip  
gizlenmiş hikâyeleri bulmaktır.  

Büyük verilerde kaybolmuş gibi görünür.  
Ama doğru araçlarla çıkarılabilir.  
Anlamlandırılabilir.  
Karar verilebilir.

Veri Bilimi ise bu süreci yönetir.  
Ham veriden başlayıp  
bilgiye ulaşmanın yolculuğudur.

Ve bu yolculukta  
sınıflandırma, regresyon, kümeleme gibi  
güçlü teknikler bizimle yürüyor.

---


