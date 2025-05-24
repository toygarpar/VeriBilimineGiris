# Veri Bilimi Araçları

## Sayılarla Çalışmak İçin Gerekli Araçlar

Veri bilimi sadece kuramdan ibaret değildir.  
Gerçek hayatta sayılarla çalışır.  
Bunun için doğru araçlara ihtiyaç vardır.

Her işte olduğu gibi,  
veri biliminde de doğru aletle iş daha kolay olur.

Python, R, SAS, RapidMiner…  
Bütün bu araçlar veriyi anlamak için kullanılır.

AMA her biri farklıdır.  
Her biri özel bir iş yapar.

---

## 1. Python – Veri Biliminin En Güçlü Dili

## Python'un Veri Bilimindeki Yeri

Python, veri bilimciler için en popüler programlama dili olarak öne çıkıyor. Bunun temel nedenleri:

- **Zengin ekosistem**: 200.000'den fazla kütüphane
- **Öğrenme kolaylığı**: Sade ve okunabilir sözdizimi
- **Topluluk desteği**: Aktif geliştirici topluluğu
- **Çok yönlülük**: Veri analizinden web geliştirmeye geniş kullanım alanı

Python, veri bilimcilerin en çok kullandığı programlama dilidir.  
Okunabilirliği vardır.  
Basit sözdizimi vardır.  
Ve güçlü kütüphaneleri vardır.

### Neden Python?
- Öğrenmesi kolaydır.  
- Büyük topluluk desteği vardır.  
- Hem küçük projelerde hem büyük veri analizlerinde çalışır.  
- Makine öğrenmesi, görselleştirme, web scraping, veri madenciliği için uygun.

---

## Python ile Veri Bilimi: Ana Kategoriler

### 🔹 Veri Toplama
Veriyi almanın yolları vardır.  
Web sitelerinden, veritabanlarından, API’lerden alınır.

#### Kullanılan Kütüphaneler:
- `requests`: Web sayfalarından veri çeker.  
- `BeautifulSoup`: HTML’i inceler.  
- `Scrapy`: Web scraping için güçlü bir çerçeve.  
- `SQLAlchemy`, `psycopg2`, `pymongo`: SQL ve NoSQL veritabanlarıyla iletişim kurar.

> **Örnek Kod:**
```python
import requests

x = requests.get("toygarpar.com.tr")
print(x.text)
```
- **BeautifulSoup**: Web scraping için
  ```python
  from bs4 import BeautifulSoup
  soup = BeautifulSoup(response.text, 'html.parser')
  ```
- **Veritabanı Bağlantıları**:
  - PostgreSQL: `psycopg2`
  - MongoDB: `pymongo`
  - Oracle: `cx_Oracle`

> Grafik Açıklaması:  
API → Python kodu → JSON / HTML verisi → Temizleniyor → Analiz ediliyor  

---

### 🔹 Veri Ön İşleme
Veri gelir ama hemen kullanılmaz.  
Temizlenir. Düzenlenir. Hazırlanır.

#### Kullanılan Kütüphaneler:
- `pandas`: Veriyi düzenlemek için ana araçtır.  
- `numpy`: Sayısal işlemler için temeldir.  
- `scipy`: İleri düzey hesaplamalar için.  
- `scikit-learn`: ML süreci öncesi hazırlıklar için.  
- `dask`: Büyük veri işleme için.  

> Grafik Açıklaması:  
Ham veri → Pandas ile temizleniyor → Gözlem yapılıyor → ML modeline hazırlanıyor  

- **Pandas**: Veri manipülasyonunun iskeleti
  ```python
  import pandas as pd
  df = pd.read_csv('veri.csv')
  df.head()
  ```
- **NumPy**: Bilimsel hesaplamalar
  ```python
  import numpy as np
  array = np.array([1, 2, 3])
  ```
- **Dask**: Büyük veri setleri için paralel işlem
---

### 🔹 Veri Görselleştirme
Sayılar bazen sessiz kalır.  
Görseller konuşur.  
Verinin hikâyesini anlatır.

#### Kullanılan Kütüphaneler:
- `matplotlib`: Temel grafik çizimi.  
- `seaborn`: Daha güzel görünümlü grafikler.  
- `plotly`: Etkileşimli görselleştirme.  
- `bokeh`: Dinamik veri görselleştirmeleri.  
- `altair`: Basit ve akıcı görseller.  
- `pyplot3d`: Üç boyutlu görselleştirme.  

> Grafik Açıklaması:  
Histogram, dağılım grafiği, çizgi grafiği örnekleri  

- **Matplotlib**: Temel çizimler
  ```python
  import matplotlib.pyplot as plt
  plt.plot([1, 2, 3])
  plt.show()
  ```
- **Seaborn**: İstatistiksel görselleştirme
- **Plotly**: Etkileşimli grafikler

---

### 🔹 Makine Öğrenmesi ve Derin Öğrenme
Model kurmak için gerekli araçlar burada yer alır.

#### Kullanılan Kütüphaneler:
- `scikit-learn`: Temel ML modelleri.  
- `tensorflow`, `keras`, `pytorch`: Derin öğrenme için.  
- `h2o`: Otomatik makine öğrenimi.  

> Grafik Açıklaması:  
Veri → Model eğitimi → Tahmin çıktısı diyagramı  

- **Scikit-learn**: Klasik ML algoritmaları
  ```python
  from sklearn.linear_model import LinearRegression
  model = LinearRegression()
  model.fit(X_train, y_train)
  ```
- **TensorFlow/PyTorch**: Derin öğrenme çerçeveleri

## Python ile Veri Analizi Örneği

```python
# Veri yükleme ve temel analiz
import pandas as pd

# CSV dosyasını yükle
df = pd.read_csv('satislar.csv')

# İlk 5 satırı göster
print(df.head())

# Temel istatistikler
print(df.describe())

# Eksik veri kontrolü
print(df.isnull().sum())

# Sütun veri tipleri
print(df.dtypes)
```


---

### 🔹 Gerçek Zamanlı ve Büyük Veri
Python, sadece küçük verilerle çalışmaz.  
Büyük verilerle, gerçek zamanlı sistemlerle de çalışır.

#### Kullanılan Araçlar:
- `pyspark.streaming`: Akış verisini işler.  
- `apache.flink`: Yüksek performanslı analiz.  
- `pyspark`, `dask`, `vaex`, `modin`: Büyük veri için.  

> Grafik Açıklaması:  
Datalake → Spark ile işlem → Gerçek zamanlı çıktı  

## Büyük Veri için Python Araçları

1. **PySpark**:
   - Dağıtık veri işleme
   - SQL benzeri sorgulama yetenekleri

2. **Vaex**:
   - Milyarlarca satırlık veri setleri
   - Bellek verimliliği

3. **Modin**:
   - Pandas API'siyle uyumlu
   - Çok çekirdekli işlem

---

## Diğer Programlama Dilleri ve Araçlar

### 1. **R Programlama**
Veri analizi için özel olarak geliştirildi.  
İstatistiksel analizlerde güçlüdür.  
AMA büyük veride yavaş kalır.

Ex:  
Regresyon, hipotez testi, istatistiksel raporlama için idealdir.

---

### 2. **Matlab ve Octave**
Mühendislik ve matematiksel hesaplamalarda kullanılır.  
AMA lisans maliyeti yüksektir.  
Octave, Matlab’a benzer ama ücretsizdir.

Ex:  
Sinyal işleme, görüntü analizi, optimizasyon  

---

### 3. **SAS (Statistical Analysis System)**
Finans ve sağlık sektöründe yaygın kullanılır.  
Lisanslıdır.  
AMA güvenilir sonuçlar verir.

Ex:  
Risk analizi, kredi skorlaması  

---

### 4. **Julia**
Yeni nesil dildir.  
Hızlı çalışır.  
AMA henüz çok yaygın değildir.

Ex:  
Sayısal hesaplamalar, simülasyonlar  

---

### 5. **RapidMiner & KNIME**
GUI tabanlı veri bilimi platformlarıdır.  
Kod yazmadan model kurulabilir.  
AMA esneklik azdır.

Ex:  
Akademik araştırmalar, hızlı prototipleme  

---

## Karşılaştırmalı Tablo: Veri Bilimi Araçları

| Özellik | **Python** | **R** | **SAS** | **MATLAB/Octave** | **Julia** | **RapidMiner / KNIME** |
|--------|------------|--------|-----------|--------------------|-------------|--------------------------|
| **Veri Toplama** | Var | Sınırlı | Var | Yok | Az | Yok |
| **Veri Ön İşleme** | Çok güçlü | Güçlü | Orta | Orta | Hızlı | Kolay |
| **Görselleştirme** | Seaborn, Plotly | ggplot2 | Enterprise | MATLAB plot | Yüksek performans | GUI üzerinden |
| **ML/DL** | TensorFlow, PyTorch | Caret, randomForest | Enterprise Tools | Yok | Flux.jl | Arayüzle model kurma |
| **Kodlama Gereksinimi** | Var | Var | Var | Var | Var | Yok |
| **Kullanım Kolaylığı** | Kolay | Orta | Zor | Orta | Orta | Çok kolay |

---

## Hangi Araç Ne Zaman?

| Problem Türü | Uygun Araç |
|--------------|-------------|
| Küçük veri analizi | Python, R |
| Büyük veri analizi | Python (PySpark, Dask) |
| İstatistiksel analiz | R |
| Finansal risk analizi | SAS |
| Mühendislik hesaplamaları | MATLAB, Julia |
| Kod yazmadan model kurmak | RapidMiner, KNIME |

---

## Jupyter Notebook ile Çalışma

Veri bilimciler için vazgeçilmez bir araç:
- Hücre tabanlı yürütme
- Markdown desteği
- Görselleştirme entegrasyonu

```bash
# Kurulum
pip install jupyterlab

# Başlatma
jupyter notebook
```

Python, veri bilimi projelerinin tüm aşamalarında - veri toplamadan model dağıtımına kadar - kapsamlı bir çözüm sunar. Doğru araçların seçimi ve etkili kullanımıyla, karmaşık veri problemlerine elegant çözümler geliştirilebilir.

---

## Son Söz

Veri bilimi, doğru araç olmadan yürümeyen bir yoldur.  
Python ile yürümek en hızlı yoldur.  
AMA diğer araçlar da unutulmamalıdır.

Her aracın güçlü bir yönü vardır.  
AMA hepsi aynı şey değildir.

Bazıları kodla çalışır.  
Bazıları arayüzle çalışır.  
Bazıları ise sadece belirli alanlarda uygundur.

Sen hangi aracı seçersen seç,  
veriyi anlamak hep ön planda olmalı.  
Çünkü veri bilimi;  
sayılardan anlam çıkarmaktır.  
Araçlar ise bunun anahtarıdır.

---

