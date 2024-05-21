## Python - Set

Set mak tipu data mutabel ne'ebé halo kolesaun ba data husi item barak iha variavel ida de'it.

Set mós tipu data ida husi Python ne'ebé uza hodi rai kolesaun data hanesan sira seluk list, tuple no dictionary sira iha diferensa oinsá atu uza. Set simbolika mak **{ }**.

Kolesaun data set mak hanesan:

  - Set mutable bele muda objetu sira iha list ho dict
  - Set immutable la bele muda objetu ka aumenta iha set nia laran hanesan list ho dict
  - Set distinct valór sira ne'ebé dupla
  - Set la simu print ka buka elementu husi índise(unindexed)
  - Set la order objetu (unordered)



```python
>>> numeru = {2, 4, 6, 8, 10} # Kria set numeru 
>>> print(numeru) # print set
{2, 4, 6, 8, 10}

>>> string = {"Mario", "Ano"} # Kria set string
>>> print(string)
{'Mario', 'Ano'}

>>> item = {1, "Jose", 5.5, True} # Kria diferensia objetu
>>> print(item)
{1, 5.5, 'Jose'}
```

Set ida la rai objetu dupla. Maski objetu ida aumenta liu dala ida iha curly brackets laran, iha de'it kopia ida iha objetu ne'ebé define ona. Tanba ne'e, la bele halo operasaun index no slicing iha objetu ne'ebé define ona.

```python
>>> numeru = {1, 2, 2, 3, 4, 4, 5, 5} # elementu 5 mak dupla
>>> print(numeru) # elementu 5 sei print ida deit
{1, 2, 3, 4, 5}
```

**Unordered**

Order ba elementu sira iha set ne'e la nesesariamente hanesan ho orden ne'ebé fó tiha ona. Python optimista estrutura set ida ne'ebé bele hala'o operasaun iha set ne'e mak define iha matemátika ka númeru sira ne'ebé ita fó iha set laran.

```
>>> set1 = {'a', 'b', 'c', 'd'}
>>> print(set1)
{'a', 'c', 'b', 'd'}

>>> set1 = {1, 2, 7, 4, 5}
>>> print(set1)
{1, 2, 4, 5, 7}
```



**Set Mutable**

set mutable nian bele muda tanba set ne'e rasik bele modifika, maibé elementu sira ne'ebé iha set ne'e tenki iha tipu immutable.

```
>>> set1 = {1, 2}
>>> print(set1)
{1, 2}
>>> set1.add(3)
>>> print(set1)
{1, 2, 3}
>>> set1.update([4, 5])
>>> print(set1)
{1, 2, 3, 4, 5}

>>> set1 = {"Mario"}
>>> print(set1)
{'Mario'}
>>> set1.add("Ano")
>>> print(set1)
{'Mario', 'Ano'}

>>> set1 = {("Mario", "Ano")}
>>> print(set1)
{('Mario', 'Ano')}
>>> set1.add("Ony")
>>> print(set1)
{'Ony', ('Mario', 'Ano')}
```

**Set Immutable**

Objetu immutavel (Hashable) mak bele sai parte ida husi objetu set mak hanesan númeru (integer, float, no mós kompleksu), string no tuple, maibé la simu objetu set iha lista, no dictionary.

```python
>>> set_val = {(5, 5), 6, 8} # Bele aumenta tuple iha set nia laran
>>> print(set_val)
{8, (5, 5), 6}
>>> set_val = {[5, 5], 6, 8} # La bele aumenta list iha set nia laran
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unhashable type: 'list'

unhashable type: 'list'
>>> set_val = {[5, 5], 6, 8} # La bele aumenta set iha set seluk nia laran
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unhashable type: 'set'

unhashable type: 'set'
```

Iha ezemplu iha leten, `(5, 5)` mak tuple ida, ne'e duni sai parte husi set. Maibé, `[5, 5]` mak lista ida ne'ebé hatudu mensajen erru ida ne'e dehan katak lista ne'e la bele fó sai (unhashable). (Hashing mak mekanizmu ida iha siénsia komputadór nian ne'ebé permite buka lalais objetu sira iha memória komputadór nian.)

Maski objetu mutavel (bele muda) sira la rai iha set ida, maibé set ne'e rasik mak objetu mutavel ida.

Uza funsaun set () atu kria set ne'ebé mamuk. Empty curly braces sei kria dictionary ne'ebé mamuk duke set ne'ebé mamuk.

```python
>>> set_val = {} # Kria dictionary mamuk
>>> print(set_val)
{}
>>> type(set_val)
<class 'dict'>

>>> set_mamuk = set() # kria set mamuk
>>> print(set_mamuk)
set()
>>> type(set_mamuk)
<class 'set'>
```

Funsaun set () ne'e mós uza hodi transforma objetu string, tuple, ka dictionary ba objetu set hanesan hatudu iha kraik.

```python
>>> s = set('Hello') # konverte string ba set
>>> print(s)
{'e', 'H', 'l', 'o'}

>>> n = set((1,2,7,4,5)) # konverte tuple ba set
>>> print(n)
{1, 2, 4, 5, 7}

>>> i = {1: 'Ida', 2: 'Rua'}
>>> s = set(i) # konverte dict ba set
>>> print(s)
{1, 2}
```

### Modify Set Elements

Uza métodu add (), remove () ka update () hodi modifika kolesaun set.

```python
>>> s = set() # kria set mamuk
>>> s.add(1) # Aumenta elementu 1
>>> s.add(2) # Aumenta elementu 2
>>> print(s)
{1, 2}
>>> s.update([2, 3]) # Update elementu
>>> print(s)
{1, 2, 3}
>>> s.remove(2) # Hamoos elementu
>>> print(s)
{1, 3}
```

### Set Operations

Hanesan temi tiha ona iha leten, tipu dadus ne'ebé define iha Python implementasaun hanesan set ne'ebé define iha matemátika. Bele hala'o operasaun oioin **|, &, - no ^** . Operadór sira halo operasaun ho nia unidade, intervensaun, diferensa no diferensa simetrika (union, intersection, difference, and symmetric difference operations ). Operador sira ne'e ida-idak iha métodu korrespondénsia ne'ebé asosiadu ho klase ne'ebé harii ona.

**Union:** Returns ka fó fila set foun ida ho elementu sira husi set rua ne'ebé la inklui sira ne'ebé dupla no for order.

**Operadór: |**
**Metode:** set.union()

```python
>>> s1 = {1, 2, 3, 4, 5}
>>> s2 = {4, 5, 6, 7}
>>> s1|s2
{1, 2, 3, 4, 5, 6, 7}

>>> s2|s1
{1, 2, 3, 4, 5, 6, 7}
```

```python
>>> s1 = {1, 2, 3, 4, 5}
>>> s2 = {4, 5, 6, 7}
>>> s1.union(s2)
{1, 2, 3, 4, 5, 6, 7}

>>> s2.union(s1)
{1, 2, 3, 4, 5, 6, 7}
```

**Intersection:** Returns ka fó fali set foun ne'ebé kontein elementu ne'ebé hanesan iha set rua ne'e nia laran.

**Operadór:** & 

**Metode:** set.intersection()

```python
>>> s1 = {1, 2, 3, 4, 5}
>>> s2 = {4, 5, 6, 7}
>>> s1&s2
{4, 5}

>>> s2&s1
{4, 5}
```

```python
>>> s1 = {1, 2, 3, 4, 5}
>>> s2 = {4, 5, 6, 7}
>>> s1.intersection(s2)
{4, 5}

>>> s2.intersection(s1)
{4, 5}
```

**Difference**: Returns ka fó fali de'it elementu sira ne'ebé iha set primeiru ne'ebé la'os kontein iha set segundu no la'ós fó elementu sira iha set segundu nian.

**Operadór:** - 

**Metode:** set.difference()

```python
>>> s1 = {1, 2, 3, 4, 5}
>>> s2 = {4, 5, 6, 7}
>>> s1-s2
{1, 2, 3}

>>> s2-s1
{6, 7}
```

```python
>>> s1 = {1, 2, 3, 4, 5}
>>> s2 = {4, 5, 6, 7}
>>> s1.difference(s2)
{1, 2, 3}

>>> s2.difference(s1)
{6, 7}
```

**Symmetric Difference:** Returns ka fó fali set ida ne'ebé kompostu husi elementu sira iha set rua ne'e, maibé la fó elementu sira ne'ebé hanesan iha set rua ka fó de'it elementu unique iha set rua ne'e.

**Operadór: ^** 

**Method:** set.symmetric_difference()

```python
>>> s1 = {1, 2, 3, 4, 5}
>>> s2 = {4, 5, 6, 7}
>>> s1^s2
{1, 2, 3, 6, 7} 

>>> s2^s1
{1, 2, 3, 6, 7}
```

```python
>>> s1 = {1, 2, 3, 4, 5}
>>> s2 = {4, 5, 6, 7}
>>> s1.symmetric_difference(s2)
{1, 2, 3, 6, 7}

>>> s2.symmetric_difference(s1)
{1, 2, 3, 6, 7}
```