#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream>

class Nec {
public:
	Nec(int i) : i(i) { std::cout << i; }
	~Nec() { std::cout << i + 4; }

private:
	int i;
};

int main() {
	Nec&& nec = Nec{ 0 };
	Nec{ 1 };
	Nec{ 2 };
}
```
