#### C++17 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?


```
#include <iostream>
#include <vector>
 
struct A
{
	A()
	{
		std::cout << "d";
	}
	
	A(const A&)
	{
		std::cout << "c";
	}
};
 
int main()
{
	std::vector<A> avec(4);
}
``


__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
