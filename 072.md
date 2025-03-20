#### Aşağıdaki C++ kodunda (varsa) sentaks hatası olan yerleri belirtiniz. Her bir sentaks hatasının nedenini açıklayınız. `main` fonksiyonu içindeki `using` bildiriminin `main` fonksiyonunun üstündeki global isim alanına `(global namespace)` taşınması durumunda yine sentaks hatası olan (varsa) yerleri belirtiniz ve her bir sentaks hatasının nedenini açıklayınız.

```
#include <iostream>

namespace Nec {
	void func(int)
	{
		std::cout << "void Nec::func(int)\n";
	}

	void func(double)
	{
		std::cout << "void Nec::func(double)\n";
	}
}

int func()
{
	std::cout << "int func()\n";
	return 1;
}

// using Nec::func; //2
int main()
{
	using Nec::func; //1

	func();
	func(12);
	func(2.5);
}
```
