#  Programlama Temelleri: Ders İçeriği ve Yol Haritası

Bu rehber, Programlama Temelleri dersi boyunca adım adım öğreneceğimiz temel konuları ve C# dili ile yapacağımız pratikleri içermektedir.

---

## 1️⃣ Algoritma ve Programlama Mantığını Kavrama
Bilgisayara nasıl düşünmesi gerektiğini öğreteceğimiz temel mantık adımıdır. 
* **Algoritma nedir?** Günlük hayattaki problemleri mantıksal adımlarla çözme becerisi.
* **C# Karşılığı:** Bilgisayarın verileri nasıl işlediğini ve kod akışının sırasını anlamak.

---

## 2️⃣ Akış Şeması Oluşturma
Bir problemin çözüm adımlarını görselleştirerek mantıksal hataları önleme aşamasıdır.
* Standart semboller (Başlangıç/Bitiş, İşlem, Karar, Giriş/Çıkış).
* **Örnek Senaryo:** Kullanıcıdan sayı alıp tek mi çift mi olduğunu gösteren şemanın mantığı.

---

## 3️⃣ Gerçek Akış Diyagramı Oluşturulmuş Bir Problemi Programlama
Hazırlanan akış şemalarını C# dili ile koda dökme aşamasıdır.
* Diyagramdaki karar bloklarını koda uyarlama.

### C# Örnek (Tek/Çift Sayı Kontrolü):
```csharp
int sayi = 10;
if (sayi % 2 == 0) 
{
    Console.WriteLine("Sayı çifttir.");
} 
else 
{
    Console.WriteLine("Sayı tektir.");
}
```

---

## 4️⃣ C# Programlama Dili Arayüzünü Öğrenme
Visual Studio ortamını tanıma, yeni proje oluşturma ve konsol ekranını kullanma aşamasıdır.
* Temel arayüz bileşenleri, `Solution Explorer` ve hata ayıklama (debugging) araçları.

---

## 5️⃣ C# Programlama Diliyle Programlama Yapma
Değişkenler, veri tipleri ve temel kontrol yapıları ile basit konsol uygulamaları geliştirme aşamasıdır.

### C# Örnek (Değişkenler ve Temel Girdi/Çıktı):
```csharp
Console.Write("Adınızı giriniz: ");
string ad = Console.ReadLine();
Console.WriteLine("Hoş geldin, " + ad + "!");
```

---

## 6️⃣ C# Dilinde String (Metin) İşlemlerini Yapma
Metinsel veriler üzerinde arama, değiştirme, birleştirme ve biçimlendirme işlemleri yapma aşamasıdır.

### C# Örnek (String Metotları):
```csharp
string mesaj = "Programlama Temelleri";
Console.WriteLine(mesaj.ToUpper()); // PROGRAMLAMA TEMELLERI
Console.WriteLine(mesaj.Length);    // 21 karakter uzunluğu
```

---

## 7️⃣ C# Programlama Diliğinde Fonksiyonları Kullanma
Kod tekrarını önlemek ve projeyi modüler hale getirmek için metotları (fonksiyonları) kullanma aşamasıdır.

### C# Örnek (Fonksiyon Kullanımı):
```csharp
static int Topla(int sayi1, int sayi2) 
{
    return sayi1 + sayi2;
}

// Kullanımı:
// int sonuc = Topla(5, 10);
```

---

## 8️⃣ C# Programlama Dilinde Dosya ve Klasör İşlemlerini Yapma
Harici dosyalar oluşturma, dosyalara veri yazma ve mevcut dosyaları okuma aşamasıdır (`System.IO` kütüphanesi).

### C# Örnek (Dosyaya Yazma ve Okuma):

```csharp
// Dosya oluşturma ve yazma
File.WriteAllText("bilgi.txt", "Merhaba Programlama Dünyası!");

// Dosyadan okuma
string icerik = File.ReadAllText("bilgi.txt");
Console.WriteLine(icerik);
```

---
