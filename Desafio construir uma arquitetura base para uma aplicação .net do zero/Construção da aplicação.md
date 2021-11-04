Desafio construir uma aplicação .net do zero: 


using System;
namespace Desafio
{
    class Program
    {
        static void Main(string[] args)
        {
         Console.WriteLine("###################- Programa para calcular a media de um aluno -#################### ");
         Console.WriteLine("Digite sua primeira nota: ");
         float Nota1 = float.Parse(Console.ReadLine()); 
         Console.WriteLine("Digite sua segunda nota: ");
         float Nota2 = float.Parse(Console.ReadLine()); 
         Console.WriteLine("Digite sua terceira nota: ");
         float Nota3 = float.Parse(Console.ReadLine()); 
         Console.WriteLine("Digite sua quarta nota: ");
         float Nota4 = float.Parse(Console.ReadLine()); 
         float media = (Nota1 + Nota2 + Nota3 + Nota4) / 4;
         if (media < 7 && media >= 4)
         {
             Console.WriteLine("Você está em recuperação! Média = "+ media);
         }  
         else if (media < 4 && media >= 0)
         {
             Console.WriteLine("Você foi reprovado! Média = "+ media);
         }
         else if (media >= 7 && media <=10)
         {
             Console.WriteLine("Você foi aprovado! Parabéns! Média = "+media);
         }
        }
    }
}