using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace Calculadora
{
    class Program
    {
        enum Menu { Soma = 1, Subtracao,Divisao, Multiplicacao, Potencia, Raiz, Sair }

        static void Main(string[] args)
        {
            
            Menu menu = Menu.Soma;

            bool escolheuSair = false;
            while(!escolheuSair)
            {

            
            Console.WriteLine("Calculadora RpvS:");
            Console.WriteLine("1-Soma\n2-Subtração\n3-Divisão\n4-Multiplicação\n5-Potência\n6-Raiz\n7-Sair");

            Menu opcao = (Menu)int.Parse(Console.ReadLine());
                
            switch (opcao)
                {
                    case Menu.Sair:
                        escolheuSair = true;
                        break;
                    case Menu.Soma:
                        Soma();
                        break;
                    case Menu.Subtracao:
                        Subtracao();
                        break;
                    case Menu.Multiplicacao:
                        Multiplicacao();
                        break;
                    case Menu.Divisao:
                        Divisao();
                        break;
                    case Menu.Potencia:
                        Potencia();
                        break;
                    case Menu.Raiz:
                        Raiz();
                        break;
                }
            Console.WriteLine(opcao);

                Console.Clear();
            }

        }
        static void Soma()
        {
            Console.WriteLine("Soma de dois numeros: ");
            Console.WriteLine("Digite o primeiro numero: ");
            int a = int.Parse(Console.ReadLine());
            Console.WriteLine("Digite o segundo numero: ");
            int b = int.Parse(Console.ReadLine());
            int resultado = a + b;
            Console.WriteLine("O resultado é: " + resultado);
            Console.WriteLine("Aperte ENTER para voltar para o menu");
            Console.ReadLine();

        }
        static void Subtracao()
        {
            Console.WriteLine("Subtração de dois numeros: ");
            Console.WriteLine("Digite o primeiro numero: ");
            int a = int.Parse(Console.ReadLine());
            Console.WriteLine("Digite o segundo numero: ");
            int b = int.Parse(Console.ReadLine());
            int resultado = a - b;
            Console.WriteLine("O resultado é: " + resultado);
            Console.WriteLine("Aperte ENTER para voltar para o menu");
            Console.ReadLine();

        }
        static void Multiplicacao()
        {
            Console.WriteLine("Multiplicação de dois numeros: ");
            Console.WriteLine("Digite o primeiro numero: ");
            int a = int.Parse(Console.ReadLine());
            Console.WriteLine("Digite o segundo numero: ");
            int b = int.Parse(Console.ReadLine());
            int resultado = a * b;
            Console.WriteLine("O resultado é: " + resultado);
            Console.WriteLine("Aperte ENTER para voltar para o menu");
            Console.ReadLine();

        }
        static void Divisao()
        {
            Console.WriteLine("Divisão de dois numeros: ");
            Console.WriteLine("Digite o primeiro numero: ");
            float a = int.Parse(Console.ReadLine());
            Console.WriteLine("Digite o segundo numero: ");
            float b = int.Parse(Console.ReadLine());
            float resultado = a / b;
            Console.WriteLine("O resultado é: " + resultado);
            Console.WriteLine("Aperte ENTER para voltar para o menu");
            Console.ReadLine();

        }
        static void Potencia()
        {
            Console.WriteLine("Potencia de um numero: ");
            Console.WriteLine("Digite a base: ");
            int baseNumero = int.Parse(Console.ReadLine());
            Console.WriteLine("Digite o expoente: ");
            int expoente = int.Parse(Console.ReadLine());
            int resultado = (int)Math.Pow(baseNumero,expoente);
            Console.WriteLine("O resultado é: " + resultado);
            Console.WriteLine("Aperte ENTER para voltar para o menu");
            Console.ReadLine();

        }
        static void Raiz()
        {
            Console.WriteLine("Raiz de um numero: ");
            Console.WriteLine("Digite o numero: ");
            int a = int.Parse(Console.ReadLine());
            double resultado = Math.Sqrt(a);
            Console.WriteLine("O resultado é: " + resultado);
            Console.WriteLine("Aperte ENTER para voltar para o menu");
            Console.ReadLine();

        }
    }



}
