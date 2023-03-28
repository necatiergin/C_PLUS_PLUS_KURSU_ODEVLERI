#### C++17 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?


```
#include <iostream>
 
class Myclass {
public:
	Myclass(int x) : x(x) 
	{
		std::cout << x;
	}
	
	~Myclass() 
	{ 
		std::cout << x + 3;
	}
 
private:
	int x;
};
 
int main() 
{
	const Myclass &c = Myclass(1);
	Myclass(2);
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
