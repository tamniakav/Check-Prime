using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Prime
{
    class Prime
    {
        static void Main(string[] args)
        {
            int n = int.Parse(Console.ReadLine());

            bool prime = true;

            if (n < 2)
            {
                Console.WriteLine("Not Prime");
            }
            else
            {
                for (int i = 2; i <= Math.Sqrt(n); i++)
                {
                    if (n % i == 0)
                    {
                        prime = false;
                        break;
                    }

                }

                if (prime == true)
                {
                    Console.WriteLine("Prime");
                }
                else 
                {
                    Console.WriteLine("Not Prime");
                }

            }
        }
    }
}
