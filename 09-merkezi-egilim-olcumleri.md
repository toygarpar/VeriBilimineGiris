# Merkezi Eğilim Ölçümleri

Merkezi eğilim ölçümleri, bir veri kümesinin genel eğilimini ya da ortalama davranışını belirlemeye yarayan istatistiksel göstergelerdir. Verilerin merkezi değerine dair fikir verirler.

## Sayıların Ortası Nerede?

Bazen sayılar çok fazla olur.  
Dağınık gibi görünür.  
Ama hepsi bir merkeze doğru çeker.  

İstatistikte bu merkeze ulaşmak için üç ana yol vardır:  
**Ortalama (Mean)**  
**Medyan (Median)**  
**Mod (Mode)**  

Her biri farklıdır.  
Her biri farklı bir şey anlatır.  
Ve her biri farklı durumlarda işe yarar.

---

## 1. Ortalama – Mean

Bir veri kümesindeki tüm değerlerin toplamının, değer sayısına bölünmesiyle elde edilir.

Ortalama, en bilinen ölçüm türüdür.  
Tüm sayıları toplarsın.  
Kaç tane varsa ona bölersin.  
Çıkan sayı, genelin ortalamasıdır.

### Nasıl Hesaplanır?

1. **Sayıları topla.**  
2. **Eleman sayısına böl.**

### Örnek:

Matematik sınav notları:  
70, 80, 90, 60, 75  

Toplam: 375  
Sayı adedi: 5  

**Ortalama = 375 / 5 = 75**

### Formülü:
```
Ortalama = (x₁ + x₂ + x₃ + ... + xₙ) / n
```

Burada:  
x = her bir veri noktası  
n = toplam veri sayısı

### Ne Zaman Kullanılır?

- Veriler düzenliyse  
- Aşırı yüksek ya da düşük değer yoksa  
- Genel eğilimi görmek istiyorsak  

### Dezavantajı Nedir?

Ortalama, aşırı büyük ya da küçük değerlere karşı hassastır.  
Bir kişi çok yüksek maaş alıyorsa, ortalama gerçekliği yansıtmayabilir.

---

## 2. Medyan – Median

Medyan, sıralanmış bir veri listesindeki ortadaki sayıdır. Çift sayıda değer varsa, ortadaki değer aslında veri kümesinde olmayan, bunun yerine sıralanmış veriyi üst ve alt yarılara bölen iki değerin ortalamasıdır.

Medyan, sayıların ortasındaki değerdir.  
Sayıları sıralarsın.  
Tam ortadaki sayı medyandır.

### Nasıl Bulunur?

1. **Sayıları küçükten büyüğe sırala.**  
2. **Eğer tek sayı varsa, ortadaki sayı medyandır.**  
3. **Eğer çift sayı varsa, ortadaki iki sayının ortalaması alınır.**

### Örnekler:

- **Tek eleman:** 2, 4, **6**, 8, 10 → Medyan: 6  
- **Çift eleman:** 1, 3, **5**, **7**, 9, 11 → Medyan: (5 + 7) / 2 = 6

### Ne Zaman Kullanılır?

- Aşırı değerler varsa  
- Daha gerçekçi bir orta nokta isteniyorsa  
- Gelir dağılımı, ev fiyatları gibi alanlarda  

### Özellikleri:

- **Aşırı değerlere daha dayanıklıdır.**  
- **Veriler sıralandığında daha güvenilirdir.**

---

## 3. Mod – Mode

Mod, en çok tekrar eden sayıdır.  
En sık görülen değerdir.

✔️ Özellik:
Birden fazla mod olabilir (çok modlu dağılım).

Aritmetik ortalama ya da medyanın yeterli olmadığı durumlarda anlamlı olabilir.

Özellikle kategorik veriler için kullanışlıdır.

### Nasıl Bulunur?

Sayılara bak.  
Hangisi en çok tekrar ediyor?  
O sayı moddur.

### Örnek:

Notlar: 70, 80, 70, 90, 70, 60  
**Mod = 70** (3 kez tekrar ediyor)

### Ne Zaman Kullanılır?

- Kategorik verilerde (örneğin: favori renk, marka tercihi)  
- En popüler seçeneği bulmak istediğimizde  
- Bir dağılımın zirvesini görmek istediğimizde  

### Özellikleri:

- **Formülü yoktur.**  
- **Algoritmik olarak bulunur.**  
- **Birden fazla mod olabilir.**

---

## Ortalama, Medyan, Mod – Hangisini Kullanmalı?

| Özellik | Ortalama | Medyan | Mod |
|--------|----------|--------|-----|
| **Hassasiyet** | Aşırı değerlere duyarlı | Daha dayanıklı | Sadece tekrar edenleri gösterir |
| **Veri Türü** | Sayısal | Sayısal | Hem sayısal hem kategorik |
| **Nasıl Hesaplanır?** | Toplama ve bölme | Sıralama ve orta değer | En çok tekrar eden |
| **Kullanım Alanı** | Genel eğilim | Uç değer varsa | Popüler değerleri bulmak |

---

## Son Söz

Sayılar bazen çok fazla olur.  
Ne olduğunu anlamak zorlaşır.  
Ama ortalama, medyan ve mod bize yardım eder.  

**Ortalama** geneli gösterir.  
**Medyan** uç değerlerden korur.  
**Mod** en popüler olanı vurgular.  

Biri yeterli değilse, diğerine başvur.  
Sayıların ortasını bulmak için üç yolun var.  
Onları iyi tanı.

---
