#### _Nec_ sınıfının tanımımnda sentaks hatası oluşturan bildirimleri işaretleyiniz.


```
#include <string>

class Nec {
	int i1 = 20;
	int i2(30);
	int i3{ 20 };
	constexpr static double dval{ 3.0 };
	static const pi{ 3.14159 };
	static const int x = 83246;
	inline static std::string str{ "necati" };
	const static int primes[] = { 2, 3, 5, 7, 9, 13 };
	inline static int i4 = i1;
};
```
