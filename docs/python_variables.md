##**Python - Variabel**

**Saida mak Variabel ?**

Variavel mak fatin memória rezerva ida hodi rai valór sira. Signifika katak bainhira ita kria variavel ida ita rezerva hela fatin mamuk iha memória, valór sira ne'ebé ita rai bele ho tipu data interger ka karakterístika sira.

### Deklara variabel

Atu deklara variavel iha python partikularmente ita identifika `Naran` no `Valor`

`Naran` mak hodi identifika  variavel

`Valor` bele identifika depois operadór (=)  

  Por ezemplu:

  ```
  a = 1
  ```

![var](https://i.postimg.cc/KYvB4scS/Screen-Shot-2021-03-10-at-6-10-06-PM.png)

Notas: a mak identifika ona naran husi variavel no valor mak 1 

### Naran Variabel

Python naran variavel bele refere ba kualkér naran husi variavel bele hakerek ho letra maiskula ka minuskula no bele hakerek dijitál husi 0 to’o 9 no uza símbolu sira hanesan underscore(__)

```
>>> naran = "Mario"
>>> tinan = 30
>>> altura = 168
```

Print variavel naran :

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

Iha python bele kria variavel barak no refere ba valor ida deit ka ita bele kria valor ida bele assign ba multipla variavel ka variavel oin-oin.

  Ezemplu:

Assign valor ida ba multipla variavel ka bele kria multipla variavel fo valor ida edit.

```
a = b = c = 10

print(a)
print(b)
print(c)
```

Assign multipla valor ba multipla variavel 

```
x, y, z = 10, 15, "hello"

print (x)
print (y)
print (z)
```

### Tipu Variavel

Tipu python variavel iha rua local variavel no global variavel.

**Local Variavel**

Local variavel mak defini iha funsaun nia laran no iha local scope.

Ezemplu:

```
# Deklara funsaun  
def func():  
    # defini lokal variabel 
    a = 20  
    print("Variavel a mak", a)  
  # bolu funsaun
func() 
```

Fó sai rezultadu

```
Variavel a mak 20
```

Global Variavel bele uza jeral ka laos iha funsaun nia laran ka global scope no bele uza mos iha funsaun nia laran ka local scope maybe tenki uza global keyword. 

Ezemplu:

```
a = 20 # Global variabel
# Deklara funsaun  
def func():  
    print("global a mak", a)  
    # bolu funsaun
func()
```

Fó sai rezultadu

```
global a mak 20
```

Ezemplu global variavel iha funsaun nia laran uza global keyword:

```
# Deklara funsaun  
def func():
    global a
    a = 20
    # defini lokal variabel 
    print("global a mak", a)  
# bolu funsaun
func()
```

Fó sai rezultadu

```
global a mak 20
```

Ezemplu konaba deklara global no local variavel iha funsaun nia laran:

```
# Deklara funsaun  
def func():
    global a
    a = 20 
    h = 2  # defini local variabel 
    print("global", a, "no local", h)  
  
func() # bolu funsaun 
```
