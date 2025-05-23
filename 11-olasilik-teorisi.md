# Çıkarımcı İstatistik: Olasılık Teorisi ve Dağılımlar

Çıkarımcı istatistik, küçük bir örnek grubundan yola çıkarak, büyük topluluklar hakkında tahminde bulunma işidir. Elimizdeki birkaç veriye bakar, tüm resim hakkında bir fikir yürütürüz.

## Sayılardan Tahmine Yolculuk

Veri bilimi tahmin etmektir.  
Geleceği, bilinmeyeni, olası olanı tahmin etmek.  

Ve bu tahminlerin temelinde **olasılık teorisi** vardır.

Çıkarımcı istatistik, bir örneklem üzerinden popülasyon hakkında yorum yapmamızı sağlar.  
Yani az veriyle çok şey anlayabilmemizi sağlar.

Olasılık ise bize o anın belirsizliğini ölçer.  
Bir şeyin ne kadar mümkün olduğunu gösterir.

## OLASILIK TEORİSİ
Bir olayın olup olmayacağını önceden bilemeyiz. Ama ne kadar olası olduğunu hesaplayabiliriz. Olasılık teorisi, işte bu belirsizliği anlamamıza yardım eder.
Bir olayın olasılığı 0 ile 1 arasındadır.

0: Olmaz.

1: Kesin olur.

Gündelik hayatın diliyle: "Belki", "ihtimal", "şansı var" dediğimiz şeylerin matematiksel karşılığıdır.

---

## Olasılık Nedir?

Olasılık, bir olayın ne kadar muhtemel olduğunu gösteren sayıdır.  
0 ile 1 arasında değişir.  
0 = imkansız.  
1 = kesin.  
0.5 = iki eşit şans.

### Temel Kavramlar

### Rastgele Olay (Deney)  
Sonucu önceden bilinemeyen olaylardır.  
Zar atmak, para fırlatmak, hava durumu tahmini gibi.

### Örneklem Uzayı (Ω)  
Tüm olası sonuçların bulunduğu kümedir.  
Örneğin bir zar atışı için Ω = {1, 2, 3, 4, 5, 6}

### Olay (A)  
Örneklem uzayının bir alt kümesidir.  
Zar atışında "çift gelme" A = {2, 4, 6} olur.

### Olasılık (P(A))  
Bir olayın gerçekleşme ihtimalidir.  
Sayısal olarak ifade edilir.  
Formülü:  
```
P(A) = Başarı sayısı / Toplam deney sayısı
```

---

## Olasılık Teorisinin Kuralları

### 1. Olasılık Aralığı  
Herhangi bir A olayı için:  
**0 ≤ P(A) ≤ 1**

### 2. Kesin Olay  
Tüm örneklem uzayının olasılığı her zaman 1'dir.  
**P(Ω) = 1**

### 3. Karşılıklı Dışlayan Olaylar  
İki olay aynı anda gerçekleşemiyorsa, birleşimleri toplamlarına eşittir.  
**P(A ∪ B) = P(A) + P(B)**

### 4. Koşullu Olasılık  
Bir olayın başka bir olayın gerçekleştiği bilindiğinde ne kadar muhtemel olduğunu gösterir.  
**P(A|B) = P(A ∩ B) / P(B)**

### 5. Bağımsız Olaylar  
Bir olayın sonucu diğerini etkilemiyorsa, bu olaylar bağımsızdır.  
**P(A ∩ B) = P(A) × P(B)**

---

## Veri Bilimi ve Olasılık

Veri Bilimi tahmin üzerine kuruludur.  
Ve tahminin kalbi olasılıktır.

Makine öğrenmesi algoritmaları,  
NLP modelleri,  
veri madenciliği yöntemleri  
hepsi olasılık teorisine dayanır.

Örneğin:  
- Bir spam filtrenin nasıl çalıştığını bilir misin?  
Spam kelime olasılıklarını hesaplar.  
- Ya bir öneri sistemi?  
Kullanıcının hangi ürünleri beğeneceğini olasılıkla tahmin eder.

Olasılık olmadan veri bilimi sessiz kalır.  
Olasılık onun dilidir.

---

## Olasılık Dağılımları

Sayılar bir desen izler.  
Bu desenleri dağılımlarla anlarız.  
Dağılım, bir rastgele değişkenin değerlerinin nasıl yayıldığını gösterir.

### Rastgele Değişken Nedir?

Rastgele bir deneyin sonucunu sayıya dönüştüren fonksiyondur.  
Zar atma → sayısal değer  
Para fırlatma → yazı mı tura mı  
Kişinin boyu → gerçek sayı

İki türevi vardır:  
**Kesikli** ve **Sürekli**

---

## 1. Kesikli Rastgele Değişkenler

Başarı – başarısızlık gibi ikili sonuçları sayar.
Belirli ve ayrık değerler alır.  
Zar atışı gibi.  
Ya 1, ya 2, ya 3… ama 2.5 yoktur.

### Binom Dağılımı  
Bağımsız deneylerde başarı sayısını modellemek için kullanılır.  
Ex: 10 kez zar atıldığında kaç defa 6 geldi?

### Poisson Dağılımı  
Belirli bir sürede veya alanda olay sayısını modellemek için kullanılır.  
Ex: Bir hastaneye gelen hasta sayısı

---

## 2. Sürekli Rastgele Değişkenler

Bir aralıkta her değeri alabilir.  
Boyunuzun 170 cm mi 170.1 cm mi olduğunu bilebilirsiniz.

### Normal Dağılım  
Çoğu doğal fenomen bu dağılıma uyar.  
Sınav notları, gelir dağılımı, ağırlıklar genellikle normal dağılır.  
Grafiği çan eğrisi şeklindedir.

### Üstel Dağılım  
Olaylar arasındaki süreyi modellemek için kullanılır.  
Ex: Bir makinenin arızalanma süresi

---

## Dağılım Nedir?

Dağılım, bir veri kümesindeki değerlerin nasıl yayıldığını gösterir.  
Hangi değerler daha sık görülüyor?  
Ortalama etrafında nasıl dağılmışlar?  
Uç değerler var mı?

Dağılım, bir rassal değişkenin alabileceği tüm değerleri ve bu değerlerin olasılıklarını tanımlar.

Ex:  
Bir sınıftaki sınav notlarının dağılımı, öğrencilerin başarısı hakkında ipucu verir.  
Dağılım genişse, notlar çok değişken demektir.  
Dar bir dağılım homojenliği gösterir.

---

## Son Söz

Olasılık teorisi,  
verilerin içindeki belirsizliği ölçmenin yolu.  
Dağılımlar ise  
bu verilerin düzenini anlamamızı sağlar.

Çıkarımcı istatistikte küçük bir örneklemden başlayıp  
büyük bir popülasyon hakkında karar veriyoruz.  
Ve bu kararlar olasılık ve dağılımlarla destekleniyor.

Sayılar sadece sayı değildir.  
Onlar tahmindir.  
Onlar bilgiyi taşıyan seslerdir.

Ve biz,  
veri bilimciler olarak,  
bu sesleri duymaya çalışıyoruz.

---

