# ATMapp
ATM Application

//Kullanıcıya hangi işlemi gerçekleştirmek isediği sorulur.
// 1- Bakiye Sorgulama
// 2- Para Çekme
// 3- Para Yatırma
// e ile çıkış yapma

int bakiye = 5000;
Console.WriteLine("Merhaba Hoşgeldiniz");
Console.WriteLine("Hangi işlemi gerçekleştirmek istiyorsunuz? Lütfen seçim yapınız");

string secim = Console.ReadLine();

if (secim =="1")
{
    Console.WriteLine($"Bakiyeniz: {bakiye}");
}

else if (secim =="2")
{
    Console.WriteLine("Para çekme işlemi için tutar giriniz.");
    int cekilecekTutar = Convert.ToInt32(Console.ReadLine());

    Console.WriteLine("Para çekme işlemi gerçekleştiriliyor lütfen bekleyiniz.");
    Console.WriteLine($"Kalan tutar : {bakiye-cekilecekTutar}");
}
else if (secim =="3")
{
    Console.WriteLine("Yatırmak istediğiniz tutarı giriniz");
    int yatirilacakTutar = Convert.ToInt32(Console.ReadLine());

    Console.WriteLine("Para yatırma işlemi gerçekleştiriliyor lütfen bekleyiniz.");
    Console.WriteLine($"Yeni bakiye : {bakiye + yatirilacakTutar}");
}
else if (secim == "e")
{
    Console.WriteLine("Çıkış yapıldı.İyi günler dileriz.");
}
else
{
    Console.WriteLine("Lütfen geçerli bir seçim yapınız");
}
