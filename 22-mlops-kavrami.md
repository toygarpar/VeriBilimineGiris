# MLOps Kavramı  

## MLOps Nedir?

MLOps (Machine Learning Operations), makine öğrenmesi modellerinin geliştirilmesinden üretim ortamına dağıtımına ve yönetimine kadar olan tüm yaşam döngüsünü kapsayan bir disiplindir. DevOps prensiplerini makine öğrenmesi süreçlerine uyarlayarak:

- **Geliştirme süreçlerini hızlandırır**
- **Dağıtım risklerini azaltır**
- **Model performansını sürekli izler**
- **Yönetim maliyetlerini düşürür**

## MLOps'un Temel Bileşenleri

### 1. Veri Yönetimi
- **Veri Kalitesi**: Eksik veri, aykırı değer yönetimi
- **Veri Sürümleme**: DVC (Data Version Control) gibi araçlarla
- **Veri Pipeline'ları**: Otomatik veri akış sistemleri

### 2. Model Geliştirme
- **Deney Takibi**: MLflow, Weights & Biases
- **Hiperparametre Optimizasyonu**: Optuna, Ray Tune
- **Model Kayıt Defteri**: Model depolama ve sürümleme

### 3. Model Dağıtımı
- **CI/CD Pipeline'ları**: GitLab CI/CD, GitHub Actions
- **Konteynerleştirme**: Docker, Kubernetes
- **Canlıya Alma Stratejileri**: A/B testi, Canary dağıtım

### 4. Model İzleme
- **Performans Metrikleri**: Accuracy, Precision, Recall drift
- **Veri Drift**: Evrimleşen veri dağılımlarının tespiti
- **Altyapı İzleme**: CPU/GPU kullanımı, gecikme süreleri

## Makine Öğrenmesi Modelini Üretime Göndermek

Makine öğrenmesi modeli eğitmek kolaydır.  
AMA onu gerçek hayatta çalıştırmak zordur.  
İnsanlar etkileşim kurar.  
Veriler değişir.  
Model eskir.  
Yeni verilere göre yenilenmelidir.

Bunu yapmak için MLOps vardır.

**MLOps – Machine Learning Operations**,  
makine öğrenmesi modellerinin geliştirilmesi, dağıtılması  
ve üretim ortamında yönetilmesi sürecidir.

---

## Neden MLOps?

Bazı modeller laboratuvarda iyi çalışır.  
AMA üretimde başarısı düşebilir.  
Çünkü üretim ortamı dinamiktir.  
Veriler sürekli değişir.  
İş süreçleri farklıdır.

MLOps ile her şey daha düzenli olur.  
Modeller hızlıca güncellenir.  
Doğru çalışan model tekrar eder.  
Bozulan model fark edilir.  
Ve yenisiyle değiştirilir.

---

## MLOps Ne Amaçlı?

### 1. Geliştirme ve Dağıtımı Otomatikleştirmek  
Manuel süreçlerden kaçın.  
Modeller otomatik olarak hazırlanıp gönderilir.

### 2. Versiyon Kontrolü  
Hangi model hangi sürümde?  
Ne zaman güncellendi?  
Hangi veriyle eğitildi?  
Versiyon kontrolü sayesinde hepsi bilinir.

### 3. Model İzleme  
Model canlı ortamda çalışmaya başladı.  
Nasıl çalışıyor?  
Hata yapıyor mu?  
Performansı düşüyor mu?

Gözlemlediğinizde fark edersiniz.  
Düşüş varsa müdahale edebilirsiniz.

### 4. Güvenlik ve Uyumluluk  
Model kimin erişebileceğini bilir mi?  
Gizlilik politikalarına uyuyor mu?

MLOps ile tüm bu sorulara cevap verilir.


---

## MLOps Süreçleri

### 1. Veri Yönetimi  
Veri toplama, temizleme, dönüştürme ve sürüm kontrolü yapılır.  
Modelin kalitesi, veri kalitesine bağlıdır.  
Bu yüzden veri her zaman güncel ve tutarlı olmalıdır.

Ex:  
E-ticaret sitesi verisinde yeni bir ürün kategorisi çıktı.  
Bu değişiklik veri yönetim sisteminde yer almalı.  
Yoksa model eskiye dayalı tahmin yapar.

### 2. Model Geliştirme  
Model oluşturulur. Eğitilir. Test edilir.  
Doğrulama yapılır. Sonra dağıtım aşamasına geçilir.  
Bu süreçte hiperparametre optimizasyonu yapılır.  
En iyi performans için doğru seçim yapılır.

### 3. Model Dağıtımı  
Eğitim bitince sıra geldi modeli kullanmaya.  
Model canlıya alınır.  
API’ye bağlanır.  
Her müşteri isteğine yanıt verir.

Yeni bir model çıksa bile  
eski model hâlâ çalışırken  
geçiş düzgün yapılmalı.  
Bu iş MLOps’in görev alanıdır.

### 4. Model İzleme ve Yönetim  
Model çalışmaya başlayınca izlenmelidir.  
Zamanla veri değişir.  
Modelin performansı bozulabilir.  
Bu durum “model drift” olarak bilinir.  
Model yeniden eğitilmelidir.

MLOps, modeli takip eder.  
Uyarı verir.  
Otomatik eğitimi başlatır.  
Yeni modeli güvenli şekilde devreye alır.

---

## MLOps Seviyeleri

Bir şirketin MLOps olgunluğunu ölçmek için üç ana seviye tanımlanmıştır.  
Bu seviyeler, otomasyon düzeyini ve entegrasyonu gösterir.

## MLOps Olgunluk Seviyeleri

### Seviye 0: Manuel Süreçler
- **Özellikler**:
  - Tüm işlemler elle yapılır
  - Veri setleri statik ve güncellenmez
  - Model dağıtımı manuel
  - Performans izleme yok
- **Kullanım**: Küçük POC'ler ve başlangıç projeleri

### Seviye 1: ML Pipeline Otomasyonu
- **Gelişmeler**:
  - Veri ve model sürümleme
  - Otomatik eğitim pipeline'ları
  - Temel CI/CD entegrasyonu
  - Basit performans izleme
- **Faydalar**: Hata oranlarında %40-60 azalma

### Seviye 2: CI/CD Pipeline ile Sürekli Öğrenme
- **Gelişmiş Özellikler**:
  - Otomatik yeniden eğitim (retraining)
  - Çoklu model A/B testi
  - Gelişmiş drift tespiti
  - Self-healing sistemler
- **Örnekler**: Netflix öneri sistemi, Tesla otonom sürüş

---

### 🔹 MLOps Seviyesi 0 – Manuel Süreç

Her şey elle yapılır.  
Model elle eğitilir.  
Elle test edilir.  
Elle dağıtılır.

- CI/CD yoktur.  
- Otomasyon yoktur.  
- Yeni sürümler nadiren çıkar.  
- Performans takibi yapılmaz.

Bu seviye, sadece deneme projeleri içindir.  
Gerçek hayatta uygulanması risklidir.

> Grafik Açıklaması:  
Bir kişinin masa başında tek tek yaptığı işlemleri gösteren basit bir diyagram.

---

### 🔹 MLOps Seviyesi 1 – ML Pipeline

Modeller artık otomasyonla işler.  
Data pipeline ile veri akışı sağlanır.  
Model eğitimi yeniden üretilebilir olur.

#### Hangi Özellikler Var?
- Otomatik veri toplama  
- Model versiyonlaması  
- CI/CD kısmen uygulanmış  
- Model performansı izleniyor  
- Geribildirim mekanizması kurulmuş  

Modelin kötüleştiğini anladığınızda  
yeniden eğitebilirsiniz.  
Yeni sürümü üretime gönderebilirsiniz.

> Grafik Açıklaması:  
Veri girişinden model çıktısına kadar olan işlem hattını gösteren bir pipeline diyagramı.

---

### 🔹 MLOps Seviyesi 2 – Tam Otomasyon + Ölçeklenebilirlik

Burada her şey tamamen otomatik çalışır.  
Model yeniden eğitilir.  
Dağıtılır.  
Binlerce sunucuda çalıştırılır.  
Saatlik olarak güncellenir.

Bu seviye, büyük şirketler için gereklidir.  
Çünkü veri hızla değişir.  
Modelin güncel kalması şarttır.

#### Hangi Özellikler Var?
- Gerçek zamanlı veri beslemesi  
- Tam otomatik CI/CD  
- Dinamik model izleme  
- Otomatik yeniden eğitim (retraining)  
- Yüksek ölçeklenebilirlik  

Modelin performansı saatlik olarak kontrol edilir.  
Drift tespit edilirse,  
otomatik olarak yeni model eğitilir ve yayına alınır.

> Grafik Açıklaması:  
Birden fazla sunucu, veri akışı, model izleme sistemleriyle bağlantılı bir sistem diyagramı.

---

## Karşılaştırmalı Tablo: MLOps Seviyeleri

| Özellik | **Level 0 – Manuel** | **Level 1 – Pipeline** | **Level 2 – Otomatik / Ölçeklenebilir** |
|--------|-----------------------|-------------------------|------------------------------------------|
| **Veri Yönetimi** | Manuel | Kısmen otomatik | Tamamen otomatik |
| **Model Geliştirme** | Elle | Scriptlerle | Otomatik |
| **Model Dağıtımı** | El ile | Kısmi CD | Otomatik CI/CD |
| **Model İzleme** | Yok | Temel izleme | Gelişmiş izleme + uyarı |
| **Model Güncellemesi** | Nadiren | Planlı | Sürekli ve otomatik |

---

## MLOps Araç Ekosistemi

| Kategori | Popüler Araçlar |
|----------|-----------------|
| Veri Yönetimi | DVC, Pachyderm, Delta Lake |
| Deney Takibi | MLflow, Weights & Biases, Neptune |
| Model Dağıtım | Seldon, BentoML, TorchServe |
| İzleme | Evidently, WhyLabs, Prometheus |
| Orkestrasyon | Kubeflow, Metaflow, Airflow |

---

## MLOps Uygulama Örnekleri

1. **Finans Sektörü**: Kredi skorlama modellerinin günlük güncellenmesi
2. **E-ticaret**: Kişiselleştirilmiş önerilerin saatlik yeniden eğitimi
3. **Sağlık**: Tıbbi görüntü analiz modellerinin FDA uyumlu dağıtımı
4. **Üretim**: Ekipman arıza tahmin sistemlerinin edge cihazlara dağıtımı

MLOps, makine öğrenmesi modellerinin gerçek dünyada değer üretebilmesi için kritik bir disiplindir. Kuruluşların MLOps olgunluk seviyelerini artırması, AI yatırımlarından elde edilen getiriyi doğrudan etkilemektedir.

---

## Son Söz

MLOps;  
makine öğrenmesi modellerinin hayat bulduğu süreçtir.  
Eğitilen model, sadece bir dosya değildir.  
Onu bir ürün haline getiren süreç budur.

Modelin başarılı olması için  
doğru veri,  
doğru dağıtım,  
ve doğru izleme şarttır.

MLOps olmadan,  
modeller kapalı dünyada kalır.  
AMA MLOps ile  
modeller hayat bulur.  
Ürün olur.  
Gerçek hayatta iş yapar.

Veri seti sessizken,  
MLOps, onları konuşmaya öğretir.

---


