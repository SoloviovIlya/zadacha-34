//  Задайте массив заполненный случайными положительными трёхзначными числами. Напишите программу, которая покажет количество чётных чисел в массиве.
//[345, 897, 568, 234] -> 2

void Chet(int[] a, int n)

{

    int m = 0;
    
    for (int i=0;i<n;i++)
    
    {
    
       if (a[i]%2 == 0)
       
       {
        m = m+1;
       }
       
    }
    
    Console.WriteLine($"Количество четных чисел в массиве равно {m}");
    
}

int n = new Random().Next(5,11);

int[] a = new int[n];

for (int i = 0; i<n; i++)

{

    a[i] = new Random().Next(100,1000);
    
    Console.WriteLine(a[i]);
    
}

Chet(a, n);
