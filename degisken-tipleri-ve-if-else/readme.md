
## 1. Klavyeden Veri Girip İşlem Yapan Program Örneği

C# ile kullanıcıdan veri almak için `Console.ReadLine()` komutunu kullanırız. Klavyeden girilen her şey "metin" olarak algılanır. Sayısal bir işlem yapacaksak, bunu sayılara çevirmemiz gerekir.a

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

### Örnek: Farklı Değişken Tiplerinin Birlikte Kullanımı

```csharp
string urunAdi = "Laptop";
int stokAdedi = 15;
double fiyat = 25999.99;
bool satistaMi = true;

// Farklı tipleri birleştirip ekrana yazdırma
Console.WriteLine("Ürün: " + urunAdi);
Console.WriteLine("Stok: " + stokAdedi);
Console.WriteLine("Fiyat: " + fiyat + " TL");
Console.WriteLine("Satışta mı?: " + satistaMi);
```

## 3. If-Else Kullanımı ve Anlamı

`if` ve `else` komutları, programın **karar vermesini** sağlar. 
- **`if` (Eğer):** Koşul doğruysa burası çalışır.
- **`else` (Değilse):** Koşul yanlışsa burası çalışır.

### Örnek 1: Temel If-Else (Ehliyet Yaşı Kontrolü)

```csharp
Console.Write("Yaşınızı girin: ");
int yas = Convert.ToInt32(Console.ReadLine());

if (yas >= 18)
{
    Console.WriteLine("Ehliyet alabilirsiniz!");
}
else
{
    Console.WriteLine("Ehliyet almak için yaşınız yetmiyor.");
}
```

### Örnek 2: Else If (Birden Fazla Koşul Kontrolü)

İkiden fazla durum varsa `else if` kullanılır. Şartlar yukarıdan aşağıya doğru kontrol edilir.

```csharp
Console.Write("Sınav notunuzu girin: ");
int not = Convert.ToInt32(Console.ReadLine());

if (not >= 85)
{
    Console.WriteLine("Sonuç: Çok İyi (A)");
}
else if (not >= 70)
{
    Console.WriteLine("Sonuç: İyi (B)");
}
else if (not >= 50)
{
    Console.WriteLine("Sonuç: Geçer (C)");
}
else
{
    Console.WriteLine("Sonuç: Kaldınız (F)");
}
```

### Örnek 3: && (VE) / || (VEYA) ile Çoklu Şartlar

- **`&&` (VE):** İki şartın da aynı anda doğru olması gerekir.
- **`||` (VEYA):** Şartlardan sadece birinin doğru olması yeterlidir.

```csharp
Console.Write("Kullanıcı adı: ");
string kullanici = Console.ReadLine();

Console.Write("Şifre: ");
string sifre = Console.ReadLine();

// && kullanımı: Hem kullanıcı adı hem şifre doğru olmak zorunda
if (kullanici == "admin" && sifre == "1234")
{
    Console.WriteLine("Sisteme başarıyla giriş yaptınız.");
}
else
{
    Console.WriteLine("Kullanıcı adı veya şifre hatalı!");
}
```
