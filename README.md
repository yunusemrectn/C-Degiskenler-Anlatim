# C-Degiskenler-Anlatim
using System;

namespace degisken
{
    class Program
    {
        static void Main(String[] args)
        {
            /*
            C# Değişkenler
            Değişken nasıl tanımlanır?
            Değişken Türü belirtilir ve boşluk bırakılıp değişkenin ismi yazıldıktan sonra '=' konularak karşısına bir değer yazılır ve ';' konulur.
            Örneğin 
            string isim = "Yunus Emre ÇETİN";
            int sayi = 7;

            Değişken ismi nasıl olmalı:
            -Değişken isimleri büyük küçük harfe duyarlıdır. Örneğin sayi ve Sayi farklı bir değişkendir. Ama genelde değişkenler küçük harfle başlar. Sınıflar büyük harfle yazılır.
            -Değişken ismi yazılırken harf ile başlamalısınız. İkinci bir kelime yazacaksanız araya '_' koyabilirsiniz veya ikinci kelimeyi büyük harfle başlatabilirsiniz. Not: İkinci harfi büyük başlatmak bir zorunluluk değildir. isterseniz 'musterininadresbilgileri' şeklinde de bir değişken ismi yazılabilir ama bu şekilde yazmak hem gönünüş hem de okunuş açısından zor olur. musterininAdresBilgileri şeklinde yazmanızı öneririm.
            Örneğin : 
            string musteriAdi = "Ahmet Bir";
            string musteri_Adi = "Ahmet Bir";

            -Değişken isimlerinin ilk harfinden sonra sayı kullanabilirsiniz. 
            Örneğin :
            int sayi1 = 5;
            int s1 = 2; 
            
            -Aynı tipteki değişkenler aralarına ',' konularak birlikte yazılabilir.
            Örneğin :
            int sayi1, sayi2, sayi3;
            Bunları birlikte tanımlarken aynı zamanda değer ataması da yapabiliriz.
            int sayi1=7, sayi2=1, sayi3=4;

            Not: Bir değişken ismi yazarken açıklayıcı olmalısınız. İleride bir program geliştirdiğiniz zaman çok fazla kod satırınız olacak. Bu yüzden hangi değişkeni nerede ne için yazdığınızı sizin ve sizden sonra o programı geliştirecek olan yazılımcıların anlaması için değişkenlerin isimlerini açıklayıcı şekilde yazmalısınız.
             
            Değişken ismi koyarken dikkat etmemiz gerekenler:
            -Değişken isimleri özeldir. Yani bir değişken ismini farklı bir değişkende kullanamazsınız.
            -Değişken ismi sayı ile başlayamaz.
            -Değişken ismi yazarken kelimeler arasına boşluk ve simge koyamayız. Ayrınca değişkem ismini yazarken : string isim+soyisim = "Yunus Emre ÇETİN" olarakta yazamayız.

            */
            
            byte b = 224;// doğal sayı tutar. 1 bayt (0-255)
            sbyte sb = -18; // tam sayı tutar. 1 bayt (-128-127)

            short s = 28;// tam sayı değer tutar. 2 bayt 
            int i = 34;// 4 bayt
            long l = 25;// 8 bayt

            float f = 5.67F; // Ondalıklı sayı tutar.
            double db = 5D; //
            decimal dc = 4546; 

            char c = 'N'; // Tek bir karakter tutar.
            string s1 = "Bugün hava çok soğuk." ; //Sınırsız metin tutar
            string yazi = string.Empty; //Boş string tutar

            //Bool doğru ya da yanlış şeklinde 2 değer alır. (True/False)
            bool b1 = 10>2; // Doğru olarak çıktı verir.
            bool b2 = 1<7; // Yanlış olarak çıktır verir.

            object kelime = "Güneş"; // Her türden veri alabilir. 
            object sayi = 7915;

            DateTime tarih = DateTime.Now; // Programı çalıştığınız tarih ve saati gösterir.
            System.Console.WriteLine(tarih);

            string tarih2 = DateTime.Now.ToString("dd.MM.yyyy"); // Programı çalıştığınız tarihi aralarında . olacak şekilde gösterir. dd/MM/yyyy yaparsanız da 01/01/2022 şeklinde gösterir.
            System.Console.WriteLine(tarih2);

            string saat = DateTime.Now.ToString("HH:mm"); // Programı çalıştığınız saati gösterir.
            System.Console.WriteLine(saat);

            const  float pi = 3.14F; // const anahtar kelimesini sabit bir değişken oluşturulmak istendiğinde kullanılır.
            
            Console.ReadKey();// Bunu yazmamın sebebi :  "console": "externalTerminal" şeklinde kullandığım için eğer bunu yazmazsam ekran direkt kapanıyor. Bu kod satırı ben herhangi bir şeye basmadığım sürece açılan console ekranının kapanmamasını sağlıyor.
        }
    }
}
