#### Aşağıdaki C++ programı hakkında yorum yapınız:

+ sentaks hatası
+ tanımsız davranış
+ derleyiciye göre değişir
+ ekrana şunu yazar: 

```
#include <iostream>

using namespace std;

class Nec {
public:
	Nec() { cout << "c"; }
	~Nec() { cout << "d"; }
};

int n = 2;

int main() {
erg:
	Nec nec;
	if (n--)
		goto erg;
}
```
