##**Python - Variabel**

**Saida mak Variabel ?**

Variavel mak fatin memória rezerva ida hodi rai valór sira. Signifika katak bainhira ita kria variavel ida ita rezerva hela fatin mamuk iha memória, valór sira ne'ebé ita rai bele ho tipu data interger ka karakterístika sira.

### Deklara variabel

Atu deklara variavel iha python partikularmente ita identifika Naran no Valor:

Naran mak hodi identifika variavel.

Valór bele identifika depois operadór `(=)`.

 Por ezemplu:

  ```
a = 1
  ```

![var](https://i.postimg.cc/KYvB4scS/Screen-Shot-2021-03-10-at-6-10-06-PM.png)

Notas: `a` mak identifika ona naran husi variavel no valór mak `1`.

### Naran Variavel

Python naran variavel bele refere ba kualkér naran husi variavel bele hakerek ho letra mais-kula ka minus-kula no bele hakerek dijitál husi 0 to’o 9 no uza símbolu sira hanesan underscore(__)

```
>>> naran = "Mario"
>>> tinan = 30
>>> altura = 168
```
Print variable naran :
```
>>> print(naran)  
>>> print(tinan)  
>>> print(altura)  
```
Fo sai rezultadu:
```
Mario
30
168
```

### Multipla Assignment

Iha python bele kria variavel barak no refere ba valór ida de'it ka ita bele kria valór ida bele assign ba multipla variavel ka variavel oin-oin.

Ezemplu:

a. Assign valór ida ba multipla variavel ka bele kria multipla variavel fó valór ida edit.

```
a = b = c = 10
  
print(a)
print(b)
print(c)
```

b. Assign multipla valor ba multipla variavel 

```
x, y, z = 10, 15, "hello"
  
print (x)
print (y)
print (z)
```

### Tipu Variavel

Tipu python variavel iha rua lokal variabel no global variavel.

**Lokal Variavel**

Lokál variavel mak define iha funsaun nia laran no iha local scope.

Ezemplu:

```
# Deklara funsaun  
def funs():  
	# defini lokal variabel 
    a = 20  
    print("Local variabel a mak", a)  
# bolu funsaun
funs() 
```

Fo sai rezultadu

```
Local variabel a mak 20
```

Globál Variabel bele uza jerál ka la'ós iha funsaun nia laran ka globál scope no bele uza mós iha funsaun nia laran ka local scope maibé tenki uza global keyword.

  Ezemplu:

```
a = 20 # Global variabel
# Deklara funsaun  
def funs():  
    print("global variabel a mak", a)  
# bolu funsaun
funs()
```

Fo sai rezultadu  
```
global variabel a mak 20
```

Ezemplu globál variavel iha funsaun nia laran uza global keyword:

```
# Deklara funsaun  
def funs():
    global a
    a = 20
    # defini lokal variabel 
    print("global a mak", a)  
# bolu funsaun
funs()
```

Fo sai rezultadu

```
global a mak 20
```

Ezemplu kona-ba deklara globál no lokál variavel iha funsaun nia laran:

```
# Deklara funsaun  
def funs():
    global a
    a = 20 
    h = 2  # defini lokal variabel 
    print("global", a, "no local", h)  
  
funs() # bolu funsaun 
```

Fo sai rezultadu

```
global 20 no local 2
```

