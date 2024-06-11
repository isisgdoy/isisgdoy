

- 👋 Olá mundo! Eu sou a Isis :)
- 👀 Estudante em Análise e desenvolvimento de sistemas
- 🌱 Iniciante na programação
##
<div> 
  
  <a href="https://www.instagram.com/isis_godoy/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a href = "mailto:isisgodoi2@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/isis-valeria-godoy-bueno-33b979230/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
  
</div>

<!---
isisgdoy/isisgdoy is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take fha look at your changes.


using System.ComponentModel.Design;
using System.Security.Cryptography.X509Certificates;


// minhas classe é Program
// Metodo é o Menu
namespace Calculadora
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Menu();
        }

        public static void Menu() 
        {
            Console.Clear();
            Console.WriteLine("Menu:");
            Console.WriteLine("1 - Somar");
            Console.WriteLine("2 - Subtrair");
            Console.WriteLine("3 - Dividir");
            Console.WriteLine("4 - Multiplicação"); 
            Console.WriteLine("5 - Resto da divisão");
            Console.WriteLine("6 - Potenciação");
            Console.WriteLine("0 - Sair"); 

            string opcao = Console.ReadLine();

            switch (opcao)
            {
                case "1":
                    Somar();
                    break;

                case "2":
                    Subtrair();
                    break;

                case "3":
                    Dividir();
                    break;

                case "4":
                    Multiplicacao();    
                    break;

                case "5":   
                    RestoDaDivisao();
                    break;

                case "6":   
                    CalcularPotenciacao();  
                    break;

                case "0":
                    break;

                default:
                    Menu();
                    break;

            }
                
        }

        
        public static void Somar()
        {
            double valor1, valor2;
            Console.WriteLine("Digite o primeiro valor:");
            valor1 = double.Parse(Console.ReadLine());
            Console.WriteLine("Digite o segundo valor:");
            valor2  = double.Parse(Console.ReadLine());

            Console.WriteLine($"{valor1} + {valor2} = {valor1 + valor2}");
            Console.ReadLine();

            Menu();
            
        }


        public static void Subtrair() 
        {
            double valor1, valor2;
            Console.WriteLine("Digite o primeiro valor:");
            valor1 = double.Parse(Console.ReadLine());
            Console.WriteLine("Digite o segundo valor:");
            valor2 = double.Parse(Console.ReadLine());

            Console.WriteLine($"{valor1} - {valor2} = {valor1 - valor2}");

            Console.ReadLine(); 
            Menu();
            
        }


        public static void Dividir()
        {
            double dividendo, divisor;

            Console.WriteLine("Informe o dividendo:");
            dividendo = double.Parse(Console.ReadLine());
            Console.WriteLine("Informe o divisor:");
            divisor = double.Parse(Console.ReadLine());

            if (divisor != 0)
                Console.WriteLine($"{dividendo} / {divisor} = {dividendo / divisor}");
            else
                Console.WriteLine("Não é possível dividir por zero.");

            Console.ReadLine();
            Menu();

        }

        public static void Multiplicacao()
        {
            double valor1, valor2;
            Console.WriteLine("Digite o primeiro valor:");
            valor1 = double.Parse(Console.ReadLine());
            Console.WriteLine("Digite o segundo valor:");
            valor2 = double.Parse(Console.ReadLine());

            Console.WriteLine($"{valor1} * {valor2} = {valor1 * valor2}");

            Console.ReadLine();
            Menu();

        }

        public static void RestoDaDivisao()
        {
            double dividendo, divisor;

            Console.WriteLine("Informe o dividendo:");
            dividendo = double.Parse(Console.ReadLine());
            Console.WriteLine("Informe o divisor:");
            divisor = double.Parse(Console.ReadLine());

            if (divisor != 0)
                Console.WriteLine($"Resto entre {dividendo} e {divisor} = {dividendo % divisor}");
            else
                Console.WriteLine("Não é possível dividir por zero.");

            Console.ReadLine();
            Menu();
        }

        public static void CalcularPotenciacao()
        {
            double basePotenciacao, expoente;

            Console.WriteLine("Informe a base:");
            basePotenciacao = double.Parse(Console.ReadLine());
            Console.WriteLine("Informe o expoente:");
            expoente = double.Parse(Console.ReadLine());

            Console.WriteLine($"{basePotenciacao} elevado a {expoente} = {Math.Pow(basePotenciacao, expoente)}");

            Console.ReadLine();
            Menu();

        }

    }
}

--->
