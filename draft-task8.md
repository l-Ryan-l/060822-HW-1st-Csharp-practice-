

Console.WriteLine("Введите любое целое положительное число: "); 
int N = int.Parse(Console.ReadLine()!);

void FillArray(int[] collection)
{
    int lenght = collection.Length;
    int index = 0;
    while (index < lenght)
    { 
        collection[index] = new Random().Next(1, N);
        index++;
    }

}

//void PrintArray(int[] col)
//{
//    int count = col.Length;
//    int position = 0;
//    while (position < count)
//    {
//        Console.WriteLine(col[position]);
//        position++;
//    }
//}

int[] array = new int[N];

FillArray(array);

for(int i = 0; i <= N; i++)
{
    if (i % 2 == 0)
    {
        Console.WriteLine(i + "");
    }
}

