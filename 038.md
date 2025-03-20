#### C++17 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?


```
#include <initializer_list>
#include <iostream>
 
class Myclass {
public:
	Myclass() 
	{
		std::cout << "default ctor.\n";
	}
 
	Myclass(int)
	{
		std::cout << "ctor with int param\n";
	}
 
	Myclass(std::initializer_list<int>)
	{
		std::cout << "ctor with init_list param\n";
	}
};
 
int main() 
{
	Myclass m1;
	Myclass m2{};
	Myclass m3{ 1 };
	Myclass m4{ 1, 2 };
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
