#### C++17 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?

```
#include <iostream>
 
struct A {
	A() 
	{
		std::cout << "1";
	}
 
	A(const A &x) 
	{
		std::cout << "2";
	}
	
	const A &operator=(const A &x)
	{
		std::cout << "3";
		return *this;
	}
};
 
int main()
{
	A x;
	A y(x);
	A z = y;
	z = x;
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
