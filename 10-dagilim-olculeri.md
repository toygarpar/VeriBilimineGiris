# Dağılım Ölçüleri

| Ölçü Türü         | Temsil Ettiği | Yöntemler                  | Özellikler                           |
| ----------------- | ------------- | -------------------------- | ------------------------------------ |
| Merkezi Eğilim    | Tipik Değer   | Ortalama, Medyan, Mod      | Verinin merkezi hakkında bilgi verir |
| Dağılım (Varyans) | Yayılım       | Range, Varyans, Std. Sapma | Verinin nasıl dağıldığını gösterir   |

```python
import numpy as np

veriler = [4, 8, 6, 2]
print("Ortalama:", np.mean(veriler))
print("Medyan:", np.median(veriler))
print("Varyans:", np.var(veriler))
print("Standart Sapma:", np.std(veriler))

```

Bir veri kümesinin ne kadar yayıldığını gösteren sayılardır. Yani, veriler birbirine yakın mı, yoksa uzak mı? İşte bunu anlamamıza yardım eder.


## Sayıların Ne Kadar Yayıldığını Öğrenmek

Sayılar bazen bir arada durur.  
Bazen çok uzaklaşır.  
Bu fark önemlidir.  
Çünkü verilerin nasıl dağıldığını bilmek, onları anlamamızı sağlar.

Dağılım ölçüleri, verilerin ne kadar çeşitlendiğini ya da ne kadar benzer olduğunu gösterir.

Üç temel dağılım ölçüsü vardır:  
**Değişim Aralığı (Range)**  
**Varyans**  
**Standart Sapma**

Her biri farklı bir şey anlatır.  
Ama hepsi aynı amaca hizmet eder:  
Verilerin yayılımını görmek.

---

## 1. Değişim Aralığı – Range

En büyük değerle en küçük değer arasındaki farktır.
Basitçe:
Değişim Aralığı = En büyük değer - En küçük değer

En basit dağılım ölçüsüdür.  
Sadece en yüksek ve en düşük değere bakılır.  
Aradaki fark alınır.  
Bu fark bize verinin ne kadar geniş yayıldığını söyler.

### Nasıl Hesaplanır?

1. **En yüksek değeri bul.**  
2. **En düşük değeri bul.**  
3. **İkisini çıkar.**

### Örnek:

Notlar: 40, 50, 60, 70, 100  
En yüksek = 100  
En düşük = 40  
**Değişim Aralığı = 100 - 40 = 60**

### Özellikleri:

- **Basittir.**  
- **Yalnızca iki değerle çalışır.**  
- **Uç değerlere duyarlıdır.**

---

## 2. Varyans

Verilerin ortalamadan ne kadar saptığını gösterir.
Tüm değerlerin ortalamaya olan uzaklıklarının karelerinin ortalamasıdır.

Daha derine iner.  
Tüm sayıların ortalamaya göre sapmasını ölçer.  
Sayılar ortalamanın etrafında nasıl dağılmış?  
Bu sorunun cevabını verir.

### Nasıl Hesaplanır?

1. **Ortalamayı hesapla.**  
2. **Her sayının ortalamadan farkını bul.**  
3. **Farkların karesini al.**  
4. **Karelerin toplamının ortalamasını al.**
5. **Popülasyonsa, eleman sayısına böl. Örneklemse, (n-1)'e böl.**


### Formülü:

**Popülasyon Varyansı:**  
σ² = Σ(xᵢ – μ)² / N  

**Örneklem Varyansı:**  
s² = Σ(xᵢ – x̄)² / (n – 1)

Burada:  
xᵢ = her bir veri noktası  
μ = popülasyon ortalaması  
x̄ = örneklem ortalaması  
n = örneklem sayısı  
Σ = toplam sembolü

### Örnek:

Sayılar: 4, 8, 6, 2  
Ortalama = 5  
Farklar = -1, 3, 1, -3  
Kareler = 1, 9, 1, 9  
Toplam = 20  
Varyans = 20 / 4 = 5

### Özellikleri:

- **Sayıların ortalamadan sapmasını gösterir.**  
- **Yüksek varyans = geniş dağılım**  
- **Düşük varyans = dar dağılım**

---

## 3. Standart Sapma

Verilerin ortalamadan ne kadar uzaklaştığını gösteren daha anlaşılır bir ölçüdür.
Birimi, verinin birimiyle aynıdır. Bu yüzden yorumlaması kolaydır.

Varyansın kareköküdür.  
Yani varyans gibi çalışır ama daha yorumlanabilir bir ölçüdür.  
Çünkü orijinal verilerin birimleriyle ifade edilir.

### Nasıl Hesaplanır?

1. **Varyansı hesapla.**  
2. **Karekökünü al.**

### Formülü:

**Popülasyon Standart Sapması:**  
σ = √[Σ(xᵢ – μ)² / N]

**Örneklem Standart Sapması:**  
s = √[Σ(xᵢ – x̄)² / (n – 1)]

### Örnek:

Varyans = 5  
**Standart Sapma = √5 ≈ 2.24**

### Özellikleri:

- **Varyansın daha anlaşılır halidir.**  
- **Verilerin ne kadar yayıldığını gösterir.**  
- **Yüksek standart sapma = veriler çok değişken. Veriler ortalamadan uzak.**  
- **Düşük standart sapma = veriler homojen. Veriler birbirine yakın, ortalamaya sadık.**

---

## Hangi Ölçüyü Kullanmalı?

| Özellik | Değişim Aralığı | Varyans | Standart Sapma |
|--------|------------------|---------|----------------|
| **Karmaşıklık** | En basit | Orta | Orta |
| **Duyarlılık** | Uç değerlere duyarlı | Ortalamaya göre | Ortalamaya göre |
| **Kullanım Alanı** | Temel analizler | İstatistiksel testler | Geniş kullanım alanı |

---

## Son Söz

Sayılar sadece ortalama ile anlatılmaz.  
Onların nasıl dağıldığını da bilmek gerekir.

**Değişim Aralığı** başlangıçtır.  
**Varyans** daha derin bilgi verir.  
**Standart Sapma** ise en güçlü araçtır.

Bu üç ölçüyü birlikte kullanmak,  
sayıların ne kadar değiştiğini,  
ne kadar tutarlı olduğunu  
ve ne kadar uç noktalar içerdiğini gösterir.

Ve bu bilgiler olmadan  
veri hakkında doğru karar veremezsin.

---

