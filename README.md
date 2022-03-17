using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace CalculatorConsoleApp
{
    class Program
    {
        static void Main(string[] args)
        {

            Console.Title = "Aplikasi Calculator";

            Console.WriteLine("======Aplikasi Calculator Sederhana======");
            Console.WriteLine("Pilihan Operasi Hitung : \n 1. Operasi Penambahan \n 2. Operasi Pengurangan \n 3. Operasi Perkalian \n 4. Operasi Pembagian ");
            Console.WriteLine();

            int pilih;
            Console.Write("Masukkan Pilihan Anda (1-4) : ");
            pilih = int.Parse(Console.ReadLine());

            if (pilih == 1)
            {
                Console.Write("Inputkan nilai a = ");
                int a = int.Parse(Console.ReadLine());

                Console.Write("Inputkan nilai b = ");
                int b = int.Parse(Console.ReadLine());

                Console.WriteLine();

                Console.WriteLine("Hasil Penambahan " + a + " + " + b + " = " + Penambahan(a, b));
            }
            else if (pilih == 2)
            {
                Console.Write("Inputkan nilai a = ");
                int a = int.Parse(Console.ReadLine());

                Console.Write("Inputkan nilai b = ");
                int b = int.Parse(Console.ReadLine());

                Console.WriteLine();

                Console.WriteLine("Hasil Pengurangan " + a + " - " + b + " = " + Pengurangan(a, b));
            }
            else if (pilih == 3)
            {
                Console.Write("Inputkan nilai a = ");
                int a = int.Parse(Console.ReadLine());

                Console.Write("Inputkan nilai b = ");
                int b = int.Parse(Console.ReadLine());

                Console.WriteLine();

                Console.WriteLine("Hasil Perkalian " + a + " x " + b + " = " + Perkalian(a, b));
            }
            else if (pilih == 4)
            {
                Console.Write("Inputkan nilai a = ");
                int a = int.Parse(Console.ReadLine());

                Console.Write("Inputkan nilai b = ");
                int b = int.Parse(Console.ReadLine());

                Console.WriteLine();

                Console.WriteLine("Hasil Pembagian " + a + " : " + b + " = " + Pembagian(a, b));
            }
            else
            {
                Console.WriteLine("Pilihan Tidak Tersedia");
            }

            Console.WriteLine("Tekan sembarang untuk keluar");
            Console.ReadKey();
        }

        static int Penambahan(int a, int b)
        {
            return a + b;
        }

        static int Pengurangan(int a, int b)
        {
            return a - b;
        }

        static int Perkalian(int a, int b)
        {
            return a * b;
        }

        static int Pembagian(int a, int b)
        {
            return a / b;
        }
    }
}
