#### C++11 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?

```
#include <iostream>
 
class Myclass {
public:
	Myclass() { std::cout << "1"; }
	Myclass(const Myclass &m) { std::cout << "2"; }
	void func() { std::cout << "3"; }
};
 
int main() 
{
	Myclass a[2];
 
	for (auto x : a) {
		x.func();
	}
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
