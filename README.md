# Herencia-C-
Herencia con figuras geometricas
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Examen_Parcial_1
{
    class Program
    {
        static void Main(string[] args)
        {
            double baseTrianguloporcliente;
            double alturaTrianguloporcliente;
            double areaTrianguloporcliente;
            Triangulo figtriangulo;
            figtriangulo = new Triangulo();
            Console.Write("Ingrese el dato de base del triangulo:");
            baseTrianguloporcliente = double.Parse(Console.ReadLine());
            figtriangulo.Basetri = baseTrianguloporcliente;
            Console.WriteLine();
            Console.Write("Ingrese el dato de altura del triangulo:");
            alturaTrianguloporcliente = double.Parse(Console.ReadLine());
            figtriangulo.Alturatri = alturaTrianguloporcliente;
            Console.WriteLine();
            Console.Write("Ingrese el dato de area del triangulo:");
            areaTrianguloporcliente = double.Parse(Console.ReadLine());
            figtriangulo.Alturatri = areaTrianguloporcliente;
            Console.WriteLine();
            Triangulo ImpresionCalculo;
            ImpresionCalculo = new Triangulo();
            ImpresionCalculo.calcularAreatri(alturaTrianguloporcliente, baseTrianguloporcliente);
            double alturaclienterec;
            double baseclienterec;
            double areaclienterec;
            Rectangulo Rec;
            Rec = new Rectangulo();
            Console.WriteLine("ingrese el dato de la base del rectangulo:");
            baseclienterec = double.Parse(Console.ReadLine());
            Console.WriteLine("ingrese el dato de la altura del rectangulo:");
            alturaclienterec = double.Parse(Console.ReadLine());
            Console.WriteLine("ingrese el dato de la area del rectangulo:");
            areaclienterec = double.Parse(Console.ReadLine());
            Rectangulo ImpresionRec;
            ImpresionRec = new Rectangulo();
            ImpresionRec.calcularAreaRec(baseclienterec, alturaclienterec, areaclienterec);
            double radiocliente;
            Circulo cir;
            cir = new Circulo();
            Console.Write("Ingrese el dato de Radio del circulo:");
            radiocliente = double.Parse(Console.ReadLine());
            Circulo ImpresionCalculoCir;
            ImpresionCalculoCir =new  Circulo();
            ImpresionCalculoCir.calcularAreaCir(radiocliente);
        Console.ReadKey();
        }
    }
}
