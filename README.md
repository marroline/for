clase main//

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace DPRN_U3_A4_JMFG
{
    class Program
    {
        static void Main(string[] args)
        {
            //variables.
            int captura;

            //Construtor info.
            info informa = new info("Actividad 4. Programa de estructuras cíclicas", "José Manuel Flores Gasca", "AL12500999");
            Console.WriteLine("Actividad: "+informa.titulo);
            Console.WriteLine("Autor: "+informa.autor);
            Console.WriteLine("Matricula: "+ informa.matricula);
            Console.WriteLine("Fecha: " + DateTime.Now.ToShortDateString());
            Console.WriteLine("Hora : " + DateTime.Now.ToShortTimeString());
            

            //constructor desripcion
            descripcion describe = new descripcion();

            //Pidiendo informaacion al cliente.
            do
            {
                Console.WriteLine("Ingrese el número para obtener el cuadrado: ");
                Console.SetCursorPosition(43, 15);
                captura = Int32.Parse(Console.ReadLine());
            }
            while(captura >=0);
            

            Console.ReadKey();
        }
    }
}




.-.-.-.-.-.-.-.-.-.-.-.-.-

clase info.

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace DPRN_U3_A4_JMFG
{
    class info
    {
        public String titulo, autor, matricula;
        public info (string  titulo, string autor, string matricula)
        {
            this.titulo = titulo;
            this.autor = autor;
            this.matricula = matricula;
        }

        
    }
}



.-.-.-.-.-.-.-.-.-.-.-


clase descripcion.


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace DPRN_U3_A4_JMFG
{
    class descripcion
    {
        public descripcion() 
        {
            Console.WriteLine("");
            Console.WriteLine("********************************************************************************");
            Console.WriteLine("DESCRIPCION:");
            Console.WriteLine("Implementa un programa que solicite un número entero y muestre en pantalla ");
            Console.WriteLine("Su cuadrado calculado por medio de las operaciones aritméticas indicadas.");
            Console.WriteLine("El programa deberá finalizar cuando se introduzca un valor menor o igual a cero.");
            Console.WriteLine("********************************************************************************");
        }

        public static void respuesta(int captura)
        {

        }
    }
}









