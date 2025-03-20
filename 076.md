#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream>

namespace A {
	class Nec {};
	void func(const Nec&) 
	{
		std::cout << "1";
	}
}

namespace B {
	void func(const A::Nec&) 
	{
		std::cout << "2";
	}
}

int main() {
	func(A::Nec());
}
```
