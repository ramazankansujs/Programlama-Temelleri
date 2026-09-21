# Ders: Programlama Temelleri
## Konu: Algoritma ve Programlama Mantığını Kavrama

Bilgisayar bilimlerinin temeli, makinelerin donanımsal gücünden ziyade, o gücü yönlendiren **algoritmik düşünme** becerisine dayanır. Bilgisayarlar kendi başlarına düşünemezler; yalnızca kendilerine verilen komut dizilerini olağanüstü bir hızda işlerler. Bu nedenle programlama, bilgisayara "ne yapması gerektiğini" değil, "nasıl yapması gerektiğini" adım adım ve eksiksiz bir biçimde anlatma sanatıdır. 

Bu süreçte temel alınan iki ana kavram **algoritma** ve **programlama mantığıdır**.

---

### 1. Algoritma Nedir?

Algoritma, belirli bir problemi çözmek veya belirli bir amaca ulaşmak için tasarlanmış, başlangıcı ve sonu olan, sonlu sayıdaki adımlardan oluşan kesin kurallar dizisidir. Başarılı bir algoritmanın matematiksel ve mantıksal olarak taşıması gereken temel özellikler vardır:

*   **Girdi (Input):** Algoritma dışarıdan sıfır veya daha fazla değer alabilir. Başlangıç durumunu belirleyen verilerdir.
*   **Çıktı (Output):** Algoritma, en az bir sonuç (çıktı) üretmelidir. Girdilerin işlenmesiyle elde edilen çözüm değeridir.
*   **Kesinlik:** Algoritmadaki her adım açık, net ve yoruma kapalı olmalıdır. Bilgisayar belirsizlikleri çözemez.
*   **Sonluluk:** Algoritma her türlü olasılıkta sonlu sayıda adım işlem gördükten sonra mutlaka sonlanmalıdır. Sonsuz döngüye (infinite loop) giren bir yapı algoritma olarak kabul edilemez.

### 2. Algoritmanın İfade Ediliş Biçimleri

Geliştirilen mantığın bilgisayar koduna dökülmeden önce formüle edilmesi gerekir. Bu amaçla üç temel yöntem kullanılır:

#### A. Günlük Dille İfade
Problemin çözüm adımlarının doğal dille yazılmasıdır. Ancak doğal dildeki anlam karmaşaları (kesinlik ilkesine aykırılık) nedeniyle karmaşık problemlerde tercih edilmez.

#### B. Sözde Kod (Pseudocode)
Doğal dil ile programlama dilleri arasında bir geçiş formudur. Belirli bir programlama dilinin sözdizimine (syntax) bağlı kalmadan, ancak kodlamaya çok yakın bir mantıkla yazılır.

> **Örnek Sözde Kod (Girilen iki sayının ortalamasını alma):**
> 1. BAŞLA
> 2. SAYI_OKU X
> 3. SAYI_OKU Y
> 4. TOPLAM = X + Y
> 5. ORTALAMA = TOPLAM / 2
> 6. YAZDIR ORTALAMA
> 7. BİTİR

#### C. Akış Şemaları"
Algoritmanın adımlarının standart geometrik şekillerle görselleştirilmesidir. Büyük projelerde sistemin genel yapısını görmek için kullanılır.

| Geometrik Şekil | Anlamı ve İşlevi |
| :--- | :--- |
| **Elips / Oval** | Algoritmanın başlama ve bitiş noktalarını belirtir. |
| **Paralelkenar** | Dışarıdan veri girişini veya dışarıya veri çıkışını ifade eder. |
| **Dikdörtgen** | Matematiksel hesaplamaların ve atama işlemlerinin yapıldığı süreç bloğudur. |
| **Eşkenar Dörtgen** | Karar verme ve karşılaştırma (Şart/Eğer) durumlarını gösterir. |
| **Oklar** | İşlem akışının yönünü belirtir. |

---

### 3. Programlama Mantığı ve Temel Yapıtaşları

Bir algoritmayı tasarladıktan sonra, onu herhangi bir programlama dili (Python, C, Java vb.) ile bilgisayarın anlayacağı dile çevirmek gerekir. Hangi dili kullanırsanız kullanın, programlama mantığı **üç temel yapı taşı** üzerine inşa edilir:

**1. Ardışık Yapı:** 
Komutların yukarıdan aşağıya doğru, yazılış sırasına göre hiçbir atlama olmadan sırayla çalıştırılmasıdır. Çoğu basit algoritmanın belkemiğidir.

**2. Seçimli / Karar  Yapısı:** 
Programın çalışması esnasında bir koşulun sınanması ve duruma göre (Doğru veya Yanlış) farklı işlem bloklarına yönlenilmesidir. Programın "karar vermesini" sağlar. (Örn: `Eğer (If)` sıcaklık 100'den büyükse, suyu kaynıyor olarak işaretle, `Değilse (Else)` ısıtmaya devam et).

**3. Tekrarlı (Iteration/Loop) Yapı:** 
Bir işlemin veya işlem bloğunun belirli bir koşul sağlandığı sürece veya belirli bir sayıda tekrar tekrar çalıştırılmasıdır. Kod tekrarını önler ve performansı artırır. (Örn: `Döngü (While, For)` yapısı kullanılarak 1'den 1000'e kadar olan sayıların ekrana tek satır kodla yazdırılması).

### 4. Yazılım Geliştirme Süreci (Problem Çözme Mantığı)

Bir mühendis veya bilgisayar bilimcisi olarak problemi çözerken şu sırayı takip etmelisiniz:

1. **İhtiyaç Analizi:** Problem nedir? Girdiler ve istenen çıktılar nelerdir?
2. **Algoritma Tasarımı:** Çözüm yolu adım adım oluşturulur (Sözde kod veya akış şeması ile).
3. **Kodlama:** Tasarlanan algoritma seçilen programlama diliyle koda dönüştürülür.
4. **Test (Sınama):** Kod farklı girdilerle çalıştırılarak doğru sonuç üretip üretmediği, uç durumlarda çöküp çökmediği kontrol edilir.
5. **Bakım ve İyileştirme:** Gerekli optimizasyonlar yapılır ve kod güncellenir.
