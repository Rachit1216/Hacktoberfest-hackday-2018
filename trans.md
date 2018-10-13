#include<stdio.h>
#include<conio.h>
void main()
{
	int i,j,ar[3][3],c;
	clrscr();
	printf("Enter any 3x3 matrix\n");
	for(i=0;i<3;i++)
	{
	for(j=0;j<3;j++)
	{
	 scanf("%d",&ar[i][j]);
	}
	}
	printf("Entered the 3x3 matrix is\n");
		for(i=0;i<3;i++)
	{
	for(j=0;j<3;j++)
	{
	 printf("%d\t",ar[i][j]);
	}
	printf("\n");
	}
	printf("The transpose of this matrix is\n");
	for(i=0;i<3;i++)
	{
		for(j=0;j<3;j++)
	{
	c=i;
	i=j;
	j=c;
	printf("%d\t",ar[i][j]);
	}
	printf("\n");
	}
	getch();
}
