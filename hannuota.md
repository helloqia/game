# game
#include<stdio.h>
#include<stdlib.h>
#include<time.h>
#include<string.h>

void hannota(int n,char A,char B,char C )
{
	int c=1;
	if (n == 1)
		printf("%c->%c\n",A,C);
	else
	{
		hannota(n - 1, A, C, B);
		printf("%c->%c\n", A, C);
		hannota(n - 1, B, A, C);	
	}}

int main()
{
	int n;
	scanf("%d", &n);
	hannota(n, 'A', 'B', 'C');
	return 0;
}

