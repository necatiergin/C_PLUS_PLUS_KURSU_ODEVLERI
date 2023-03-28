#### Aşağıdaki C++ programı derlenip çalıştırıldığında ekran çıktısı ne olur?

```
#include <iostream>

class Myclass {
public:
	Myclass()
	{
		static int x{};
		std::cout << x++ << " ";
	}
	
};

int main()
{
	Myclass a[100];
}
```
