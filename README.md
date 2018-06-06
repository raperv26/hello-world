# hello-world
Just another repository

public int[] SelectionSort(int[] array)
{
    for (int i = 0; i < array.Count(); i++)
    {
        int min = i;
        for (int j = i + 1; j < array.Count(); j++)
        {
            if (array[j] < array[min])
            {
                min = j;
            }
        }

        if (min != i)
        {
            int temp;
            temp = array[min];
            array[min] = array[i];
            array[i] = temp;
        }
    }
    return array;
}
