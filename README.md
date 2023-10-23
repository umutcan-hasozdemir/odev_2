using System;

int boy;
string cinsiyet;
double inç = 2.54;

Console.WriteLine("kilonuzu giriniz!");
double kilo = Convert.ToInt16(Console.ReadLine());

double işlem;
Console.WriteLine("boyunuzu girin!");
boy = Convert.ToInt16(Console.ReadLine());

Console.WriteLine("cinsiyetinizi giriniz!");
cinsiyet = Console.ReadLine();


if (cinsiyet == "kadın")
{

    işlem = 45.5 + 2.3 * (boy / inç - 60);
    if (kilo >= işlem)
    {
        Console.WriteLine("fazla kilolusunuz!!");
    }

    else
    {
        Console.WriteLine("ideal kilodasınız");
    }
}
if (cinsiyet == "erkek")
{
    işlem = 50 + 2.3 * (boy / inç - 60);
    if (kilo <= işlem)
    {
        Console.WriteLine("ideal kilodasınız");
    }
    else
    {
        Console.WriteLine("fazla kilolusunuz");
    }
}
