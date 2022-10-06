using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
namespace ConsoleApplication1
{
    public class LONG
    {

        double Dow(int x1, int x2, int y1, int y2)
        {

            double d = (Math.Sqrt(Math.Pow((x2 - x1), 2) + Math.Pow((y2 - y1), 2)));
            return d;
        }

        class TestPerson
        {
            static void Main()
            {
                double z1, z2, z3, z4, P;
                LONG l = new LONG();

                z1 = l.Dow(0, 2, 2, 3);
                z2 = l.Dow(2, 3, 3, 0);
                z3 = l.Dow(0, 3, 0, 0);
                z4 = l.Dow(0, 0, 2, 0);
                P = z1 + z2 + z3 + z4;
                Console.WriteLine(z1);
                Console.WriteLine(z2);
                Console.WriteLine(z3);
                Console.WriteLine(z4);
                Console.WriteLine("Perimeter =  " + P);
            }
        }
    }
}
