
#define _CRT_SECURE_NO_WARNINGS
#include <stdlib.h>
#include <stdio.h>

void masterfoo(int* P1, int* P2, int* P3)
{

	if ((*P1 > *P2) && (*P1 > *P3))
	{
		printf("biggest num is %d\n", *P1);
		
	}
	if ((*P2 > *P1) && (*P2 > *P3))
	{ 
		printf("biggest num is %d\n", *P2);
		
	}
	if ((*P3 > *P1) && (*P3 > *P2))
	{
		printf("biggest num is %d\n", *P3);
		
	}
	


	if ((*P1 < *P2) && (*P1 < *P3))
	{
		printf("smallest num is %d\n", *P1);
		
	}
	if ((*P2 < *P1) && (*P2 < *P3))
	{
		printf("smallest num is %d\n", *P2);
		
	}
	if ((*P3 < *P1) && (*P3 < *P2))
	{
		printf("smallest num is %d\n", *P3);
		
	}


}



void main()
{
	int num1 = 1, num2 = 2, num3 = 3;
	masterfoo(&num1, &num2, &num3);

	printf("%d %d %d", num1, num2, num3);
}

