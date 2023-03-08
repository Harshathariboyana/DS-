#include<stdio.h>
void main ()
{
    int arr [20],size,i,j,temp;
    printf ("enter the size of array");
    scanf ("%d",&size);
    printf ("enter the elements of array");
    for(i=0;i<size;i++)
    {
        printf ("\n enter the %d elements",i+1);
        scanf("%d",&arr[i]);
    }
    /* code for selection sort*/
    for(i=0;i<size;i++)
 
    {        for (j=0;j<size;j++)
        {
            if (arr [j]>arr[j+1])
            {
                temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }
        }
            
    }
    /*end of the code for selection sort*/
    printf ("\n selection array is ....");
    for (i=0;i<size;i++)
    printf ("\t%d",arr[i]);
}
