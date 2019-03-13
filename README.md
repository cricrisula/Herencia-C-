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


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Examen_Parcial_1
{
     class Figura
    {
        public  string NombreFigura { get; set; }

    }
}



namespace Examen_Parcial_1
{
    class Triangulo:Figura
    {
        private double _Basetri;
        private double _Alturatri;
        private double _Areatri;

        public void calcularAreatri(double pbase,double paltura)
        {

            Basetri = pbase;
            Alturatri = paltura;
            double result = Basetri * Alturatri/2;
            Console.WriteLine("El Area del Triangulo es:"+result);
            Console.WriteLine();
            Console.WriteLine();


        }


        public double Basetri
        {
            get { return _Basetri;}

            set{ _Basetri = value; }
        }

        public double Alturatri
        {
            get
            {
                return _Alturatri;
            }

            set
            {
                _Alturatri = value;
            }
        }

        public double Areatri
        {
            get
            {
                return _Areatri;
            }

            set
            {
                _Areatri = value;
            }
        }
    }
    }

namespace Examen_Parcial_1
{
    class Rectangulo:Figura
    {
        private double _Baserec;
        private double _Alturarec;
        private double _Arearec;


        public void calcularAreaRec(double pAltura, double pBase, double pArea)
        {
            Baserec = pBase;
            Alturarec = pAltura;
            Arearec = pArea;
            double resultado = pAltura * pBase;
            Console.WriteLine(  "El resultado del Area del Rectangulo es: "+resultado);
            Console.WriteLine();
            Console.WriteLine();
        }


        public double Baserec
        {
            get
            {
                return _Baserec;
            }

            set
            {
                _Baserec = value;
            }
        }

        public double Alturarec
        {
            get
            {
                return _Alturarec;
            }

            set
            {
                _Alturarec = value;
            }
        }

        public double Arearec
        {
            get
            {
                return _Arearec;
            }

            set
            {
                _Arearec = value;
            }
        }
    }
    }
    
    
    namespace Examen_Parcial_1
{
    class Circulo:Figura
    {
        private  double _RadioCir;
        private double _AreaCir;
        
        public void calcularAreaCir(double pRadio)

        {

            RadioCir = pRadio;
            
            double result = RadioCir * RadioCir;
            Console.WriteLine("El Area del circuilo es:" + result);


        }

        public double RadioCir
        {
            get
            {
                return _RadioCir;
            }

            set
            {
                _RadioCir = value;
            }
        }

        public double AreaCir
        {
            get
            {
                return _AreaCir;
            }

            set
            {
                _AreaCir = value;
            }
        }
    }
}

