# Example-AdvanceComPro

Ex 1.1
#include<stdio.h>
int main()
{
	int a, b, temp;
	
	printf("Example of Running\n");
	printf("Enter the value of a : ");
	scanf("%d", &a);
	printf("Enter the value of b : ");
	scanf("%d", &b);
	printf("a = %d b = %d\n===", a, b);
	
	temp = a;
	a = b;
	b = temp;
	
	printf("\na = %d b = %d", a, b);

	return 0;
}


Ex 1.2
#include<stdio.h>
int main()
{
	int a, b;
	
	printf("Example of Running\n");
	printf("Enter the value of a : ");
	scanf("%d", &a);
	printf("Enter the value of b : ");
	scanf("%d", &b);
	printf("a = %d b = %d\n===", a, b);
	
	a = a + b;
	b = a - b;
	a = a - b;
	
	printf("\na = %d b = %d", a, b);
	
	return 0;
}


Ex 2.1
#include<stdio.h>
int main()
{
	int n1, n2;
	
	printf("Enter number 1 : ");
	scanf("%d", &n1);
	printf("Enter number 2 : ");
	scanf("%d", &n2);
	
	if(n1 > n2)
		printf("min = %d, max = %d", n2, n1);
	else
		printf("min = %d, max = %d", n1, n2);
		
	return 0;
}


Ex 2.2
#include<stdio.h>
int main()
{
	int n1, n2, min, max;
	
	printf("Enter number 1 : ");
	scanf("%d", &n1);
	printf("Enter number 2 : ");
	scanf("%d", &n2);

	max = n1 > n2 ? n1 : n2;
	min = n1 < n2 ? n1 : n2;
	printf("min = %d max = %d\n", min, max);
	
	return 0;
}


Ex 3
#include<stdio.h>
int main()
{
	int a, b, c, min, mid, max;
	
	printf("Enter number 1 : ");
	scanf("%d", &a);
	printf("Enter number 2 : ");
	scanf("%d", &b);
	printf("Enter number 3 : ");
	scanf("%d", &c);

	min = a < b ? a : b;
	min = c < min ? c : min;
	max = a > b ? a : b;
	max = c > max ? c : max;
	mid = (a + b + c) - min - max;
	
	printf("mid = %d,mid = %d max = %d", min, mid, max);
	
	return 0;
}


Ex 4
#include<stdio.h>
int main()
{
	int a, b;
	
	printf("Enter number : ");
	scanf("%d", &a);

	for(b = 1; b <= a; b++ )
	{
		printf("%c", '*');
	}
	
	return 0;
}


Ex 5
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num; j++ )
		{
			printf("%c", '*');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 6
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= i; j++ )
		{
			printf("%c", '*');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 7
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num - i + 1; j++ )
		{
			printf("%c", '*');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 8
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= i - 1; j++)
		{
			printf("%c", ' ');
		}
		for(j = 1; j <= num - i + 1; j++ )
		{
			printf("%c", '*');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 9
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num - i; j++)
		{
			printf("%c", ' ');
		}
		for(j = 1; j <= i; j++ )
		{
			printf("%c", '*');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 10
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num - i; j++)
		{
			printf("%c", ' ');
		}
		for(j = 1; j <= 2 * i - 1; j++ )
		{
			printf("%c", '*');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 11
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= i - 1; j++)
		{
			printf("%c", ' ');
		}
		for(j = 1; j <= 2 * (num - i) + 1; j++ )
		{
			printf("%c", '*');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 12
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= 2 * num; i++)
	{
		for(j = 1; j <= abs(num - i); j++)
		{
			printf("%c", ' ');
		}
		for(j = 1; j <= 2 *(num - abs(num - i)) - 1; j++ )
		{
			printf("%c", '*');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 13
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num; j++)
		{
			if(i == 1 || i == num || j == 1 || j == num)
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 14
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= i; j++)
		{
			if(j == 1 || i == num || j == i)
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 15
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num - i + 1; j++)
		{
			if(i == 1 || j == 1 || j == num - i + 1)
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 16
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= i - 1; j++)
			printf("%c", ' ');
		for(j = 1; j <= num - i + 1; j++)
		{
			if(i == 1 || j == 1 || j == num - i + 1)
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 18
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num - i; j++)
		{
			printf("%c", ' ');
		}
		for(j = 1; j <= 2 * i - 1; j++ )
		{
			if(i == num || j == 1 || j == 2 * i - 1)
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 19
#include<stdio.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= i - 1; j++)
		{
			printf("%c", ' ');
		}
		for(j = 1; j <= 2 * (num - i) + 1; j++ )
		{
			if(i == 1 || j == 1 || j == 2 * (num - i) + 1 )
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 20
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= 2 * num; i++)
	{
		for(j = 1; j <= abs(num - i); j++)
		{
			printf("%c", ' ');
		}
		for(j = 1; j <= 2 *(num - abs(num - i)) - 1; j++ )
		{
			if(j == 1 || j == 2 *(num - abs(num - i)) - 1)
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 21
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num; j++)
		{
			if((i+j)%2==0)
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 22
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= num; i++)
	{
		for(j = 1; j <= num; j++)
		{
			if(i == 1 || i == num ||j == 1 || j == num || i == j || j == num - i + 1)
				printf("%c", '*');
			else
				printf("%c", ' ');
		}
		printf("\n");
	}
	
	return 0;
}


Ex 23
#include <stdio.h>
#include <math.h>
int main()
{
	int num, i, j, numI, numJ;
	
	printf("Enter number : ");
	scanf("%d", &num);
	
	for(i = 1; i <= (2*num)-1; i++)
	{
		for(j = 1; j <= (2*num)-1; j++)
		{
				numI = num - abs(num-i);
				numJ = num - abs(num-j);
				
				if(numI < numJ)
					printf("%d", numI);
				else
					printf("%d", numJ);
		}
		printf("\n");
	}
	
	return 0;
}
