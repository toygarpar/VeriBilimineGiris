# Makine Öğrenmesi Algoritmaları

## Bilgisayarlar Veriden Nasıl Karar Verir?

Bilgisayarlar verileri kullanarak öğrenir.  
Veriden desenleri çeker.  
Sayıların arasına girer.  
Ve tahmin yapar.

Makine Öğrenmesi, bu süreci yönetir.  
Algoritmalar farklıdır.  
AMA tümü aynı amaca hizmet eder:  
**Geleceği tahmin etmek. Karar vermek. Anlam çıkarmak.**

Üç ana kategori vardır:  
**Gözetimli Öğrenme** – Doğru cevap varsa  
**Gözetimsiz Öğrenme** – Doğru cevap yoksa  
**Pekiştirmeli Öğrenme** – Deneme yanılma ile öğreniyorsa

---

## 1. Gözetimli Öğrenme (Supervised Learning)

Burada bilgisayar bir öğretmenle çalışır.  
Her örnek veride bir girdi ve bir çıktı vardır.  
Model, bu ilişkiyi öğrenebilir.

### Kullanım Alanları:
- Fiyat tahmini  
- Spam tespiti  
- Hastalık teşhisi  

### İki Türü Vardır:
#### a) Sınıflandırma (Classification)
Çıkışlar sınıflardır.  
Evet / Hayır  
Spam / Spam değil  
Satın alma / Satın alma  

Ex: Müşterinin sipariş vereceğini tahmin etmek.

#### b) Regresyon (Regression)
Çıkışlar sayısal değerlerdir.  
Fiyat, yaş, gelir gibi.

Ex: Bir evin fiyatını tahmin etmek.

---

### Yaygın Gözetimli Öğrenme Algoritmaları

#### 🔹 KNN – K En Yakın Komşu (k-Nearest Neighbors)

- **Mantık**: "Bana arkadaşlarını söyle, sana kim olduğunu söyleyeyim" 
- **Çalışma Şekli**: Yeni veri noktasını en yakın K komşusunun çoğunluk sınıfına atar
- **Kullanım Alanları**: 
  - El yazısı tanıma
  - Ürün öneri sistemleri
  - Tıbbi teşhis

Bir veri noktası alınır.  
Ona en yakın olan K komşuya bakılır.  
En çok hangi sınıf varsa, o sınıf seçilir.

Ex: Yeni bir müşteri geldi.  
Onunla benzer alışveriş yapan müşteriler kimler?  
Bu komşulara göre yeni müşteriyi sınıflandırırız.

> Grafik Açıklaması:  
Noktalar renklere göre gruplandırılmıştır.  
Yeni nokta geldiğinde en yakın K noktaya bakılır.  
Renkler neyse ona göre karar verilir.



---

#### 🔹 Naive Bayes

- **Temel Prensip**: Bayes Teoremi'ne dayanır
- **Formül**: P(A|B) = [P(B|A) * P(A)] / P(B)
- **Avantajlar**:
  - Hızlı eğitim süresi
  - Yüksek boyutlu verilerde etkili
- **Uygulamalar**:
  - Spam e-posta filtresi
  - Duygu analizi
  - Belge sınıflandırma

Olasılığa dayalı çalışır.  
Bir şeyin olasılığını, başka bir şeyin bilgisiyle hesaplar.

Formülü basittir:  
```
P(A|B) = [P(B|A) × P(A)] / P(B)
```

Ex: E-posta spam mı değil mi?  
“Kazan” kelimesi geçiyorsa, spam olma ihtimali artar.  
Bu kelimeye göre karar verilir.

> Grafik Açıklaması:  
Kelime sıklığına göre spam / non-spam oranları gösterilir.

---

#### 🔹 Decision Tree (Karar Ağacı)

- **Yapı**: If-else kurallarından oluşan hiyerarşik yapı
- **Güçlü Yönleri**:
  - Yorumlanabilirlik
  - Kategorik ve sayısal verilerle çalışabilme
- **Örnekler**:
  - Kredi risk değerlendirme
  - Müşteri kaybı tahmini

Veriyi dallara ayırır.  
Her dal bir sorudur.  
Her yaprak bir sonuçtur.

Ex: Müşteri sipariş verecek mi?  
Yaşı 35’in altında mı?  
Müşteri gelir durumu nedir?  
Bu sorularla karar verilir.

> Grafik Açıklaması:  
Ağaç yapısıyla “Evet / Hayır” dalları gösterilir.

---

#### 🔹 Linear Regression (Doğrusal Regresyon)

- **Temel Fikir**: Bağımlı ve bağımsız değişkenler arasındaki doğrusal ilişki
- **Denklem**: y = b0 + b1*x1 + b2*x2 + ... + bn*xn
- **Kullanım Senaryoları**:
  - Ev fiyat tahmini
  - Satış projeksiyonları
  - Hisse senedi analizi

İki değişken arasında doğrusal bir ilişki kurar.  
Biri artarken diğeri nasıl değişiyor?

Ex: Reklam harcaması arttıkça satışlar nasıl değişiyor?  
Bunu bir çizgiyle ifade edebiliriz.  
Bu çizgi sayesinde gelecek ayki satış tahmini yapılır.

> Grafik Açıklaması:  
X ekseni: reklam harcamaları  
Y ekseni: satışlar  
Noktalar: geçmiş veriler  
Çizgi: regresyon modeli  

---

#### 🔹 Logistic Regression (Lojistik Regresyon)

Regresyon ama çıkış iki sınıftan oluşur.  
0 ya da 1  
Evet ya da Hayır  
Spam ya da Spam Değil  

Ex: Müşteri sipariş verecek mi?  
Verilen özelliklerle “evet” ya da “hayır” tahmini yapılır.

> Grafik Açıklaması:  
Olasılık eğrisi çizilir.  
Belirli eşikten sonra “sipariş verecek” kararı verilir.

---

#### 🔹 Ridge ve Lasso Regresyon

- **Fark**: Regularizasyon teknikleriyle aşırı uydurmayı önleme
- **Karşılaştırma**:
  - Ridge: Katsayıları küçültür
  - Lasso: Bazı katsayıları sıfıra indirir (özellik seçimi)



#### 🔹 Support Vector Machine (Destek Vektör Makinesi)

Veriler arasındaki sınırı çizer.  
Bu sınır, sınıfları en iyi şekilde ayırır.

Ex: İnsan mı robot mu?  
Bu iki gruba göre veriler ayrılır.  
Sınır çizilir.  
Yeni veri bu sınırlarla sınıflandırılır.

> Grafik Açıklaması:  
İki sınıfa ait noktalar yer alır.  
Araya bir sınır çizilir.  
Yeni nokta bu sınıra göre sınıflandırılır.

---

#### 🔹 Random Forest (Rastgele Orman)

Birden fazla karar ağacının ortak çalışmasıdır.  
Her ağacın kararı toplanır.  
En çok oy alan karar alınır.

Ex: Hasta kanser mi değil mi?  
Her karar ağacı farklı özelliklere bakar.  
Toplamda en çok desteklenen karar alınır.

> Grafik Açıklaması:  
Birden fazla karar ağacı çizilir.  
Sonuç, hepsinin ortalaması veya çoğunlukla alınır.

---

#### 🔹 XGBoost (Extreme Gradient Boosting)

Güçlü bir sınıflandırıcıdır.  
Yarışmalarda sıkça kullanılır.  
Karar ağaçlarını ardışık olarak eğitir.  
Her seferinde hataları düzeltilir.

Ex: Kredi başvurusuna kabul verilsin mi?  
Her adım önceki hatayı düzeltir.  
En sonunda güçlü bir model çıkar.

> Grafik Açıklaması:  
Her adımda hata azalır.  
Modelin doğruluğu artar.

---

## 2. Gözetimsiz Öğrenme (Unsupervised Learning)

Burada doğru cevap yoktur.  
Sadece giriş verisi vardır.  
Model kendi başına kalıpları bulmaya çalışır.

### Kullanım Alanları:
- Müşteri segmentasyonu  
- Anomali tespiti  
- Boyut indirgeme  

---

### Yaygın Gözetimsiz Öğrenme Algoritmaları

#### 🔹 K-Means Clustering

**K-Means**
- **Adımlar**:
  1. K sayıda merkez nokta rastgele seç
  2. Her veri noktasını en yakın merkeze ata
  3. Merkezleri yeniden hesapla
  4. Merkezler sabitlenene kadar tekrarla
- **Uygulamalar**:
  - Müşteri segmentasyonu
  - Görüntü sıkıştırma
  - Anomali tespiti

Verileri gruplara ayırır.  
Benzer olanlar aynı gruba girer.  
Her grubun merkezi vardır.  
Yeni veri, en yakın merkeze atanır.

Ex: Müşteriler satın alma alışkanlıklarına göre gruplandırılır.  
Hangi müşteri daha sadık?  
Hangi müşteri riskli?

> Grafik Açıklaması:  
Her nokta bir müşteridir.  
Gruplar farklı renklerde gösterilir.  
Merkezler belirlenir.  

---

#### 🔹 Principal Component Analysis (PCA)

- **Amacı**: Yüksek boyutlu veriyi daha az boyuta indirgerken varyansı koruma
- **Kullanım Alanları**:
  - Görüntü tanıma
  - Veri görselleştirme
  - Gürültü azaltma

Boyut indirgemek için kullanılır.  
Çok fazla sütun varsa, bunları azaltır.  
Veri kaybı olmadan anlamlı özellikleri korur.

Ex: 100 sütun var.  
AMA sadece 10 tanesi önemli.  
PCA ile boyut düşer.  
Model hızlanır.

> Grafik Açıklaması:  
Veri, yüksek boyuttan düşük boyuta indirgenir.  
Esas yapı bozulmadan görselleştirilir.

---

#### 🔹 Association Rule Learning (Birliktelik Kuralları - Apriori)

Veriler arasındaki ilişkileri bulur.  
Bir ürün alındığında başka hangi ürünün alınacağını gösterir.

Ex: Bebek bezi alanlar genellikle bira da alır.  
Bu ilişki bulunur.  
Market raflarına yerleştirilir.

> Grafik Açıklaması:  
Ürünler arası bağlantılar çizilir.  
En sık birlikte alınan ürünler gösterilir.

---

## 3. Pekiştirmeli Öğrenme (Reinforcement Learning)

**Temel Kavramlar**
- **Ajan (Agent)**: Öğrenen sistem
- **Ortam (Environment)**: Etkileşim kurulan dünya
- **Ödül (Reward)**: İstenen davranış için pozitif geri bildirim
- **Politika (Policy)**: Durumlara karşı alınacak aksiyonların haritası

**Uygulama Örnekleri**
1. Oyun AI'ları (AlphaGo)
2. Otonom sürüş sistemleri
3. Robotik kontrol
4. Reklam teklif optimizasyonu

Burada bilgisayar deneyerek öğrenir.  
Her karar için ödül veya ceza alır.  
Zamanla en çok ödülü veren strateji öğrenilir.

Ex: Otonom araç sürüyor.  
Sağa dönünce çarpıyor → ceza  
Düz gitmeyi öğreniyor → ödül  

---

### Yaygın Pekiştirmeli Öğrenme Algoritmaları

**Popüler Algoritmalar**
- Q-Learning
- Deep Q Network (DQN)
- Policy Gradient Methods

#### 🔹 Q-Learning

Ödül tablosu oluşturur.  
Her eylem için bir ödül değeri saklanır.  
En yüksek ödül veren yol tercih edilir.

Ex: Robot süpürge, en kısa yoldan temizlemeyi öğrenir.

> Grafik Açıklaması:  
Robotun izlediği yollar gösterilir.  
Ödüllü yollar yeşil, cezalı yollar kırmızı olabilir.

---

#### 🔹 Deep Q Network (DQN)

Q-learning'e derin öğrenme katılır.  
Daha karmaşık sistemlerde çalışır.  
CNN gibi görüntü işlemeyle beraber çalışır.

Ex: Atari oyunlarında en yüksek skoru yapan AI.

> Grafik Açıklaması:  
Oyun ekranı + AI'nın aldığı kararlar  
Her karar ödül/ceza ile değerlendirilir.

---

## Karşılaştırmalı Tablo: ML Yöntemleri

| Özellik | **Gözetimli** | **Gözetimsiz** | **Pekiştirmeli** |
|--------|------------------|------------------|--------------------|
| **Veri Tipi** | Girdi + Çıktı | Sadece girdi | Eylem + Ödül/Ceza |
| **Amacı** | Tahmin veya sınıflandırma | Gruplama veya desen bulma | Optimize edilmiş karar almak |
| **Kullanım Alanı** | Fiyat tahmini, spam tespiti | Müşteri segmentasyonu | Otonom araçlar |

---

## Hangi Algoritma Ne Zaman?

### Algoritma Seçim Kılavuzu

| Problem Türü | Önerilen Algoritmalar |
|--------------|-----------------------|
| Sınıflandırma | Logistic Regression, Random Forest, SVM |
| Regresyon | Linear Regression, Decision Trees, XGBoost |
| Kümeleme | K-Means, DBSCAN, Hierarchical |
| Boyut İndirgeme | PCA, t-SNE, UMAP |
| Sıralı Karar Verme | Q-Learning, DDPG, PPO |


| Problem Türü | Uygun Algoritma |
|--------------|------------------|
| Ev fiyat tahmini | Linear Regression |
| Spam tespiti | Logistic Regression, Naive Bayes |
| Müşteri segmentasyonu | K-Means Clustering |
| Ürün önerisi | Association Rules |
| Otonom karar verme | Reinforcement Learning |
| Yüksek boyutlu veri | PCA |
| Riskli müşteri tespiti | Random Forest, XGBoost |

Hiçbir algoritma tüm problemler için en iyisi değildir. Model seçimi veri yapısına, problem gereksinimlerine ve performans ölçütlerine göre yapılmalıdır.

---

## Son Söz

Makine Öğrenmesi algoritmaları,  
sayılardan anlamlı bilgi çıkaran araçlardır.

Bazıları veriyle öğrenir.  
Bazıları verisiz öğrenir.  
Bazıları deneyerek öğrenir.

Veri bilimi projelerinde  
her problem farklıdır.  
Her çözüm özel hazırlanmalıdır.

Çünkü makine öğrenmesi;  
veriden bilgiye ulaşmanın  
en güçlü yollarından biridir.

---

