#### _Nec_ sınıfının _foo_ isimli üye fonksiyonu içinde sentaks hatası oluşturan deyimleri _(statements)_ işaretleyin. 

```
class Nec {

	void foo() const
	{
		bar(); // 1
		baz(); // 2
		++m_val;
		++m_s; // 3
	}

	void bar();

	static void baz();

	static int m_s;
	int m_val;

};
```
