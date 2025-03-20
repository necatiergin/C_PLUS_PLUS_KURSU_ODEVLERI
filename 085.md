#### Aşağıdaki işlevleri tanımlayınız ve kendi yazacağınız test kodu (kodları) ile test ediniz:

```
std::string opposite_case(const std::string &s);
```

işlev parametresi ile aldığı yazıdaki 
 + küçük harflerin yerinde aynı karakterlerin büyüğü olan
 + büyük harflerin yerinde aynı karakterlerin küçüğü olan

bir string döndürecek.

```
std::string remove_chars(const std::string &source, const std::string &scars);

```

İşlevin geri dönüş değeri olan *string*'in değeri source *string*'i içinden *scars* stringinin karakterlerinin silinmiş hali olacak.
<br>Örnek (parantezler yazılara dahil değil)

*source*           : (ankaranin tasina bak gozlerimin yasina bak) <br>
*scars*            : (kain ) <br>
*geri dönüş değeri*: (rtsbgozlermysb)

```
std::string trim(const std::string &source);
```

işlevin geri dönüş değeri olan string source stringinin başındaki ve sonundaki boşluk karakterlerinin silinmiş hali olacak:

```
(     necati ergin     )  ->  (necati ergin)
```

parantezler yazıya ait değil.
