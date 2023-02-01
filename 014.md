#### Sentaks hatası olan satırları belirtiniz:

```

auto a;
int &b;
auto c = 10;
int &d = c;
const auto &e = 20;
int &f = ++c;
int &g = c + 5;
int &&h = c % 2;
int func(); int &&j = func();
int &foo(); int &&m = foo();
int ival = 10; int &&rval = ival + 10; int &p = rval;

```


[ödev cevabı](https://vimeo.com/433277804)
