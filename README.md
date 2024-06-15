## Olá, meu nome é Isis!

<p>Desenvolvedora Full Stack</p>



![isisgdoy's Stats](https://github-readme-stats.vercel.app/api?username=isisgdoy&theme=tokyonight&show_icons=true&hide_border=false&count_private=true) 

![isisgdoy's Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=isisgdoy&theme=tokyonight&show_icons=true&hide_border=false&layout=compact)

---

#### 🚀 Minhas Skills

<code><img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/csharp/csharp-original.svg" alt="c"/></code>
<code><img height="32" src="https://cdn.iconscout.com/icon/free/png-512/c-programming-569564.png" alt="c"/></code>
<code><img height="32" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png" alt="Javascript"/></code>
<code><img height="32" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/html/html.png" alt="HTML5"/></code>
<code><img height="32" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/css/css.png" alt="CSS"/></code>
<code><img height="32" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/bootstrap/bootstrap.png" alt="Bootstrap"/></code>
<code><img height="32" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/mysql/mysql.png" alt="MySQL"/></code>


---
</br>

<div> 
  
  <a href="https://www.instagram.com/isis_godoy/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a href = "mailto:isisgodoi2@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/isis-valeria-godoy-bueno-33b979230/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
   
</div>

<!---
isisgdoy/isisgdoy is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take fha look at your changes.

CALCULADORA

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



JOGAR DADOS

>> program.cs



using JogoDeDados;
using System;
using System.Diagnostics.Metrics;

namespace JogarDados // modulo
{
    class Program //classe
    {
        static void Main(string[] args) // metodos (funções) esse método deve receber como parâmetro um array de String (nomeado args)
        {
            MetodosJogo metodosJogo = new(); // chamando a classe para instancias os metodos 

            Console.Clear();

            metodosJogo.ConfigurarJogos(); // instanciando os metodos da classe metodoJogo
            metodosJogo.IniciarRodadas();

        }
    }
}


>>> MetodosJogo.cs



using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace JogoDeDados
{
    public class MetodosJogo
    {
        // criação das variaveis para acessar os jogadores de qqlr metodo

        public static string Jogador1;
        public static string Jogador2;

        // variavel para armazenar a pontuação dos jogos 

        public static byte PontosJogador1;
        public static byte PontosJogador2;

        // variavel para armazenar a rodada atual

        public static byte RodadaAtual;


        public void ConfigurarJogos()
        {
            RodadaAtual = 0; // campo/fields (variavel criada pra ser acessado em qqlr metodo)

            CriarJogadores(); //  metodos
            AtualizarPlacar();//  metodos

            Console.WriteLine($"\n Jogadores {Jogador1} e {Jogador2} criados. Pressione qulaquer tecla pra continuar.");
            Console.ReadKey(); // Obtém o próximo caractere ou tecla de função pressionada pelo usuário. // Console é a classe e ReadKey é o metodo

        }


        public static void CriarJogadores()
        {
            Console.WriteLine("Informe o nome do primeiro jogador:");
            Jogador1 = Console.ReadLine()!;
            PontosJogador1 = 0;

            Console.WriteLine("Informe o nome do segundo jogador:");
            Jogador2 = Console.ReadLine()!;
            PontosJogador2 = 0;

        }

        public static void AtualizarPlacar()
        {
            Console.Clear(); //é usado para limpar as mensagens do console
            Console.WriteLine($"Pontos do jogador {Jogador1}: {PontosJogador1}");
            Console.WriteLine($"Ponstos do jogador {Jogador2}: {PontosJogador2}");
            Console.WriteLine();

            if (RodadaAtual == 0)
            {

                Console.WriteLine("Jogo nao iniciado...");
            }

        }


        public void IniciarRodadas()
        {
            AtualizarPlacar();
            if (RodadaAtual == 3)
            {
                FinalizarJogo();
                return;
            }

            RodadaAtual++; // incrementando no metodo RodadaAtual

            Console.WriteLine($"Rodada {RodadaAtual} iniciada!\n");
            Console.WriteLine($"Jogador {Jogador1} precisone enter para fazer sua jogada...");
            Console.ReadLine();
            byte ValorTiradoJogador1 = JogarDado();
            Console.WriteLine($"Valor do dado jogado pelo {Jogador1}: {ValorTiradoJogador1}");

            Console.WriteLine($"Rodada {RodadaAtual} iniciada!\n");
            Console.WriteLine($"Jogador {Jogador2} precisone enter para fazer sua jogada...");
            Console.ReadLine();
            byte ValorTiradoJogador2 = JogarDado();
            Console.WriteLine($"Valor do dado jogado pelo {Jogador2}: {ValorTiradoJogador2}");

            if (ValorTiradoJogador1 == ValorTiradoJogador2)
            {
                Console.WriteLine($"O jogador {Jogador1} tirou: {ValorTiradoJogador1} e o {Jogador2} tirou: {ValorTiradoJogador2}. Empate!");
                Console.WriteLine("Pressione ENTER para continuar com o jogo...");
                Console.ReadLine();
            }
            else
            {
                string Vencedor;

                if (ValorTiradoJogador1 > ValorTiradoJogador2)
                {
                    Vencedor = Jogador1;
                    PontosJogador1++;

                }
                else
                {
                    Vencedor = Jogador2;
                    PontosJogador2++;

                }

                Console.WriteLine($"{Jogador1} tirou o numero {ValorTiradoJogador1} e {Jogador2} tirou o numero {ValorTiradoJogador2}. O vencedor foi: {Vencedor}, da rodada {RodadaAtual}");
                Console.WriteLine("Pressione ENTER para continuar o jogo...");
                Console.ReadLine();

            }

            IniciarRodadas();

        }
        public static byte JogarDado()
        {
            Random gerador = new Random(); // gera numeros aleatórios 
            return Convert.ToByte(gerador.Next(1, 6)); //Converte um valor especificado em um inteiro sem sinal de 8 bits.

        }
        public static void FinalizarJogo()
        {

            AtualizarPlacar();
            Console.WriteLine("Jogo finalizado!!!");

            if (PontosJogador1 == PontosJogador2)
            {
                Console.WriteLine("Empate!");
            }
            else if (PontosJogador1 > PontosJogador2)
            {
                Console.WriteLine($"O jogador {Jogador1} venceu com {PontosJogador1} pontos!");
            }
            else
            {
                Console.WriteLine($"O jogador {Jogador2} venceu com {PontosJogador2} pontos!");
            }
        }

    }
}




HORA E DATA


using System;
using System.Threading;

namespace HoraeData 
{

    public class Program 
    {
        public static string diaDaSemana;
        public static string mes;

        public static void Main(string[] args)
        {
            

            Console.WriteLine("========================");
            Console.WriteLine($"Hora & data");
            Console.WriteLine("========================");
            

            while (true)  // Contador do Programa, atualiza a data e hora a cada 1 segundo 
            {       
                    switch ((int)DateTime.Now.DayOfWeek) // para determinar o dia da semana
                {
                    case 0:
                        diaDaSemana = "Domingo";
                        break;
                    case 1:
                        diaDaSemana = "Segunda-Feira";
                        break;
                    case 2:
                        diaDaSemana = "Terça-Feira";
                        break;
                    case 3:
                        diaDaSemana = "Quarta-Feira";
                        break;
                    case 4:
                        diaDaSemana = "Quinta-Feira";
                        break;
                    case 5:
                        diaDaSemana = "Sexta-Feira";
                        break;
                    case 6:
                        diaDaSemana = "Sábado";
                        break;
                    default:
                        diaDaSemana = "N/D";
                        break;
                }

                
                switch ((int)DateTime.Now.Month) // Switch para determinar o nome do mês
                {
                    case 1:
                        mes = "Janeiro";
                        break;
                    case 2:
                        mes = "Fevereiro";
                        break;
                    case 3:
                        mes = "Março";
                        break;
                    case 4:
                        mes = "Abril";
                        break;
                    case 5:
                        mes = "Maio";
                        break;
                    case 6:
                        mes = "Junho";
                        break;
                    case 7:
                        mes = "Julho";
                        break;
                    case 8:
                        mes = "Agosto";
                        break;
                    case 9:
                        mes = "Setembro";
                        break;
                    case 10:
                        mes = "Outubro";
                        break;
                    case 11:
                        mes = "Novembro";
                        break;
                    case 12:
                        mes = "Dezembro";
                        break;
                    default:
                        mes = "N/D";
                        break;
                }

                // Data e Hora são atualizados usando a mesma linha no console
                //{0} = diaDaSemana
                //{ 1} = mes
                //{ 2} =

                Console.Write("\r{0} - {1} de {2} de {3} - {4}", diaDaSemana, DateTime.Now.ToString("dd"), mes, DateTime.Now.ToString("yyyy"), DateTime.Now.ToString("HH:mm:ss"));

                Thread.Sleep(1000); // Thread Principal espera 1 segundo antes de continuar o loop


            }



        }

    }

}

}





--->
