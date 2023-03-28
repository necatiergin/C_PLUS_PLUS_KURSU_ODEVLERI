#### C++17 standartlarına göre aşağıdaki C++ programı çalıştırıldığında bu programın çıktısı ne olur?


```
#include <iostream>
 
struct A {
	A() { std::cout << "a"; }
	~A() { std::cout << "A"; }
};
 
struct B {
	B() { std::cout << "b"; }
	~B() { std::cout << "B"; }
};
 
struct C {
	C() { std::cout << "c"; }
	~C() { std::cout << "C"; }
};
 
struct D {
	D() { std::cout << "d"; }
	~D() { std::cout << "D"; }
};
 
A a;
 
void f1() { static C c; }
void f2() { D d; }
 
int main()
{
	B b;
	f1();
	f2();
}
```

__Sorunun yanıtı şu seçeneklerden biri de olabilir:__

+ Sentaks hatası *(syntax error)*
+ Tanımsız davranış *(undefined behavior)*
+ Derleyiciye göre değişir *(implementation defined)*
