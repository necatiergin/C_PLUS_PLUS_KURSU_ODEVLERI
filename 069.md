#### Aşağıdaki C++ kodunda bir sentaks hatası/hataları olup olmadığını belirtiniz. Varsa, her bir sentaks hatasının nedenini açıklayınız:

```
void f();

namespace A {
	void g();
}

namespace X {
	using ::f; 
	using A::g; 
}

void h()
{
	X::f(); 
	X::g(); 
}
```
