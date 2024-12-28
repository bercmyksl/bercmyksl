
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace çalışma
{
    internal class Program
    {
        public class cocuklar
        {
            public string Name { get; set; }
            public int Yas { get; set; }
            public int time { get; set; }





        }


        static void Main(string[] args)
        {
            List<object> fiyat = new List<object>();
            {
                fiyat.Add("0-30 dk arası :" + 100 + "Tl");
                fiyat.Add("0-60 dk arası :" + 200 + "Tl");
                fiyat.Add("60 dk ve üzeri her dakika için :" + 8 + "TL");
            }
            Console.WriteLine("eğlence parkına Hosşgeldiniz...");
            Console.WriteLine("fiyatlandırma listesi :");
            Console.WriteLine("yaş sınırı : 6");
            foreach (var a in fiyat)
            {
                Console.WriteLine(a);
            }

            int tutar;

            List<cocuklar> kayıt = new List<cocuklar>();
            Console.WriteLine("çocuğunuzun ismini giriniz.");
            string isim = Convert.ToString(Console.ReadLine());
            Console.WriteLine("yaşını giriniz.");
            int yas = Convert.ToInt32(Console.ReadLine());

            if (yas > 6)
            {
                Console.WriteLine("çocuğunuz 6 yaşından büyük olduğu için oyun parkına giremez.");
            }
            else
            {

                while (yas <= 6)
                {

                    Console.WriteLine("ne kadar süre eğlence parkında kalacak?(DK cinsinden.");
                    int zaman = Convert.ToInt32(Console.ReadLine());
                    kayıt.Add(new cocuklar { Name = isim, Yas = yas, time = zaman });

                    foreach (var cocuklar in kayıt)
                    {
                        Console.WriteLine($"İsim :{cocuklar.Name}-Yaş :{cocuklar.Yas}-Kalacağı zaman :{cocuklar.time}");
                    }
                    if (zaman <= 30)
                    {
                        tutar = 100;
                        Console.WriteLine("ödenecek tutar :" + tutar);
                    }
                    else if (zaman <= 60)
                    {
                        tutar = 200;
                        Console.WriteLine("ödenecek tutar :" + tutar);
                    }
                    else if (zaman > 60)
                    {
                        tutar = 200 + ((zaman - 60) * 8);
                        Console.WriteLine("ödenecek tutar :" + tutar);



                    }
                    break;
                }
                Console.WriteLine("iyi eğlenceler dileriz.");
            }














        }
    }
}