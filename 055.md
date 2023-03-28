#### C++17 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?

```
#include <iostream>
 
class Nec {
public:
	Nec() { std::cout << "A"; }
	Nec(const Nec&) { std::cout << "B"; }
	Nec(Nec&&) { std::cout << "C"; }
	~Nec() { std::cout << "D"; }
};
 
Nec func()
{
	return Nec{};
}
 
int main()
{
	func();
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
