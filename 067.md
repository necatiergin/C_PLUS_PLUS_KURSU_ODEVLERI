#### _Nec_ sınıfının _foo_ isimli üye fonksiyonu içinde sentaks hatası oluşturan deyimleri _(statements)_ işaretleyin. 

```
class Nec {

	void foo()
	{
		m_val = 10; //1
		m_s = 20; //2
		this->m_s = 30; //3
		bar(); //4
		baz(); //5
		this->bar(); //6
		this->baz();  //7
		void (*fp1)() = &bar; //8
		void (*fp2)() = &baz; //9
		Nec::m_s++; //10
		Nec::baz(); //11
	}

	void bar();

	static void baz();

	static int m_s;
	int m_val;

};
```
