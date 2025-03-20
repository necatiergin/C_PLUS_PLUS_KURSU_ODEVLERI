#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream>

struct Nec {
	Nec() { std::cout << "A"; }
	Nec(const Nec&) { std::cout << "B"; }
	Nec(Nec &&) { std::cout << "C"; }
	~Nec() { std::cout << "D"; }
	void foo() { std::cout << "E"; }
} nec;

int main() 
{
	Nec(nec);
	nec.foo();
}
```
