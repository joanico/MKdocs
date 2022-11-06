## Tipu Data

Tipu data husi variavel ne'ebé ita kria no fó nia valór bele identifika hanesan tuir mai ne'e bele integer, string ka float no boolean.

### String

String (str) mak tipu data ida ne'ebé fó sai karakterístika iha símbolu ho marka quotation ida ka marka quotation kaduak.

a. Quotation ida

```
>>> a = 'Jose'
>>> type(a)
<class 'str'>
```

b. Quotation kaduak

```
>>> b = "Maria"
>>> type(b)
<class 'str'>
```

### Integer

Integer (int) mak tipu data ida ne'ebé ho númeru decimal bele pozitivu no negativu husi `0` zero to'o `9`, bele númeru octal no hexadecimal.

Iha octal inisiál ho `0o` no hexadecimal sei hahú ho `0x`.

a. Valor Positivu

```
>>> x = 10
>>> type(x)
<class 'int'>
```

b. Valor Negativu

```
>>> y = -10
>>> print(y)
-10
>>> type(y)
<class 'int'>
```

c. Valor boot

```
>>> z = 100000000000000000000000
>>> print(z)
100000000000000000000000
>>> type(z)
<class 'int'>
```

d. Valor Octal

```
>>> octalInt = 0o32
>>> print(octalInt)
26
>>> type(octalInt)
<class 'int'>
```

e. Valor Hexadecimal

```
>>> hexInt = 0xEE
>>> print(hexInt)
238
>>> type(hexInt)
<class 'int'>
```

### Float

Float mak tipu data ida ne'ebé reprezenta númeru ho pontu, ne'ebé ita hakerek ho pontu decimal ka ho string.

a. Reprezenta float ho integer

```
>>> x = float(10)
>>> print(x)
10.0
>>> type(x)
<class 'float'>
```

b. Reprezenta float ho string

```
>>> y = float("10")
>>> print(y)
10.0
>>> type(y)
<class 'float'>
```

### Boolean

Boolean tipu data ida ne'ebé ho valór rua de'it mak True no False ne'ebé eziste.

```
>>> a = True
>>> type(a)
<class 'bool'>

>>> b = False
>>> type(b)
<class 'bool'>
```

Kompara entre valor rua 

```
>>> x = 5
>>> y = 10
>>> print(bool(x==y))
False
```

