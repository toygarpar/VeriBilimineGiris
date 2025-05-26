# Hipotez Testleri

Bir konuda fikriniz varsa ve bunu veriyle sınamak istiyorsanız, hipotez kurarsınız.

Hipotez nedir?
Bir tahmin. Bir iddia.
Doğru olabilir. Yanlış da.
Ama önemli olan, bunu kanıtlamaya çalışmaktır.

## Gerçek mi, Yoksa Rastgelelik mi?

Bazen bir iddia duyarız.  
“Türkiye’deki erkeklerin ortalama boyu 172 cm’dir.”  
Ama bu doğru mudur?  
Gerçek midir?  
Yoksa sadece bir tahmin mi?

İşte bu sorulara cevap veren yönteme **hipotez testi** denir.  
Sayılarla iddiaları sınar.  
Verilerle karar veririz.

---

## Hipotez Nedir?

Hipotez, belirli bir konuda yapılan bir tahmindir.  
Doğru da olabilir, yanlış da.  
Ama önemli olan: test edilebilmesidir.

Bilimsel araştırmalarda hipotez, verilerle sınanır.  
Ve sonunda karar verilir:  
Kabul mu? Red mi?

## HİPOTEZ TESTİ NEDİR?
Hipotezin doğru mu, değil mi diye sorgulanmasıdır.
Veri toplanır. İncelenir. Sonuç çıkarılır.

Bu işte iki taraf vardır:

H0 (Sıfır Hipotezi): “Bir fark yoktur.” der.

H1 (Alternatif Hipotez): “Fark vardır.” diye karşı çıkar.

---

## İki Tür Hipotez Var

Örnek: Türkiye’de Erkeklerin Boy Ortalaması
Diyelim ki birisi iddia etti:

"Türkiye’deki erkeklerin boy ortalaması 1.72 metredir."

Bunu test etmek isteriz.

H0: Ortalama = 1.72

H1: Ortalama ≠ 1.72

### 1. Sıfır Hipotezi – H₀  
Varsayılan durumdur.  
Şu anki durumu temsil eder.  
Değişim yoktur.  
Eski yöntem işe yarar.  

Ex: “Erkeklerin ortalama boyu 172 cm’dir.”

### 2. Alternatif Hipotez – H₁ veya Hₐ  
Yeni iddiadır.  
Değişimin olduğunu göstermeye çalışır.  
Yeni bir şey önerir.  

Ex: “Erkeklerin ortalama boyu 172 cm değildir.”

---

## Hangi Testi Kullanacağız?

Test iki ana faktöre bağlıdır:  
- Örneklem büyüklüğü  
- Bilinen bilgiler (varyans, standart sapma)

### T-Testi  
Küçük örneklemlerde kullanılır.  
Genellikle örneklem sayısı 30’dan küçükse tercih edilir.

### Z-Testi  
Büyük örneklemlerde kullanılır.  
Genellikle 30’dan büyükse tercih edilir.  
Standart sapma biliniyorsa da Z-testi yapılır.

---

## Bir Örnek Üzerinden Gidelim

### İddia:
Türkiye’deki erkeklerin ortalama boyu 172 cm’dir.

### Hipotezler:
- H₀ = Ortalama boy = 172 cm  
- H₁ ≠ 172 cm (Ortalama farklı mı?)

40 milyon erkeğin boyunu ölçmek mümkün değil.  
Bu yüzden rastgele 100 kişi seçiyoruz.

Sonuçlar:
- Ortalama (mean) = 174 cm  
- Standart Sapma (std) = 5 cm  
- Örneklem sayısı (n) = 100  

Z-Testi yapacağız çünkü örneklem büyük.

### Formül:
```
Z = (Örneklem Ortalaması - H₀ Değeri) / (Standart Sapma / √n)
```

### Hesaplama:
```
Z = (174 - 172) / (5 / √100) = 2 / 0.5 = 4
```

---

## Anlamlılık Düzeyi ve P-Değeri

İstatistikte hata payı belirleriz.
Bu genelde %5’tir. Yani alfa = 0.05 deriz.

Eğer hesapladığımız p-değeri, bu 0.05’ten küçükse, H0 hipotezini reddederiz.

Z değerimiz = 4 olduğunda, z-tablosuna göre:
P-değeri = 0.000063

Bu, alfadan çok daha küçük.

Sonuç: H0 reddedilir.
Yani: “Türkiye’deki erkeklerin boy ortalaması gerçekten 1.72 değil.”

### Anlamlılık Düzeyi – α  
Ne kadar hata kabul edilebilir?  
Genelde %5 alınır.  
Yani α = 0.05  

### P-Değeri  
Z değerine karşılık gelen olasılıktır.  
Bizim örneğimizde p-value = 0.000063

### Karar Kuralı:
- Eğer p-value < α → H₀ reddedilir.  
- Eğer p-value ≥ α → H₀ reddedilemez.

Burada p-value çok küçük.  
α = 0.05’ten çok daha düşük.  
Yani iddia geçersiz.  
Türkiye’deki erkeklerin ortalama boyu 172 cm değildir.

---

## Tek Yönlü mü, İki Yönlü mü?

### İki Yönlü Test  

Eğer hem artış hem azalış düşünülüyorsa: İki Yönlü Test

Alternatif hipotez "farklıdır" der.  
Boy ortalaması hem daha büyük hem de daha küçük olabilir.  
Dolayısıyla her iki yöne bakılır.

### Tek Yönlü Test  

Eğer sadece artış ya da azalış test edilecekse: Tek Yönlü Test

Alternatif hipotez tek yönde olur.  
Ex: “Boy ortalaması 172 cm’den büyüktür.”  
Ya da “Boy ortalaması 172 cm’den küçüktür.”  
Sadece bir yöne bakılır.

---

## Son Söz

Hipotez testi, sayıların gerçeği söylemesini sağlar.  
Veri biliminde, tıpta, sosyal bilimlerde, mühendislikte  
sayısız alanda kullanılır.

Bir iddia duyarsınız.  
Veriyi toplarsınız.  
Test yaparsınız.  
Ve karar verirsiniz.

Gerçek mi?  
Yoksa sadece şans mı?

Hipotez testi,  
bu sorulara yanıt bulmak içindir.

---



