#### C++11 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?


```
#include <iostream>
#include <exception>
 
int g = 0;
 
class Member {
public:
	Member() 
	{
		std::cout << 'm';
		if (g++ == 0) {
			throw std::exception();
		}
	}
	~Member()
	{
		std::cout << 'M';
	}
};
 
class Owner {
public:
	Owner()
	{
		std::cout << 'o';
	}
	
	~Owner()
	{
		std::cout << 'O';
	}
	
	Member m;
};
 
void foo()
{
	static Owner owner;
}
 
int main()
{
	try {
		foo();
	}
	catch (std::exception &) {
		std::cout << 'c';
		foo();
	}
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
