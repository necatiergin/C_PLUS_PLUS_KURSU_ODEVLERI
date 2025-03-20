#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream>

class Myclass {
public:
	explicit Myclass(int) 
	{
		std::cout << "i";
	};
	Myclass(char) 
	{
		std::cout << "c";
	};
};

int main() 
{
	Myclass c1{ 7 };
	Myclass c2 = 7;
}

```
