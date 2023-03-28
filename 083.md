#### Aşağıdaki kodda bulunan her bir sentaks hatasını işaretleyin ve sentaks hatasının nedenini belirtin:

```
int x = 0;
int y = 0;

class Encloser {	
	int x;
	static int s;  
	static NestedType sn;
public:
	
	class Nested {		
		void func(int ival)
		{
			x = ival; 
			int a = sizeof x; 

			s = ival;   
			::x = ival; 
			y = ival;   
		}
	public:
		void foo(Encloser* p, int i)
		{
			p->x = i;
			NestedType nsx;
		}
	};
	typedef Nested NestedType;
	void encfunc(NestedType n)
	{
		n.foo(this, x);
		n.func(x);
	}
};

```
