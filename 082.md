#### Mark the syntax errors, if any, in the following code sections
```
namespace nec {
	class A {
	public:
		class B {};
	};

	void foo(A::B);
}

int main()
{
	nec::A::B bx;
	foo(bx);
}
```
