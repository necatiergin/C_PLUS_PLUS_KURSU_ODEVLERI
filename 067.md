#### _Nec_ sınıfının _foo_ üye fonksiyonu içinde sentaks hatası oluşturan kodları işaretleyin.

```
class Nec {
	static void foo()
	{
		Nec nec;
		nec.mval = 10; //1
		nec.sval = 10; //2
		nec.bar(); //3
		nec.baz(); //4
		bar(); //5
		baz();  //6
		sval = 10; //7
		auto x = mval; //8
	}

	static void bar();
	void baz();
	static int sval;
	int mval;
};
```
