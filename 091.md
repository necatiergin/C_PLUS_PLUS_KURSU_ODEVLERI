#### Bir std::string nesnesi üzerinde aşağıdaki ekleme (insert) işlemlerini gerçekleştirmeniz gerekiyor:

01. Yazının başına 'X' karakterini ekleyin.
02. Yazının sonuna 'X' karakterini ekleyin.
03. Yazıya 'W' karakterini yazının 3 indeksli karakteri olacak biçimde ekleyin. 
04. Yazının başına "kendi isminizi" ekleyin.
05. Yazının sonuna "kendi isminizi" ekleyin.
06. Yazının sonuna yazının uzunluğunu ekleyin: necati ----> necati6
07. Yazıda bulunan rakam karakterlerinden bir tane daha ekleyin:   a4b71p9eak23t ----> a44b7711p99eak2233t


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
