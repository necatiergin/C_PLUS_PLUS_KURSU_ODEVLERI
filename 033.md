#### Aşağıdaki kodlardan herbirinde function overloading ("işlev yüklemesi") olup olmadığını belirtin. Her bir kod için açıklama yapın:

```
void func(int);

void foo()
{
	extern func(int, int);
}
```

```
int func(double);
double func(double);
```

```
int f(double);
int f(double = 0.);
```


```
int g(int);
int g(const int);
```

```
int g(int *p);
int g(int* const p);
```

```
int f(int *p);
int f(const int *p);
```

```
void func(int &);
void func(const int &);
```

```
void g(int);
void g(int &);
```

```
void foo(int &);
void foo(int &&);
```

```
void f(const double &);
void f(double &&);
```

```
typedef int Word;

void f(Word);
void f(int);
```

```
enum Color {gray, red, blue};
void g(Color);
void g(int);
```

```
#include <cstdint>

void func(int32_t);
void func(int);
```

```
int f(bool);
int f(int);
```

```
void foo(char16_t);
void foo(int);
```

```
void func(char);
void func(signed char);
```

```
void f(char);
void f(unsigned char);
```

```
void foo(int(*)(int));
void foo(int(&)(int));
```

```
void g(int[10]);
void g(int *p);
```

```
void foo(int(&)[10]);
void foo(int(&)[20]);
```

[ödev cevabı](https://vimeo.com/433290281)
