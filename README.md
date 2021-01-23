# vs2013--1-23
#define _crt_secure_no_warnings 1
int my_strlen(char* str)
{
	int count = 0;
	while (*str != '\0')
	{
		count++;
		str++;
	}
	return count;
}
int main()
{
	char arr[] = "bit";
	//int len=strlen(arr）；//求字符串长度
	//printf("%d\n",len)
	//模拟实现了一个strlen函数
	int len = my_strlen(arr);//arr是数组，数组传参，传过去的不是整个数组，而是第一个元素的地址
	printf("len=%d\n", len);
	return 0;
}
//
//int my_strlen(char* str)
//{
//	if (*str != '\0')
//		return 1 + my_strlen(str + 1);
//	else
//		return 0;
//}
//int main()
//{
//	char arr[] = "bit";
//	int len = my_strlen(arr);
//	printf("len=%d\n", len);
//	return 0;
//}
//
////练习3：求n的阶乘，不考虑溢出
//int factorial(int n)
//{
//	if (n <= 1)
//		return i;
//	else
//		return n* factorial(n - 1);
//}
//
//int Fac1(int n)
//{
//	int i = 0;
//	inr ret = 1;
//	for (i = 1; i <= n; i++)
//	{
//		ret *= i;
//	}
//	return ret;
//}
//int main()
//{
//	//求n的阶乘
//	int n = 0;
//	int ret = 0;
//	scanf(:%d, &n);
//	ret = Fac1(n);//循环的方式
//	printf("%d\n", ret);
//	return 0;
//}
//
//int Face2(int n)
//{
//	if (n <= 1)
//		return 1;
//	else
//		return n*Face2(n - 1);
//}
//
////斐波那契数列
////1 1 2 3 5 8 13 21 34 55
////描述第n个斐波那契数的时候
//int Fib(int n)
//{
//	if (n <= 2)
//		return 1;
//	else
//		return Fib(n - 1) + Fib(n - 2);
//}
//int main()
//{
//	int n = 0;
//	int ret = 0;
//	scanf("%d", &n);
//	//TDD-测试驱动开发
//	ret = Fib(n);
//	printf("ret=%d\n", ret);
//	return 0;
//}
//
////50
////49 48
////48 47 47 46
////47 46 46 45 45 44 
//int main()
//{
//	int n = 0;
//	int ret = 0;
//	scanf("%d", &n);
//	//TDD-测试驱动开发
//	ret = Fib(n);
//	printf("ret=%d\n", ret);
//	printf("count=%d\n", count);
//	return 0;
//}
//
////描述第n个斐波那契数的时候
//int count = 0;
//int Fib(int n)
//{
//	if (n == 3)//测试第三个斐波那契数的计算次数
//	{
//		count++;
//	}
//	if (n <= 2)
//		return 1;
//	else
//		return Fib(n - 1) + Fib(n - 2);
//}
//
//int Fib(int n)
//{
//	int a = 1;
//	int b = 1;
//	int c = 0;
//	while (n > 2)
//	{
//		c = a + b;
//		a = b;
//		b = c;
//		n--;
//	}
//	return c;
//}
//
//void test(int n)
//{
//	if (n < 10000)
//	{
//		test(n + 1);
//	}
//}
//int main()
//{
//	test(1);
//	return 0;
//}
