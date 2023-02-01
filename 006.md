#### Aşağıdaki C++ programı derlenip çalıştırıldığında standart çıkış akımına ne yazar?

```
int foo(int *p, int *q)
{
	*p = 1;
	*q = 2;
	
	return *p + *q;
}

char str[] = "0123";

#include <iostream>

int main()
{
	using namespace std;

	int a = 3;
	int b = 4;
	int c = foo(&a, &a);
	cout << c;
	(c == a + b ? a : b) = 5;
	cout << a << b;
	int i = 0;
	str[i] = i[str + 2];
	cout << str;
	
} 
```

[ödevin cevabı](https://youtu.be/DDYvnqgowUs)
