# Encryption

﻿using System;

public class Program
{
    public static void Main()
    {
        int p, s;
        char r, k = 'a';

        Console.WriteLine("Podaj przesunięcie");
        p = Convert.ToInt32(Console.ReadLine());
        Console.WriteLine("Wpisz szyfr. Naciśnij 'q' aby zakończyć");
        while (k != 'q')
        {
            k = Console.ReadKey(true).KeyChar;
            s = Convert.ToInt32(k);
            if (k != 'q')
            {
                s = p + s;
                r = Convert.ToChar(s);
                Console.Write(r);
            }
        }
    }
}
