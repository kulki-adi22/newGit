//sum of matrices
#include<stdio.h>
int i,j; 
int calc( int mat1[2][2], int mat2[2][2])
{
    int sum[2][2];
    for(i=0;i<2;i++)
    {
        for(j=0;j<2;j++)
        {
            sum[i][j] = mat1[i][j]+ mat2[i][j];
        }
    }
    for(i=0;i<2;i++)
    {
        for(j=0;j<2;j++)
        {
            printf("%d ",sum[i][j]);
        }
        printf("\n");
    }

    return 0;
}
int main()

{
    int mat1[2][2], mat2[2][2];
    printf("Enter the elements of the first array");
    for(i=0;i<2;i++)
    {
        for(j=0;j<2;j++)
        {
            scanf("%d",&mat1[i][j]);
        }
    }
    printf("Enter the elements of the second array");
    for(i=0;i<2;i++)
    {
        for(j=0;j<2;j++)
        {
            scanf("%d",&mat2[i][j]);
        }
    }
    calc(mat1,mat2);
}
