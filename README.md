# hack_life
#include <stdio.h>
#include <stdlib.h>
#include<conio.h>

  int max[10][10], need[10][10], Allocated[10][10], Available[10], flag[10], safeSequence[10];
    int pr, resource, i, j, process, c=0;

int main()
{
  

    printf("Enter the no of processes : ");
    scanf("%d", &pr);

    for(i = 0; i< pr; i++)
        flag[i] = 0;

    printf("\n\nEnter the no of resources : ");
    scanf("%d", &resource);

    printf("\n\nEnter the Maximum instances required for each process : ");
    for(i = 0; i < pr; i++)
    {
        printf("\nFor Process %d : ", i + 1);
        for(j = 0; j < resource; j++)
            scanf("%d", &max[i][j]);
    }

    printf("\n\nEnter the value of alloacted instances for each process : ");
    for(i = 0; i < pr; i++)
    {
        printf("\nFor process %d : ",i + 1);
        for(j = 0; j < resource; j++)
            scanf("%d", &Allocated[i][j]);
    }

    printf("\n\nEnter the available value of instances for each resources : ");
    for(i = 0; i < resource; i++)
        scanf("%d", &Available[i]);

        void changeNeed();
  void isSafeSequence();

}
