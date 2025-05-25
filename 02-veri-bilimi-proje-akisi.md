# Veri Bilimi Proje Akışı

**Problem Tanımlama** - bir problemi veya bir hedefi sürecin en başında tanımlamamız gerekiyor

Projeye başlamadan önce hangi sorunun çözülmesi gerektiği net bir şekilde tanımlanmalıdır.

İş hedefleriyle uyumlu ve çözülmesi gereken spesifik bir problemi anlamayı içerir.

## Problemi Anlamak
Her şey bir soruyla başlar. Ne çözmek istiyoruz? Neyi daha iyi hale getirmek istiyoruz?
Bu soruya net cevap veremiyorsak, yola çıkmamalıyız.

Amacınız müşteri memnuniyetini artırmak olabilir. Belki de satışları tahmin eden bir sistem kurmak istiyorsunuz.
Hedef net olmalı. Çünkü yanlış soruya doğru cevap yoktur.


## 1. Problem Tanımlama

Her projede ilk adım budur: neyi çözmek istediğimizi net bilmek.  
Problem açık değilse, çözüm de olmaz.  

Örneğin:  
Müşteri memnuniyetini artırmak mı istiyoruz?  
Yoksa bir satış tahmin modeli mi kurmak istiyoruz?  

İş hedefleriyle uyumlu olmalı.  
Çözülmesi gereken sorun tek bir cümleyle anlatılabilir olmalı.  

Başarılı bir proje, doğru tanımlanan bir problemle başlar.



---
## Veri Nerede?
Doğru veriye ulaşmadan, doğru sonuç beklemek boşunadır.
İhtiyacımız olan verileri belirlemekle başlarız. Sonra da bu veriler nerede saklı, nasıl erişilir, onu araştırırız.

Bu veriler dosyalarda, veri tabanlarında, API’lerde, şirketin kendi sistemlerinde veya başka yerlerde olabilir.
Toplanması sabır ve dikkat ister.


## 2. Veri Toplama

Hangi verilere ihtiyacımız var?  
Bu veriler nerede saklı?  
Nasıl toplayacağız?

Veri kaynakları farklı olabilir: dosyalar, veritabanları, API’ler, dış sağlayıcılar veya şirket içi sistemler.  

Bazı veriler hazır bulunur.  
Bazıları özel yazılımlarla çekilir.  
Bazıları için izin alınır.  

Veri toplamak, bilgi toplamaktır.  
Ve bu bilgi olmadan hiçbir model çalışmaz.

---

## 3. Veri Hazırlama

Elimize ulaşan ham veri genelde dağınıktır. Eksik bilgiler, hatalı girişler, uyumsuz formatlar...
Temizlenmeden işe yaramaz.

Önce düzenlenir. Eksikler tamamlanır. Hatalar düzeltilir.
Veri anlaşılır ve kullanılabilir hale getirilir.
Gerekirse bazı yeni bilgiler de mevcut verilerden türetilir. Bu işin adı "özellik mühendisliği'dir/feature engineering".

Toplanan veri her zaman düzgün değildir.  
Eksik satırlar olabilir.  
Yanlış değerler olabilir.  
Farklı biçimlerde saklanmış veriler olabilir.  

Bu yüzden veriyi temizlemek gerekir.  
Düzenlenir.  
Standart hale getirilir.  
Kayıp veriler tamamlanır.  

Bu adımda yapılan işlemler şunlardır:  
- Normalizasyon  
- Özellik mühendisliği (feature engineering)  
- Hatalı verilerin düzeltilmesi  

Hazırlanan veri, analiz edilebilir veridir.  
Hazırlık yapılmadan ileriye geçmek zordur.

---

## 4. Veri Analizi

Hangi problem için  hangi verileri kullanacağız, verilerle ilgili kullanım için bir senaryo var mı? 

Sonunda elimizde düzgün bir veri seti var. Ama bu verinin içinde ne var?
Şimdi sıra geldi veriyi anlamaya.  
Keşfe çıkarız. Rakamların ardında ne saklı, anlamaya çalışırız.
Dağılımlar, ortalamalar, uç değerler, ilişkiler...
Ne tür veriler var?  
Sayılar arasında bir ilişki var mı?  
Dağılımları nasıl?  

Bu aşamada keşifsel analiz yapılır.  
İstatistik kullanılır.  
Veri bilgisi ile problem bilgisi birleştirilir.  

Örneğin:  
Müşteri memnuniyetini artırmak istiyorsanız, anket sonuçları ve şikayet verileri incelenir.  
Buradan eğilimler çıkarılır.  

Analiz, verinin içinde saklı olan gerçekleri ortaya çıkarır.

Veriyle hikâyeyi kurmak bu aşamada başlar.

---

## 5. Veri Görselleştirme

Sayılar bazen kuru kalır.  
Görsellerle anlam kazanırlar.  

Bazen bir tablo, sayfalarca açıklamadan daha etkilidir.
Grafikler, diyagramlar, ısı haritaları… Rakamları gözle görünür hale getiririz.

Bu yüzden bulgular grafikler, tablolar, haritalar ile gösterilir.  
Amacı basittir: bilgiyi daha kolay anlaşılır hale getirmek.  

Bir tabloya bakıp anlamak zaman alabilir.  
Bir grafiğe bakıp fark etmek birkaç saniye sürer.  

Görselleştirme, hem analiz aşamasında hem de raporlamada kullanılır.  
Veri bilimcilerin en güçlü araçlarından biridir.

Böylece analiz sonuçları sadece anlaşılır değil, paylaşılır da olur.
Veri herkesin görebileceği bir dile çevrilir.

---

## 6. Model Oluşturma

Veri hazırlandı.  
Analiz edildi.  
Görselleştirildi.  

Artık geleceğe bakmak istiyoruz.
Elimizdeki verilerden öğrenen bir model kurarız.

Şimdi sıra geldi geleceği tahmin edecek modelleri oluşturmaya.  
Bu modeller makine öğrenmesi (ML), derin öğrenme (DL) gibi tekniklerle geliştirilir.  

Tahmin yapar, sınıflandırır.
Hangi müşteriler ayrılabilir, hangi ürün tutar, satışlar nasıl gider…
Makine öğrenmesi ve derin öğrenme bu işte bizim araçlarımızdır.

Sınıflandırma modelleri:  
Hangi müşteri sipariş verecek?  
Hangi e-posta spam?

Tahmin modelleri:  
Gelecek ay kaç ürün satılır?  
Bir hastalığın risk seviyesi nedir?

Model, verideki örüntüleri öğrendikten sonra yeni veriler üzerinde karar verir.  
Doğru model, doğru karar demektir.

---

## 7. İzleme ve Bakım

Hayat değişir. Veriler değişir. Sistemler değişir.

Proje bitmez model kurulunca.  
Zamanla veriler değişebilir.  
İş süreçleri değişebilir.  
Modelin performansı düşebilir.  

Bu yüzden modeller izlenmelidir. 
Kurulan modelin performansı düzenli olarak izlenir.
İşe yarıyor mu? Hâlâ doğru tahminler yapıyor mu? 
Hata oranları kontrol edilmelidir.  
Değişime göre yeniden eğitilmelidir.  

Bakım yapılmalıdır.  
Yeni verilere göre güncellenmelidir.  

İyi bir model, sadece iyi çalışmayla değil,  
sürekli bakım ve izlemeyle uzun süre işlevsel kalır.
Gerekirse yeniden eğitilir, güncellenir, iyileştirilir.

---

## Son Söz

Veri bilimi, sadece veriye bakmak değil; onunla düşünmek, anlamak, karar vermek demektir.
Her aşama, birbirine bağlı bir zincirdir.
Veri Bilimi, tek bir adımla değil,  
bir dizi adımla çalışan bir süreçtir.  

Her adım bir sonrakini besler.  
Hiçbiri atlanamaz.  
Hiçbiri önemsiz değildir.  

Problem tanımlanarak başlar.  
Verilerle desteklenir.  
Analiz edilir.  
Görselleştirilir.  
Modelleme ile geleceğe dair fikir verir.  
Sonunda sürekli izlenerek iyileştirilir.  

Bu akış, veri biliminin gücünü gösterir.  
Ve bu akış sayesinde, veri bilimi gerçek hayatta işe yarar.

---

