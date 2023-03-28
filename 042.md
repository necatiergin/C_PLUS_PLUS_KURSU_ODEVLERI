#### Aşağıdaki kodda bulunan sentaks hatalarını işaretleyiniz:

```
class A {
public:
	explicit A(int);
	//
};

void f1(A);
void f2(A &);
void f3(const A &);
A f4() { return 1; }

int main()
{
	A a1{ 12 };
	A a2(24);
	A a3 = 35;
	A a4 = static_cast<A>(45);
	f1(1);
	f2(2);
	f3(3);
}
```
