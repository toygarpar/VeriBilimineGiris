# Veri Çeşitleri ve Veri Yönetimi

Veri her zaman aynı biçimde gelmez. Bazısı düzenlidir, bazısı karmaşık, bazısı başıboş.
Genel olarak üçe ayrılır:

## Üç Ana Veri Türü

Veriler üç ana gruba ayrılır:  
**Yapılandırılmış (Structured)**  
**Yarı Yapılandırılmış (Semi-Structured)**  
**Yapılandırılmamış (Unstructured)**

Her biri farklıdır.  
Farklı şekillerde saklanır.  
Farklı yöntemlerle işlenir.

### 1. Yapılandırılmış Veri (Structured Data)

Düzenlidir. Satır satır, sütun sütun ilerler.
Veritabanlarında, Excel dosyalarında görürüz.
İsim, soyisim, adres, sipariş bilgisi…
Ne olduğu bellidir, yerli yerindedir.

Bu veriler belirli bir formata sahiptir.  
Genellikle tablolarda saklanır.  
Satır ve sütunlar halinde organize edilmiştir.  

Bir müşteri veri tabanı düşünelim:  
İsim, soyisim, adres, telefon numarası gibi alanlar vardır.  
Her bilgi için ayrı bir yer vardır.  
Her satır bir müşteriyi temsil eder.

Excel dosyaları ya da veritabanları bu tür veriler için kullanılır.  
Çünkü yapıları belli olduğu için kolayca analiz edilebilirler.

### 2. Yarı Yapılandırılmış Veri (Semi-Structured Data)

Ne tam düzenli, ne tamamen dağınık.
Etiketlenmiş, hiyerarşi içerir.

Bu veriler tamamen serbest değildir.  
Ancak tam anlamıyla tablo şeklinde de değildir.  

XML veya JSON dosyalarını örnek verebiliriz.  
Veriler etiketlenmiş durumdadır.  
Hiyerarşik bir yapıya sahiptir.  

Örneğin bir ürün katalogu olabilir.  
Her ürünün özellikleri var.  
Ancak her ürünün farklı sayıda özelliği olabilir.  
Bu yüzden tam bir tabloya sığmaz.

Bu veriler esnek yapılıdır.  
Analiz edilebilir ama özel araçlar gerekir.

Bazı şeyler belli, ama yine de işlemeye ihtiyaç duyar.

### 3. Yapılandırılmamış Veri (Unstructured Data)

Kuralsız, dağınık, başıboş…
Bu veriler belirli bir biçimde değildir. 
Ne anlatmak istediğini anlamak için önce işlememiz gerekir. 
Dokümanlar, e-postalar, ses kayıtları, resimler, videolar bu sınıfa girer.

Yapısı yoktur.  
Tabloya oturtulması zordur.  
Anlam çıkarmak daha karmaşıktır.  

Ancak günümüz teknolojisiyle bu veriler de işlenebiliyor.  
Doğal dil işleme, görüntü tanıma, ses analizi gibi yöntemlerle anlamlı hale getiriliyorlar.

---

## Veri Yönetimi Nedir?

Veriyi sadece toplamak yetmez.
Onu düzenlemek, korumak, işe yarar hale getirmek gerekir.
İşte bu sürecin adı: Veri Yönetimi.

Veri Yönetimi;  
verilerin toplanması,  
düzenlenmesi,  
saklanması,  
güvenliğinin sağlanması,  
kalitesinin kontrol edilmesi  
ve doğru kişilerle paylaşılmasının planlandığı süreçtir.

Veri yönetimi olmadan veri anlamsız kalır.  
Şirketler kararlarını veriye dayandıramaz.  
Kampanyalar rastgele olur.  
Raporlar eksik kalır.

Veri Yönetimi, veri biliminin temelidir.  
Ham veriden başlayıp,  
bilgiye ulaşmak için gereklidir.

---

## Veri Yönetiminde Aşamalar

Veri yönetimi, yalnızca bir iş değil, bir sistemdir.

Veri Yönetimi on bir ana alan içerir.  
Her bir alanın uzmanlığı, sorumluluğu ve yöntemi vardır.
Bu alanların ortasında ise **Data Governance (Veri Yönetişimi)** vardır.  
Diğer alanları birbirine bağlayan odaktır.

### 1. **Data Governance (Veri Yönetişimi)**

Her şeyin kurallarını koyan merkez. Kim neye erişir, ne zaman, nasıl?

Veri ile ilgili kuralları ve standartları belirleyen aşamadır.  
Kim hangi veriye erişebilir?  
Ne zaman erişebilir?  
Veri nasıl korunmalı?  
Bu soruların cevapları burada verilir.

Data Governance, diğer tüm alanları yönetir.  
Onlar arasında bağlantı kurar.  
Veri yönetimi sürecini düzenler.

### 2. **Data Modeling and Design (Veri Modelleme ve Tasarım)**

Veriye nasıl bakacağız? Ne soracağız? Cevabı hangi modelle arayacağız?

Verilerin nasıl yapılandırılacağını belirlediğimiz aşamadır.  
Hangi tablolar olacak?  
Alanlar ne olacak?  
Veriler nasıl ilişkilendirilecek?

Bu aşama, veri amacına uygun şekilde şekillenmesini sağlar.

### 3. **Data Storage and Operations (Veri Saklama ve İşlemleri)**

Veri nerede duracak? Ne kadar süreyle? Nasıl yedeklenecek?

Veriler nerede saklanacak?  
Nasıl depolanacak?  
Kaç yıl tutulacak?

Bu aşamada veri yaşam döngüsü planlanır.  
Verilerin güvenli bir şekilde saklanması sağlanır.

### 4. **Data Security (Veri Güvenliği)**

Verilerin yalnızca yetkili kişiler tarafından erişilebilir olması için kurallar koyar.  
Şifreleme, erişim kontrolleri, izleme sistemleri burada kullanılır.

Veri güvenliği, şirketler için hayati öneme sahiptir.  
Kaybedilen veri, maddi ve itibar kaybına yol açabilir.

Veriye herkes erişemez. Güvenlik şart. Sadece doğru kişi, doğru zamanda, doğru şekilde.

### 5. **Data Integration and Interoperability (Veri Bütünleştirme ve Uyum)**

Farklı kaynaklardan gelen verileri tek bir yerde toplamak için kullanılır.  
Veri bütünlüğü sağlanır.  
Tüm sistemler aynı dili konuşur hale gelir.

### 6. **Documents and Content (Belge ve İçerik Yönetimi)**

Yapılandırılmış verileri sakladığımız alan. 
Yapılandırılmış dokümanlar ve içerikler burada yönetilir.  
PDF’ler, Word dosyaları, raporlar gibi içerikler saklanır, arşivlenir, erişilebilir hale getirilir.

### 7. **Reference and Master Data (Referans ve Ana Veri Yönetimi)**

Şirketin temel verileri. Herkesin güvendiği, değişmeyen bilgiler.
Şirket içinde sürekli kullanılan temel veriler burada saklanır.  
Örneğin ülke listesi, para birimi, departman adları gibi.

Bu veriler her sistemde aynı şekilde kullanılır.  
Tutarlılığı sağlar.

### 8. **Data Warehousing and Business Intelligence (Veri Ambarı ve İş Zekası)**

Farklı kaynaklardan gelen veriler burada toplanır.  
Veriler birikir, rapor olur. İş zekâsı araçları burada devreye girer.
Raporlar hazırlanır.  
Dashboard’lar oluşturulur.

Bu katmanda iş zekası araçları kullanılır.  
Veriler karar almaya yardımcı olacak şekilde sunulur.

### 9. **Meta Data (Üst Veri)**

Verinin verisi. Hangi veri nerede, kimin elinde, ne işe yarar? Hepsi burada tutulur.

“Veri hakkında veri”dir.  
Hangi veri nerede?  
Hangi formatla saklandı?  
Kim üretmiş?  
Ne zaman değiştirildi?

Meta veri, veri bulmayı ve anlamayı kolaylaştırır.

### 10. **Data Quality (Veri Kalitesi)**

Toplanan verilerin doğru, eksiksiz ve güncel olduğundan emin olunur.  
Toplanan veri işe yarıyor mu? Hatalı mı, eksik mi? Kontrol ederiz.
Hatalı veriler düzeltilir.  
Eksik değerler tamamlanır.

Kaliteli veri, doğru kararlar demektir.

### 11. **Data Architecture (Veri Mimarisi)**

Verilerin genel yapısını ve akışını tanımlayan aşamadır.  
Veri nasıl aktarılacak?  
Hangi sistemler birbiriyle konuşacak?  
Veri nerede nasıl saklanacak?

Tablolar nasıl ilişkilendirilmiş? Veriler nasıl akıyor? Mimari burada kurulur.
Veri mimarisi, sistemin uzun vadeli çalışmasını sağlar.

---

## DMBOK Piramidi

DMBOK: Data Management Body of Knowledge  
Türkçesiyle: Veri Yönetimi Bilgi Birikimi

Bu piramit, veri yönetimindeki tüm alanları görsel olarak gösterir.  
Her katmanda farklı bir sorumluluk vardır.  
Piramidin ortasında Data Governance bulunur.  
Diğer tüm alanları birbirine bağlayan merkezdir.

> **Turuncu Katman:** Genel veri mimarisi, veri kalitesi, meta veri süreçleri burada tanımlanır.  
> **Yeşil Katman:** Veri modelleme, veri saklama, güvenliği gibi uygulama katmanları burada yer alır.  
> **Mavi Katman:** Kurallar ve çizimler sayesinde raporların oluşturulduğu katmandır.  
> **En Üst Katman:** Veri bilimi, yapay zeka, büyük veri analizleri burada yapılır.

---

## Son Söz

Veri çeşitleri farklıdır.  
Yapıları farklıdır.  
İşlenmeleri farklıdır.  
Ama hepsi bir şey ortaya çıkarır:  
**Bilgi**

Veri Yönetimi ise bu bilgiyi elde etmenin yollarını çizer.  
On bir alanı vardır.  
Her biri önemli.  
Her biri birbirine bağlı.

Veri bilimi, yapay zeka, büyük veri analizleri  
bu temelin üzerinde inşa edilir.  
Veri Yönetimi olmadan hiçbir proje sürdürülemez.

Veriyle çalışmak, sadece rakamlarla değil, sistemle çalışmaktır.
Veri yönetimi olmazsa, veri kaosa dönüşür.
Ama doğru yönetilirse, yalnızca bilgiye değil, akıllı kararlara ulaşırız.

---

