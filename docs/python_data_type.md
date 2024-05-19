## Tipu Data

Tipu data husi variabel nebe ita kria no fo nia valor bele identifika hanesan tuir mai ne'e bele integer, string ka float no boolean.

### String

String (str) mak tipu data ida nebe fo sai karakteristika iha simbolu ho marka quotation ka  dupla marka quotation.

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

Integer (int) mak tipu data ida nebe ho numeru decimal bele pozitivu no negativu husi 0 zero too 9, bele numeru octal no hexadecimal.

Iha octal inisial ho `0o` no hexadecimal sei hahu ho `0x`.

Valor Positivu

```
>>> x = 10
>>> type(x)
<class 'int'>
```

Valor Negativu

```
>>> y = -10
>>> print(y)
-10
>>> type(y)
<class 'int'>
```

Valor boot

```
>>> z = 100000000000000000000000
>>> print(z)
100000000000000000000000
>>> type(z)
<class 'int'>
```

Valor Octal

```
>>> octalInt = 0o32
>>> print(octalInt)
26
>>> type(octalInt)
<class 'int'>
```

Valor Hexadecimal

```
>>> hexInt = 0xEE
>>> print(hexInt)
238
>>> type(hexInt)
<class 'int'>
```

### Float

Float mak tipu data ida nebe reprezenta numeru ho pontu, nebe ita hakerek ho pontu decimal ka ho string.

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

Boolean tipu data ida nebe ho valor rua deit mak True no False nebe existi.

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
x = 5
y = 10
print(bool(x==y))
```

