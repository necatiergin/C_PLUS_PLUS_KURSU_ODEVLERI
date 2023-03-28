#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream>
#include <utility>

struct Nec {
	Nec() { std::cout << "1"; }
	Nec(Nec &) { std::cout << "2"; }
	Nec(const Nec &) { std::cout << "3"; }
	Nec(Nec &&) { std::cout << "4"; }
	~Nec() { std::cout << "5"; }
};

struct A {
	mutable Nec x;
	A() = default;
	A(const A &) = default;
};

int main() 
{
	A a1;
	A a2 = std::move(a1);
}
```
