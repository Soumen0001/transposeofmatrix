# transposeofmatrix
#include<stdio.h>

int main(){
	int i,j,rows,coloumns, a[10][10], b[10][10];
	
	printf("please enter number of rows nand coloumns \n");
	scanf("%d %d", &i, &j);
	
	printf("please enter the array elements \n");
	for(rows = 0; rows < i; rows++)
	{
		for(coloumns = 0; coloumns < j; coloumns++)
		{
		scanf("%d", &a[rows][coloumns]);
		}
	}
	
	
	for(rows = 0; rows < i; rows++)
	{
		for(coloumns = 0;coloumns < j; coloumns++)
		{
			b[coloumns][rows] = a[rows][coloumns];
		}
	}
	printf("Transpose Matrix are \n");
	for(rows = 0;rows < j; rows++)
	{
		for(coloumns = 0;coloumns < i; coloumns++)
		{
			printf("%d \t", b[rows][coloumns]);
		}
		printf("\n");
	}
	return 0;
}
