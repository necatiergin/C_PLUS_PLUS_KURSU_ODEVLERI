#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream> 

typedef long long mylong;

void func(unsigned myllong) 
{
	std::cout << '1';
}

void func(unsigned long long) 
{
	std::cout << '2';
}

int main() 
{
	func(0ULL);
}
```
[ödevin cevabı](https://www.youtube.com/watch?v=Xjl2nA5E_Os)
