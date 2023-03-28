#### `main' işlevi içinde yapılan çağrılardan hangileri geçerlidir? Geçerli olan çağrılar karşılığında hangi fonksiyon(lar) çağrılır? 
Sentaks hatası olan durumlarda sentaks hatası nedeni nedir?

```
#include <iostream>

namespace A {
	void func(int)
	{
		std::cout << "void A::func(int)\n";
	}
	//...
}

namespace B {
	void func(double)
	{
		std::cout << "void B::func(double)\n";
	}
	//...
}

void func(int)
{
	std::cout << "void ::func(int)\n";
}

using namespace A;
using namespace B;

int main()
{
	::func(1);
	func(1);
	func(4.5);
  func(9.L);
}
```
