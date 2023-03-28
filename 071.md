#### C++17 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?

```
#include<iostream>
 
int func()
{
	return 0;
}
 
class Myclass
{
public:
	static int i;
	static int func()
	{
		return 1;
	}
};
 
int Myclass::i = func();
 
int main()
{
	std::cout << Myclass::i;
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
