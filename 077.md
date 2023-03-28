#### Aşağıdaki `C++` programında bir sentaks hatası var mı? Varsa sentaks hatasının nedeni/nedenleri nedir? Sentaks hatası yok ise ekrana ne yazdırılır?

```
#include <iostream>

namespace Nec {
	struct X{};
	void func(X) { std::cout << "A"; }
}

class Myclass {
public:
	void func(Nec::X) { std::cout << "B";}
	
	void foo()
	{
		Nec::X ax;
		func(ax); 
	}
};

int main()
{
	Myclass mx;
	mx.foo();
}

```
