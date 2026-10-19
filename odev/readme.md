Kullanıcının girdiği sayıyı daha önceden sistemin oluşturduğu bi sayı ile karşılaştırıp kullanıcıya bildiren program.


```csharp
Console.WriteLine("--- Sayı Tahmin Oyununa Hoş Geldiniz! ---");

int tutulanSayi = Random.Shared.Next(0, 10);
int can = 5;
//Ramazan Kansu
while (can > 0)
{
    Console.Write($"--------------------------------------\nKalan can sayısı {can}: Bir sayı girin: ");

    int tahmin = Convert.ToInt32(Console.ReadLine());

        if (tahmin == tutulanSayi){
        Console.WriteLine("Tebrikler, bildiniz!");
        break;
        }

            else if (tahmin < tutulanSayi){
            Console.WriteLine("Daha büyük bir sayı giriniz.");
            }
                else{
                Console.WriteLine("Daha küçük bir sayı giriniz.");
                }

    can--; 

    if (can == 0)
    {
        Console.WriteLine($"\nTahmin hakkınız tükenmiştir. Tutulan sayı: {tutulanSayi}");
    }
}

/*Klavyeden girilen bir sayıyı sistemde daha önceden rastgele oluşturulmuş bir sayı ile karşılaştıran bir oyun.*/
```
