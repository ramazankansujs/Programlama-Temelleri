```csharp
Console.WriteLine("Bir sayı girin: ");


int sayi = Random.Shared.Next(0,10);
int sayi2 = Convert.ToInt32(Console.ReadLine());
int can = 5;



while (true)
{
    if (can != 0)
    {
        Console.WriteLine("Bir sayı girin: ");
        if (sayi2 == sayi)
        {
            Console.WriteLine("Bildiniz.");
            break;
        }
        else
        { 
            if(sayi2 < sayi)
            {
                Console.WriteLine("Daha büyük bir sayı giriniz.");
            }
            else
            {
                Console.WriteLine("Daha küçük bir sayı giriniz.");

            }

            int sayi3 = Convert.ToInt32(Console.ReadLine());
            sayi2 = sayi3;
            can--;
        }
    }
    else
    {
        Console.WriteLine("Tahmin hakkınız tükenmiştir.");
        break;
    }
}
```
