# Keşifsel Veri Analizi (EDA)

## Veriyi Tanımaya Başlamak

Veri gelir.  
Hamdır.  
Düzensizdir.  
Bazı satırlar eksiktir.  
Bazı sütunlar anlamsızdır.  

İlk adım: veriyi tanımak.  
Sayıların içinde saklı olan hikâyeyi bulmak.  
Bu yüzden EDA yapılır.

**EDA – Exploratory Data Analysis**,  
verinin yapısını, dağılımını, ilişkilerini anlamak için yapılan ilk analizdir.

## EDA Nedir ve Neden Önemlidir?

Keşifsel Veri Analizi (EDA), veri bilimi sürecinin en kritik aşamalarından biridir. Veri setinizin yapısını, özelliklerini ve altında yatan ilişkileri anlamanızı sağlayan bir dizi teknik ve yöntem içerir.

**Temel Amaçlar:**
- Verinin genel yapısını ve içeriğini anlamak
- Potansiyel veri kalitesi sorunlarını tespit etmek
- Değişkenler arasındaki ilişkileri keşfetmek
- Analiz ve modelleme için hipotezler oluşturmak
- Uygun ön işleme tekniklerini belirlemek

---

## Neden EDA Yapılır?

### 1. Veriyi Derinlemesine Anlamak İçin  
Veri setinde hangi sütunlar var?  
Ne tür veriler taşıyorlar?  
Sayı mı? Metin mi? Tarih mi?

Her şey burada başlar.  
Veriyle tanışma sürecidir EDA.


### 2. Sorunları Belirlemek İçin  
Eksik değerler var mı?  
Yanlış değerler yer alıyor mu?  
Aykırı gözlemler var mı?

EDA, verideki hastalıkları gösterir.  
Onları görebilirsin.  
Ve onları düzeltebilirsin.

### 3. Kaliteyi Artırmak İçin  
Veri güvenilir mi?  
Tutarlı mı?  
Doğru mu?

Kaliteli veri, kaliteli karar demektir.  
EDA ile veriye kalite katarız.

### 4. Hipotez Üretmek İçin  
Veri bir hikâye anlatır.  
Desenleri vardır.  
Eğilimleri vardır.  
Bu desenleri kullanarak gelecek hakkında hipotez kurabiliriz.

---

## EDA Adımları

EDA'da işler sistemli ilerler.  
Hiçbir adımı atlanmaz.  
Her adımı önemli.

### 1. Veri Setine İlk Bakış  
`df.head()` ve `df.tail()` komutlarıyla veriyi görürüz.  
İlk birkaç satırı inceleriz.  
Son birkaç satırı da.

Ne içeriyor bu veri?  
Nasıl yapılandırılmış?  
Bu soruların cevabı burada başlar.

Veriye İlk Bakış:

```python
# İlk 5 gözlem
df.head()

# Son 5 gözlem 
df.tail()

# Veri seti boyutları (satır, sütun)
print(f"Satır sayısı: {df.shape[0]}, Sütun sayısı: {df.shape[1]}")

# Veri yapısı hakkında bilgi
df.info()
```


### 2. Boyutu Kontrol Et  
Kaç satır var?  
Kaç sütun var?

`df.shape`, `df.ndim`, `df.size` ile boyutu öğreniriz.  
Veri büyük mü? Küçük mü?  
Hangi boyutta çalışacağımızı anlarız.

### 3. Sütun Bilgilerini Gözden Geçir  
Her sütun ne ifade ediyor?  
Veri tipi nedir?  
Boş değerler nerede?

`df.info()` ile tüm bu bilgilere ulaşırız.  
Veri setini tanımanın anahtarıdır bu.

### 4. Özet İstatistiklere Bak  
Ortalama nedir?  
Standart sapma kaçtır?  
En küçük ve en büyük değerler neler?

`df.describe().T` ile merkezi eğilimleri ve yayılımı görürüz.

Temel İstatistiklerin İncelenmesi:

```python
# Sayısal değişkenler için özet istatistikler
df.describe().T

# Kategorik değişkenler için özet
df.describe(include=['object'])
```


### 5. Eksik Verileri, Aykırı Değerleri Tespit Et  
Eksik hücre var mı?  
Hangi sütun daha çok etkilenmiş?
Aykırı değerler/Outliers bulunuyor mu?

`df.isnull().sum()` ile eksiklikleri sayarız.  
Ve gerekirse düzeltiriz.

Eksik Veri Analizi: 

```python
# Eksik değerlerin toplamı
df.isnull().sum()

# Eksik değer yüzdeleri
(df.isnull().sum() / len(df)) * 100

# Eksik değer görselleştirme
import missingno as msno
msno.matrix(df)
```

Aykırı Değer Analizi:

```python
# Boxplot ile aykırı değerlerin tespiti
import seaborn as sns
sns.boxplot(data=df, x='numeric_column')

# Z-skoru ile aykırı değer tespiti
from scipy import stats
z_scores = stats.zscore(df['numeric_column'])
abs_z_scores = np.abs(z_scores)
outliers = (abs_z_scores > 3)
```

### 6. Gelişmiş Analizler

Dağılım Analizi:

```python
# Histogram
df['numeric_column'].hist(bins=30)

# Yoğunluk grafiği
sns.kdeplot(df['numeric_column'])

# Q-Q plot (normallik testi)
import statsmodels.api as sm
sm.qqplot(df['numeric_column'], line='s')
```

Korelasyon Analizi:

```python
# Korelasyon matrisi
corr_matrix = df.corr()

# Isı haritası
sns.heatmap(corr_matrix, annot=True)

# Scatter plot
sns.scatterplot(data=df, x='var1', y='var2')
```

Zaman Serisi Analizi:

```python
# Zaman serisi görselleştirme
df.set_index('tarih_değişkeni')['sayısal_değişken'].plot()

# Hareketli ortalama
df['moving_avg'] = df['sayısal_değişken'].rolling(window=7).mean()
```

Çok Değişkenli Analiz:

```python
# Pairplot
sns.pairplot(df)

# FacetGrid
g = sns.FacetGrid(df, col="kategorik_değişken")
g.map(sns.histplot, "sayısal_değişken")
```

Kategorik Değişken Analizi:

```python
# Bar plot
sns.countplot(data=df, x='kategorik_değişken')

# Cross tabulation
pd.crosstab(df['var1'], df['var2'])
```


### 7. Görselleştirme  
Sayılar bazen sessiz kalır.  
Görseller konuşur.

Histogramlar çizeriz.  
Çizgi grafikleri yaparız.  
Dağılım grafikleriyle ilişki ararız.

Veri görsel olunca anlaşılır olur.

---

## EDA Sonrası Aksiyonlar

1. **Eksik Veri Stratejisi Belirleme**:
   - Silme
   - Doldurma (ortalama, medyan, mod)
   - Modelleme ile tahmin

2. **Aykırı Değer Yönetimi**:
   - Düzeltme
   - Dönüştürme
   - Kaldırma

3. **Veri Dönüşümleri**:
   - Normalizasyon
   - Standardizasyon
   - Log dönüşümü

4. **Özellik Mühendisliği**:
   - Yeni değişkenler türetme
   - Kategorik kodlama
   - Boyut azaltma

## Son Söz

EDA, veriyle tanışma partisidir.  
Veriyi dinleyip onunla konuşmaktır.  
Sayıların arasında yatan gerçekleri bulmaktır.

Veri bilimi projelerinde EDA,  
analiz sürecinin kapısıdır.  
Model kurmadan önce yapılmalıdır.  
Çünkü model, yanlış veriyle yanlış sonuç verir.

EDA olmadan analiz,  
yolculuk plan yapmadan gitmeye benzer.  
Nereye gittiğini bilmezsin.  
Neye dayandığını anlamazsın.

Ama EDA ile yol belli olur.  
Veriyle el ele yürünür.  
Analizler daha tutarlı olur.

---

