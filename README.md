# c-questions
different c programs that i learned


//duplicate numbers

void duplicate_num(int arr[], int size, int* count){

    for (int i = 0; i < size; i++)
    {
        if (arr[i]==i)
        {
            (*count)++;
        }
    }
}
int main(){
    int count=0;
    int arr[]={1,5,2,0,4,8,6};
    int size = sizeof(arr)/sizeof(arr[0]);
    duplicate_num(arr,size,&count);
    printf("%d",count);
    return 0;
}



// array reverse program

void reverse_arr(int arr[], int size)          //ahiya parameter " arr[]" hoi  not "arr[a]"
{
    printf("Reversed array :\n");
    for (int i = size - 1; i >= 0; i--)
    {
        printf("%d, ", arr[i]);
    }
}

int main()
{
    int a;
    printf("enter the length of array");
    scanf("%d",&a);

    int arr[a];
    for (int i = 0; i < a; i++)
    {
        scanf("%d", &arr[i]);
    }

    reverse_arr(arr,a);

    return 0;
} 

// sum of elements of array


void array_sum(int arr[], int size)
{

    int sum;
    for (int i = 0; i < size; i++)   //ahiya i<size as parameter int size che
    {
        sum+= arr[i];
    }
    printf("sum of elemnts of array: %d", sum);
}

int main()
{
    int a;
    printf("enter the length of array");
    scanf("%d", &a);

    int arr[a];
    for (int i = 0; i < a; i++)
    {
        scanf("%d", &arr[i]);
    }

    array_sum(arr, a);
    return 0;
}

