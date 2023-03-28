#### Aşağıdaki kodda sentaks hatası olan yerleri belirleyiniz ve her bir sentaks hatasının nedenini açıklayınız:

```
namespace A {
	namespace B {
		class Bclass {	};
	}
	using namespace B;

	inline namespace C {
		class Cclass {	};
	}
	
	void func(B::Bclass);
	void foo(C::Cclass);
}


int main()
{
	A::Bclass bx;
	A::Cclass cx;

	func(bx);
	func(cx);
}
```
