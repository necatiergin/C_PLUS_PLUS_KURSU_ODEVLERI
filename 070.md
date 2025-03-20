#### Aşağıdaki C++ kodunda bir sentaks hatası/hataları olup olmadığını belirtiniz. Eğer varsa, her bir sentaks hatasının nedenini açıklayınız. Her bir fonksiyon çağrısı için hangi fonksiyonun çağrıldığını belirtiniz.


```
namespace A {
	struct X {};
	struct Y {};
	void f(int);
	void g(X);
}

namespace B {
	void f(int i)
	{
		f(i);
	}

	void g(A::X x)
	{
		g(x);
	}

	void h(A::Y y)
	{
		h(y);
	}
}
```
