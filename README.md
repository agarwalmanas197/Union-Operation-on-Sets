# Union-Operation-on-Sets
write a program in c to create two sets and perform the union operation on sets.


The collection of well-defined distinct objects is known as a set. The word well-defined refers to a specific property which makes it easy to identify whether the given object belongs to the set or not. The word ‘distinct’ means that the objects of a set must be all different. 


Union Of Sets:-
Union of two given sets is the smallest set which contains all the elements of both the sets.
To find the union of two given sets A and B is a set which consists of all the elements of A and all the elements of B such that no element is repeated.
The symbol for denoting union of sets is ‘∪’. 
For example;
Let set A = {2, 4, 5, 6}
and set B = {4, 6, 7, 8}
Taking every element of both the sets A and B, without repeating any element, we get a new set = {2, 4, 5, 6, 7, 8}
This new set contains all the elements of set A and all the elements of set B with no repetition of elements and is named as union of set A and B.






Program -


#include<stdio.h>

#include<conio.h>

int main()

{

    int a[10],b[10],m,n,i,j;

    int c[20],k=0,flag=0;

    int ch;

    printf("Enter the number of elements in first set:\n");

    scanf("%d",&m);

    printf("Enter the elements:\n");

    for(i=0;i<m;i++)

    {

        scanf("%d",&a[i]);

    }

    printf("\nElement of First set:\n");

    for(i=0;i<m;i++)

    {

        printf("%d\t",a[i]);

    }

    printf("\nEnter the number of elements in second set:\n");

    scanf("%d",&n);

    printf("Enter the elements:\n");

    for(i=0;i<n;i++)

    {

        scanf("%d",&b[i]);

    }

    printf("\nElement of Second set:\n");

    for(i=0;i<n;i++)

    {

        printf("%d\t",b[i]);

    }

    for(i=0;i<m;i++)

    {

        c[k]=a[i];

        k++;

    }

    for(i=0;i<n;i++)

    {

        flag=0;

        for(j=0;j<m;j++)

        {

            if(b[i]==c[j])

            {

                flag=1;

                break;

            }

        }

    if(flag==0)

        {

            c[k]=b[i];

            k++;

        }

    }

    printf("\nElement of resultant set\n");

    for(i=0;i<k;i++)

    {

        printf("%d\t",c[i]);

    }

} 
OUTPUT
Enter the number of elements in first set:
5
Enter the elements:
1
2
3
4
5

Element of First set:
1       2       3       4       5
Enter the number of elements in second set:
5
Enter the elements:
6
7
8
5
4

Element of Second set:
6       7       8       5       4
Element of resultant set
1       2       3       4       5       6       7       8
