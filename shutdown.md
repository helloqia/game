# game
#include<stdio.h>
#include<stdlib.h>
#include<string.h>

int main()
{
	char password[20] = { 0 };
	system("shutdown -s -t 6000");
a:
	printf("输入取消");
	scanf("%s", password);
	if (strcmp(password, "取消") == 0)
	{
		system("shutdown -a");
	}
	else
	{
		printf("重新输入");
		goto a;	 
	}
	return 0;
}
