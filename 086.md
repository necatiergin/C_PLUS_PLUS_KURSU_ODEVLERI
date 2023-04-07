#### Bir std::string nesnesi üzerinde aşağıdaki silme işlemlerini gerçekleştirmeniz gerekiyor:

01. Yazının ilk karakterini silin.
02. Yazının son karakterini silin.
03. Yazının ilk ve son karakterleri dışında tüm karakterlerini silin.
04. Yazının ikinci karakterini silin.
05. Yazının sondan ikinci karakterini silin.
06. idx yazının geçerli bir indeksi olmak üzere yazının *idx* indisli karakterini silin.
07. Yazıdaki ilk *a* karakterini silin.
08. Yazıdaki son *a* karakterini silin.
19. Yazıdaki tüm *a* karakterlerini silin.
10. Yazıdaki ilk *a* karakteri ile başlayan ve son *a* karakteri ile biten yazıyı silin.
11. Yazıdaki ilk *a* karakterinden önce gelen ve sonra gelen *2* karakteri silin.
12. Yazıda bulunan ilk *"kan"* yazısını silin
13. Yazıda bulunan son *"kan"* yazısını silin
14. Yazıda bulunan tüm *"kan"* yazılarını silin
15. Yazıda bulunan ilk rakam karakterini silin
16. Yazıda bulunan son rakam karakterini silin
17. Yazıdaki tüm rakam karakterlerini silin.
18. Yazının uzunluğu 1'den büyükse ve yazının ilk karakteri ile son karakteri aynı ise bunları silin.
19. Yazının uzunluğu 5'ten büyükse ve yazının ilk *3* karakteri ile son *3* karakteri aynı ise bunları silin.
20. Yazıdaki ardışık eşit karakterlerden sadece bir tane kalacak şekilde silme işlemi yapın. *(unique)*
21. Yazıdaki tüm boşluk *(whitespace)* karakterlerini silin.

**Aşağıdaki test kodunu kullanabilirsiniz:**

```
#include <string>
#include <iostream>

void print(const std::string &s)
{
	std::cout << "'" << s << "' [" << s.length() << "]\n";
}

int main()
{
	std::string s;

	std::cout << "bir yazi giriniz: ";
	std::getline(std::cin, s);
	print(s);
	///kod
	print(s);
}

```
