<h3>Aşağıdaki programın çıktısı ne olur? Açıklayınız:</h3>

```
#include <iostream>

int foo()
{
	static int x{};
	
	return ++x;
}

void func(int i = foo())
{
	std::cout << i;
}

int main()
{
	func();
	func();
	func();
}
```

[Ödevin cevabı](https://vimeo.com/551901741)
