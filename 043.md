#### C++17 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?


```
#include <iostream>
 
class Myclass  {
public:
	Myclass() 
	{ 
		std::cout << "Myclass"; 
	}
};
 
int main() 
{
	Myclass m1();
	Myclass *m2(); 
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
