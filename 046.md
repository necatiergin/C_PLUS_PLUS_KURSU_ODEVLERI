#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream>

class F;

class C {
public:
	C() { std::cout << "C"; }
	friend C F::createC();
};

class F {
public:
	F() { std::cout << "F"; }

	C createC() { return C(); }
};

int main() {
	F f;
	C c = f.createC();
}

```
