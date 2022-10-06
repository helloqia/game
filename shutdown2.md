# game
#include<stdio.h>
#include<stdlib.h>
#include<string.h>

int main()
{
	char password[20] = { 0 };
	system("shutdown -s -t 600");
	while (1)
	{
		printf("输入取消");
		scanf("%s", password);
		if (strcmp(password, "取消") == 0)
		{
			system("shutdown -a");
		}
		else
		{
			printf("重新输入");
		}
	}
	return 0;
}
