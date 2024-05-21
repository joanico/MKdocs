## Tipu Data

Tipu data husi variavel ne'ebé ita kria no fó nia valór bele identifika hanesan tuir mai ne'e bele integer, string ka float no boolean.

### String

String (str) mak tipu data ida ne'ebé fó sai karakterístika iha símbolu ho marka quotation ka  dupla marka quotation.

Single quotation

```
>>> a = 'Jose'
>>> type(a)
<class 'str'>
```

Double quotation

```
>>> b = "Maria"
>>> type(b)
<class 'str'>
```

### Integer

Integer (int) mak tipu data ida ne'ebé ho númeru decimal bele pozitivu no negativu husi 0 zero to'o 9, bele númeru octal no hexadecimal.

Iha octal inisiál ho `0o` no hexadecimal sei hahú ho `0x`.

Valór Positivu

```
>>> x = 10
>>> type(x)
<class 'int'>
```

Valór Negativu

```
>>> y = -10
>>> print(y)
-10
>>> type(y)
<class 'int'>
```

Valór boot

```
>>> z = 100000000000000000000000
>>> print(z)
100000000000000000000000
>>> type(z)
<class 'int'>
```

Valór Octal

```
>>> octalInt = 0o32
>>> print(octalInt)
26
>>> type(octalInt)
<class 'int'>
```

Valór Hexadecimal

```
>>> hexInt = 0xEE
>>> print(hexInt)
238
>>> type(hexInt)
<class 'int'>
```

### Float

Float mak tipu data ida ne'ebé reprezenta númeru ho pontu, ne'ebé ita hakerek ho pontu decimal ka ho string.

Reprezenta float ho integer

```
>>> x = float(10)
>>> print(x)
10.0
>>> type(x)
<class 'float'>
```

Reprezenta float ho string

```
>>> y = float("10")
>>> print(y)
10.0
>>> type(y)
<class 'float'>
```

### Boolean

Boolean tipu data ida ne'ebé ho valór rua de'it mak `True` no `False` ne'ebé eziste.

```
>>> a = True
>>> type(a)
<class 'bool'>

>>> b = False
>>> type(b)
<class 'bool'>
```

Kompara entre valór rua 

```
x = 5
y = 10
print(bool(x==y))
```

