# En Temel C# Rehberi

Bu rehber, C# programlamanın en temel mantığını anlamak için hazırlanmıştır. 

## 1. Klavyeden Veri Girip İşlem Yapan Program Örneği

C# ile kullanıcıdan veri almak için `Console.ReadLine()` komutunu kullanırız. Klavyeden girilen her şey "metin" olarak algılanır. Sayısal bir işlem yapacaksak, bunu sayılara  çevirmemiz gerekir.

```csharp
// Kullanıcıdan 1. sayıyı isteyip tam sayıya çeviriyoruz
Console.Write("1. sayıyı girin: ");
int sayi1 = Convert.ToInt32(Console.ReadLine()); 

// Kullanıcıdan 2. sayıyı isteyip tam sayıya çeviriyoruz
Console.Write("2. sayıyı girin: ");
int sayi2 = Convert.ToInt32(Console.ReadLine()); 

// Sayıları topluyoruz
int toplam = sayi1 + sayi2;

// Sonucu ekrana yazdırıyoruz
Console.WriteLine("Sayıların toplamı: " + toplam);
```

## 2. Değişken Tipleri ve Anlamları

Verileri bilgisayarın hafızasında tutmak için "değişkenleri" kullanırız. İçine koyacağımız veriye göre değişkenin tipi değişir:

| Veri Tipi | Ne İşe Yarar? | Örnek Kullanım | 
| ----- | ----- | ----- | 
| **int** | Tam sayıları tutar. | `int yas = 20;` | 
| **double** | Ondalıklı sayıları tutar. | `double kilo = 75.5;` | 
| **string** | Metin ve yazıları tutar. Çift tırnak ile yazılır. | `string isim = "Ali";` | 
| **char** | Tek bir harf/karakter tutar. Tek tırnak ile yazılır. | `char harf = 'A';` | 
| **bool** | Sadece Doğru (`true`) veya Yanlış (`false`) değerini tutar. | `bool ogrenciMi = true;` | 

## 3. If-Else Kullanımı ve Anlamı

`if` ve `else` komutları, programın **karar vermesini** sağlar. 
* **`if` (Eğer):** Koşul doğruysa burası çalışır.
* **`else` (Değilse):** Koşul yanlışsa burası çalışır.

### Örnek: Ehliyet Yaşı Kontrolü

```csharp
Console.Write("Yaşınızı girin: ");
int yas = Convert.ToInt32(Console.ReadLine());

// Eğer yaş 18'e eşit veya büyükse:
if (yas >= 18)
{
    Console.WriteLine("Ehliyet alabilirsiniz!");
}
// Değilse (Yani yaş 18'den küçükse):
else
{
    Console.WriteLine("Ehliyet almak için yaşınız yetmiyor.");
}
```
