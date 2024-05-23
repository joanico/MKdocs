## Python - Tuples

Tuple mak kolesaun ida-ne'ebé la bele muda (unchangeable) ba elementu sira husi tipu dadus oioin. Nee mak kolesaun ida ne'ebé halo tuir ona, nune'e nia prezerva orden ba elementu sira ne'ebé define ona.

Tuple sira define husi elementu enclosing iha parenteses (), haketak husi komma. Tuir mai deklara tipu variable tuple.

```python
>>> tpl=() # tuple mamuk
>>> print(tpl)
()
>>> naran=('fahi', 'rusa', 'bibi', 'manu')
>>> print(naran)
('fahi', 'rusa', 'bibi', 'manu')
>>> numeru=(1, 2, 3, 4, 5) # int tuple
>>> print(numeru)
(1, 2, 3, 4, 5)
>>> item=(1, "fahi", True, 30, "rusa")
>>> print(item)
(1, 'fahi', True, 30, 'rusa')
```

Maibe, la presiza loke no taka elementu tuple sira iha parentesia. Objetu tuple bele inklui elementu sira ne'ebé haketak husi komma ne'ebé la iha parente.

```python
>>> naran='fahi', 'rusa', 'bibi', 'manu' #String tuple
>>> print(naran)
('fahi', 'rusa', 'bibi', 'manu')
>>> numeru=1, 2, 3, 4, 5
>>> print(numeru)
(1, 2, 3, 4, 5)
>>> item=1, "fahi", True, 30, "rusa"
>>> print(item)
(1, 'fahi', True, 30, 'rusa')
```

Tuple la bele deklara ho elementu ida de'it se karik la uza komma hafoin elementu idą.

```python
>>> naran = ('Timor') # Konsidera hanesan tipu string deit
>>> print(type(naran))
<class 'str'>
>>> naran = ('Timor',) # Tipu tuple ho elementu ida nebe haketak husi comma
>>> print(type(naran))
<class 'tuple'>
```

### Asesu elementu tuple

Elementu ida-idak iha tuple hetan asesu liuhusi índise iha square brackets  [ ]. Indise ida hahú ho zero no remata ho (numeru elementu 0, -1), hanesan hatudu iha kraik.

```python
>>> naran=('fahi', 'rusa', 'bibi', 'manu')
>>> print(naran[0])
fahi
>>> print(naran[1])
rusa
>>> print(naran[2])
bibi
>>> print(naran[-1])
manu


>>> numeru=(1, 2, 3, 4, 5)
>>> print(numeru[0])
1
>>> print(numeru[2])
3
>>> print(numeru[-1])
5
```

Tuple mós suporta índise negativu, hanesan ho tipu lista. Indise negativu primeiru hahú husi ***- numeru***  no remata ho ***-1*** ba elementu ikus.

```python
>>> naran=('fahi', 'rusa', 'bibi', 'manu')
>>> print(naran[-4])
fahi
>>> print(naran[-3])
rusa
>>> print(naran[-2])
bibi
>>> print(naran[-1])
manu
```

Se elementu iha índise espesífiku ne'e la eziste, entaun sei mosu erru "índise out of range".

```python
>>> print(naran[5])
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
IndexError: tuple index out of range

tuple index out of range
```

Elementu tuple nia bele la halo pakote no atribui ka troka ba variavel sira, hanesan hatudu iha kraik. Maibe, númeru variavel sira tenke korresponde ho númeru elementu sira iha tuple nia laran se lae, mosu erru.

```python
>>> naran=('fahi', 'rusa', 'bibi', 'manu')
>>> a, b, c, d = naran
>>> print (a, b, c, d)
fahi rusa bibi manu

>>> print (a, b, c, d, e)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'e' is not defined
```

### Atualiza ka hamoos elementu sira tuple

Tuple la bele troka. bainhira kria tiha tuple ida, kualkér operasaun ne'ebé buka atu troka ninia konteúdu la bele. Porezemplu, koko atu modifika ka hasai elementu naran tuple sei rezulta erru.

```python
>>> naran=('fahi', 'rusa', 'bibi', 'manu')
>>> naran[-1] = "krau"
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object does not support item assignment

>>> del naran[-1]
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object doesn't support item deletion
```

Maibe, ita bele hasai duple tomak uza liafuan-xave `del`.

```python
>>> del naran
```

### Class Tuple 

Tipu tuple mak klase tuple. Haree tipu variavel ne'ebé uza funsaun **type ()**.

```python
>>> naran=('fahi', 'rusa', 'bibi', 'manu')
>>> print('tipu naran: ', type(naran))
tipu naran:  <class 'tuple'>
>>> numeru=(1, 2, 3, 4, 5)
>>> print('tipu numeru: ', type(numeru))
tipu numeru:  <class 'tuple'>
```

Konstrutór `tuple ()` uza atu transforma kualkér iterable ba tipu tuple.

```python
>>> tpl=tuple('Helo')
>>> print(tpl)
('H', 'e', 'l', 'o')
>>> tpl=tuple([1, 2, 3, 4, 5])
>>> print(tpl)
(1, 2, 3, 4, 5)
>>> tpl=tuple({1, 2, 3, 4, 5})
>>> print(tpl)
(1, 2, 3, 4, 5)
>>> tpl=tuple({1:"ida", 3:"tolu"})
>>> print(tpl)
(1, 3)
```

### Operasaun Tuple

Opersaun tuple(tuple operation) hanesan ho string no objetu tuple mós hanesan sekuensia ida. Tanba nee, operador sira ne'ebé uza ho string mós disponivel ba tuple.

Operador **+** fó fila rezultadu tuple ida-ne'ebé inklui elementu hotu-hotu husi objetu tuple primeiru no segundu.

```python
>>> T1 = (1,2,3,4,5)
>>> T2 = (6,7,8)
>>> T1+T2
(1, 2, 3, 4, 5, 6, 7, 8)

>>> T1+(6,)
(1, 2, 3, 4, 5, 6)
```

\* Operador Concatenates kopia multipla husi tuple ne'ebé hanesan.

```python
>>> T1 = (1,2,3,4,5)
>>> T2 = (6,7,8)
>>> T1*2
(1, 2, 3, 4, 5, 1, 2, 3, 4, 5)
```

Operador **[ ]** fo fali rezultadu item iha índise ne'ebé iha ona. Indise negativu sura hosi pozisaun sorin loos.

```python
>>> T1 = (1,2,3,4,5)
>>> T1[2]
3

>>> T1[-2]
4
```

Operador **[:]** fo fali rezultadu item sira iha range ne'ebé espesífika husi operandu índise rua ne'ebé haketak husi `:` símbolu.

Se operandu primeiru la hetan, entre númeru ne'ebe hahú husi zero. Se operandu daruak la iha, range ne'e ba to'o tuple nia rohan.

```python
>>> T1 = (1,2,3,4,5)
>>> T1[1:2]
(2,)

>>> T1[1:4]
(2, 3, 4)

>>> T1[3:]
(4, 5)

>>> T1[:3]
(1, 2, 3)
```

Operador **in** ne'e karik fó fali loos se item ida eziste iha tuple ne'ebé fó ona.

```python
>>> T1 = (1,2,3,4,5)
>>> 3 in T1
True

>>> 6 in T1
False
```

Operador **not in** karik la fo fila fali loos se item ida la eziste iha tuple ne'ebé fó ona.

```python
>>> T1 = (1,2,3,4,5)
>>> 5 not in T1
False

>>> 6 not in T1
True
```

