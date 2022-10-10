# game
void one(int n)
{
		int i;
		for (i = 30; i >= 0; i -= 2)
		{
			printf("%d", (n >> i)&1);
		}
		printf("\n");
		for (i = 31; i >= 0; i -= 2)
		{
			printf("%d", (n >> i)&1);
		}
}
int main()
{
	int n;
	scanf("%d", &n);
	one(n);
	return 0;
}

