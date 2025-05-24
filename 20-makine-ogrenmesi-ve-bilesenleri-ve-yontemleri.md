# Makine Öğrenmesi

## Tanım ve Tarihçe

Makine öğrenmesi, bilgisayarların açıkça programlanmadan verilerden öğrenme ve karar verme yeteneğidir. Yapay zekânın en hızlı büyüyen alanlarından biridir.

**Tarihsel Gelişim:**
- 1950'ler: Temel kavramların ortaya çıkışı
- 1980'ler: İstatistiksel öğrenme yöntemleri
- 2010'lar: Derin öğrenme devrimi
- Günümüz: Endüstriyel uygulamaların yaygınlaşması

## Bilgisayarların Kendi Kendine Öğrenmesi

Makine Öğrenmesi, bilgisayarlara veri vererek  
onların kendi kendilerine öğrenmelerini sağlar.  
Hiçbir özel programlama gerekmez.  
Yalnızca veri gerekir.

Veri gelir.  
Model öğrenir.  
Gelecekteki sorulara yanıt verir.

Ex: Evin fiyatı nasıl tahmin edilir?  
Alanı, oda sayısı, mahalle gibi verilerle  
bilgisayar bu ilişkiyi kendi kendine öğrenir.

---

## Temel Bileşenler

### 1. Veri

Her şey veriyle başlar.  
Büyük veri mi? Küçük veri mi?  
Veri, modelin besinidir.

Veri seti ikiye ayrılır:

- **Eğitim (Training)** → Model öğrenir
- **Test (Testing)** → Model ne kadar iyi öğrendiğini gösterir

Veri içinde iki tür bilgi vardır:

- **Giriş (Features):** Evde kaç oda var? Kaç metrekare?
- **Çıkış (Labels):** Fiyat nedir?

Model, giriş ile çıkış arasındaki bağlantıyı bulur.  
Ve yeni verilerde bu bağlantıya göre tahmin yapar.

Veri Yönetimi
- **Eğitim Verisi**: Modelin öğrendiği temel bilgi kaynağı
- **Test Verisi**: Model performansını ölçmek için kullanılır
- **Özellikler (Features)**: Girdi değişkenleri (örn: evin metrekaresi)
- **Etiketler (Labels)**: Tahmin edilecek çıktı (örn: ev fiyatı)

---

### 2. Model

Model, veriyle kurulan ilişkidir.  
Sayılar arasında bir fonksiyondur.  
Öğrenilmiş bir denklemdir.

Model, eğitim verisindeki örüntüleri öğrenir.  
Sonra test verisinde ya da yeni veride kullanılır.  
Doğru tahmin edebilmek için genelleme yapması gerekir.

Modeller farklı biçimlerde saklanır:  
`.h5`, `.pt`, `.pth`, `SavedModel` gibi formatlarla.

Modeller
- Matematiksel fonksiyonlar olarak düşünülebilir
- Eğitim sonucu oluşan tahmin kuralları

---

### 3. Algoritma

Algoritma, modeli oluşturan yöntemdir.  
Hangi yöntemi kullanacağımız,  
verinin yapısına ve amacımıza bağlıdır.

Ex:  
Fiyat tahmini için → Linear Regression  
Sınıflandırma için → Decision Tree veya SVM  
Gruplama için → K-Means

Her algoritmada farklı bir yol izlenir.  
AMA hedef aynıdır:  
**Veriden anlam çıkarmak.**

Algoritmalar
- Problem türüne göre seçim yapılır
- Hiperparametre ayarları kritik önem taşır
- "En iyi algoritma" yoktur, probleme göre değişir

---

### 4. Hedef Fonksiyonu

Ne tahmin etmek istiyoruz?  
Ne sınıflandırmak istiyoruz?

Bu sorunun cevabı, hedef fonksiyonudur.  
Modelin nereye gitmesi gerektiğini söyler.

Ex:  
“Bu evin fiyatı kaçtır?” → Regresyon  
“Bu mail spam mı değil mi?” → Sınıflandırma

---

### 5. Öğrenme Süreci

İşte burada büyüler olur.  
Model veriyle tanışır.  
Aradaki ilişkiyi çözmeye çalışır.

İlk aşamada model bilmez.  
Ama her iterasyonda daha iyi hale gelir.  
Yanlışları düzeltilir.  
Doğrular pekiştirilir.

Bu süreç bittiğinde model artık hazırdır.  
Yeni verilerle karşılaşınca karar verebilir.

Öğrenme Süreci
- Modelin verilerle etkileşimi
- Kayıp fonksiyonlarının optimizasyonu
- Aşırı uydurma (overfitting) riskinin yönetimi

---

## Makine Öğrenmesi Yöntemleri

Makine öğrenmesi üç ana gruba ayrılır:  
**Gözetimli/Denetimli** ,  
**Gözetimsiz/Denetimsiz** ,  
**Pekiştirmeli**

Her biri farklı iş yapar.  
Her biri farklı bir dünyadır.

---

## 1. Gözetimli Öğrenme (Supervised Learning)

- **Tanım**: Etiketli verilerle çalışır
- **Alt Kategoriler**:
  - Sınıflandırma (Classification)
  - Regresyon (Regression)
- **Örnekler**: Spam tespiti, ev fiyat tahmini

Burada veriye yön verilir.  
Label (etiket) vardır.  
Model “ne doğru” olduğunu bilir.  
Yanlış yaptığında düzeltilebilir.

### Kullanım Alanları:

- Fiyat tahmini
- Spam tespiti
- Hastalık teşhisi

### İki Ana Türü Vardır:

#### a) Regresyon

Sayısal tahminler yapmak içindir.  
Ex: Bir ürünün fiyatı

#### b) Sınıflandırma

Etiketlemek içindir.  
Ex: Bu mail spam mı değil mi?

---

## 2. Gözetimsiz Öğrenme (Unsupervised Learning)

- **Tanım**: Etiketsiz verilerde yapı keşfi
- **Alt Kategoriler**:
  - Kümeleme (Clustering)
  - Boyut indirgeme (Dimensionality Reduction)
- **Örnekler**: Müşteri segmentasyonu, anomali tespiti

Burada label yoktur.  
Model kendi başına çalışır.  
Verideki desenleri kendi keşfeder.

### Kullanım Alanları:

- Müşteri segmentasyonu
- Anomali tespiti
- Benzerlik analizi

### En Çok Kullanılan Teknik:

- Kümeleme (Clustering)
- Boyut indirgeme (Dimensionality Reduction)

Ex:  
Müşteriler alışveriş alışkanlıklarına göre gruplandırılır.  
Kimse onlara nasıl ayrılacağını söylemez.  
Model kendisi çözer.

---

## 3. Pekiştirmeli Öğrenme (Reinforcement Learning)

**Tanım**: Ödül mekanizmasıyla öğrenme
- **Uygulamalar**:
  - Otonom sistemler
  - Oyun AI'ları
  - Robot kontrolü

Burada model, deneme-yanılma yoluyla öğrenir.  
Her doğru adım ödüllendirilir.  
Her yanlış adım cezalandırılır.

### Kullanım Alanları:

- Oyun AI’ları
- Robot hareket kontrolü
- Otonom araç sistemleri

Ex:  
Robot süpürge, hangi rotayı izleyeceğini  
deneyerek öğrenir. Her başarılı temizlik ödüldür.

---

## Karşılaştırmalı Tablo: ML Yöntemleri

### Gözetimli - Gözetimsiz - Pekiştirmeli

|Özellik|**Gözetimli**|**Gözetimsiz**|**Pekiştirmeli**|
|---|---|---|---|
|**Etiket (Label)**|Var|Yok|Hayır ama ödül/ceza var|
|**Amacı**|Tahmin veya sınıflandırma|Gruplama veya yapı bulma|En iyi kararı verme|
|**Kullanım Alanı**|Satış tahmini, spam tespiti|Müşteri segmentasyonu|Otonom araç, robotlar|


---

## Yaygın Makine Öğrenmesi Algoritmaları

|Algoritma|Türü|Kullanım Amacı|
|---|---|---|
|**Linear Regression**|Gözetimli|Sayısal tahmin|
|**Logistic Regression**|Gözetimli|Sınıflandırma|
|**Decision Tree**|Gözetimli|Karar verme ağacı|
|**Support Vector Machine (SVM)**|Gözetimli|Sınırları belirleme|
|**Naive Bayes**|Gözetimli|Olasılık tabanlı sınıflandırma|
|**KNN (k-En Yakın Komşu)**|Gözetimli|Benzerliğe göre tahmin|
|**Random Forest**|Gözetimli|Birden fazla karar ağacı|
|**XGBoost**|Gözetimli|Yüksek performanslı sınıflandırma|
|**K-Means**|Gözetimsiz|Kümeleme|
|**PCA (Principal Component Analysis)**|Gözetimsiz|Boyut indirgeme|

## Yaygın ML Algoritmaları  Ne Zaman Kullanılır?

|Algoritma|Problem Türü|Açıklama|
|---|---|---|
|**Linear Regression**|Regresyon|Doğrusal ilişki arar. Fiyat tahmini için kullanılır.|
|**Logistic Regression**|Sınıflandırma|İkili sınıflar arasında karar verir. Spam olup olmadığını tahmin eder.|
|**Decision Tree**|Sınıflandırma & Regresyon|Karar ağacı şeklinde çalışır. Kolay anlaşılır.|
|**SVM (Support Vector Machine)**|Sınıflandırma|Yüksek boyutlu verilerde sınırları çizer.|
|**Naive Bayes**|Sınıflandırma|Olasılığa dayanır. Metin analizinde sık kullanılır.|
|**KNN (k-Nearest Neighbors)**|Sınıflandırma & Regresyon|En yakın komşulara bakarak karar verir.|
|**Random Forest**|Sınıflandırma & Regresyon|Birden fazla karar ağacının ortak çalışmasıdır. Daha güçlüdür.|
|**XGBoost**|Sınıflandırma & Regresyon|En güçlü sınıflandırıcılar arasındadır. Yarışmalarda yaygın kullanılır.|
|**K-Means**|Kümeleme|Benzer olanları gruplamak için kullanılır.|
|**PCA (Principal Component Analysis)**|Boyut Azaltma|Çok sayıda değişkeni azaltır. Veriyi basitleştirir.|


## Gerçek Hayatta Nerede Kullanılır?

|Uygulama|Yöntem|Açıklama|
|---|---|---|
|**Ev Fiyat Tahmini**|Supervised – Regresyon|Evin özellikleri girilir. Fiyat tahmini yapılır.|
|**Spam Tespiti**|Supervised – Sınıflandırma|Mail içeriği analiz edilir. Spam mı değil mi?|
|**Müşteri Segmentasyonu**|Unsupervised – Kümeleme|Müşteriler satın alma alışkanlıklarına göre gruplandırılır.|
|**Otomatik Araba Kontrolü**|Reinforcement|Aracı, ödül/ceza sistemine göre yönlendirir.|


---

## **Uygulama Adımları**

1. **Problem Tanımı**: Çözülmek istenen sorunun netleştirilmesi
2. **Veri Toplama**: Kaliteli ve temsili veri setinin oluşturulması
3. **Veri Ön İşleme**: Eksik veri, aykırı değer yönetimi
4. **Model Seçimi**: Problem türüne uygun algoritma seçimi
5. **Eğitim**: Modelin veriyle öğrenme süreci
6. **Değerlendirme**: Test verisi üzerinde performans ölçümü
7. **Dağıtım**: Modelin üretim ortamına alınması
8. **İzleme**: Performansın sürekli takibi


---

## Son Söz

Makine Öğrenmesi, veriden anlamlı bilgi çıkarmanın sanatıdır.  
Üç yolu vardır:  
Gözetimli,  
Gözetimsiz,  
ve Pekiştirmeli.

Her model, veriyle konuşmayı öğrenir.  
Her algoritma, farklı bir dil konuşur.

Ve en önemlisi:  
**Veri olmadan model yoktur.**  
Model olmadan tahmin yoktur.  
Tahmin olmadan karar yoktur.


Makine öğrenmesi, doğru uygulandığında iş süreçlerinde devrim yaratabilir. Ancak başarı için titiz bir veri hazırlığı, uygun algoritma seçimi ve sürekli iyileştirme gereklidir.