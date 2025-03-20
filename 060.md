#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream>

struct Nec
{
	Nec() { std::cout << "1"; }
	Nec(const Nec&) { std::cout << "2"; }
	~Nec() { std::cout << "3"; }
};

Nec func()
{
	return Nec();
}

int main()
{
	func();
}

```
