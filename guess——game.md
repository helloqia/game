# game
#include<stdio.h>
#include<stdlib.h>
#include<time.h>


void mune(int n)
{
	printf("***********************************************\n");
	printf("***********1.game                  ************\n");
	printf("***********2.exit                   ***********\n");
	printf("***********************************************\n");
}

void game(int n)
{
	int x;
	x = rand() % 100 + 1;
	while (1)
	{
		int guess;
		printf("请猜数字:");
		scanf("%d", &guess);
		if (x > guess)
		{
			printf("小了\n");
		}
		else if (x < guess)
		{
			printf("大了\n");
		}
		else
		{
			printf("恭喜");
			break;
		}
	}
}
int main()
{
	srand((unsigned int)time(NULL));
	int n;
	do {
		printf("请选择\n");
		mune(1);
		scanf("%d", &n);
		switch (n)
		{
		case 1:
			game(1);
			break;
		case 0:
			printf("退出游戏\n");
			break;
		default:
			printf("输入错误\n");
			break;
		}
	}
	while (n);

}
