## Aşağıdaki bildirimlerden sentaks hatası oluşturanları belirtiniz:

```
#include <string>

int func(int);

class Myclass {
	static int x = 10; 
	const static bool flag = true;
	const static unsigned char buffer[100] = {0};
	constexpr static int y = 20;
	constexpr static int a[]{ 1, 2, 3, 4, 5 };
	const static double dval = 12.5;
	inline static double d = 3.4;
	inline static std::string name{ "necati" };
	const static enum Color { Blue, Magenta, Red }Scolor = Red;
	inline static int ival = func(12);
};
```
