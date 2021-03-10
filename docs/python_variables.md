## Python - Variabel

Variabel mak fatin memoria rezerva hodi rai valor sira. Signifika katak bainhira ita kria variabel ida ita rezerva hela fatin mamu iha memoria no tipu data ba variabel, bele rai interger decimal ka karakteristika iha variabel sira.

python - funsaun variable:

### Deklara variabel

  Python deklara variable la partikularmente ho tipu data python waihira ita deklara ka kria variebel ida ita assign valor ba variable simbolikamente hare husi operador (=).

  Por exemple:

```
>>> a = 1
```

![var](/home/nicko/Devel/mkdocs/MKdocs/docs/img/var.png)

### Object referencia

  Python object oriented ne'e integradu ona wanhira ita print kualdu data ho tipu oin-oin

  Ezemplu:

```
>>> print("Mario")
Mario
```

  no ketik:

```
>>> type("Mario")
<class 'str'>  
```

### Naran Variabel

  Python variable names bele refere ba kualker naran husi variabel bele hakereke ho letra maiskula ka minuskula no bele hakerek digital husi 0 to'o 9 no uza simbolu sira hanesan underscore(__)

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

  Fo variabel naran la hanesan :

```
>>> naran = "A"  
>>> Naran = "B"  
>>> naRan = "C"  
>>> NARAN = "D"  
>>> n_a_r_a_n = "E"  
>>> _naran = "F"  
>>> naran_ = "G"  
>>> _naran_ = "H"  
>>> na56ra3 = "I"  
```

  Print :

```
>>> print(naran, Naran, naRan, NARAN, n_a_r_a_n, _naran, naran_, _naran_, na56ra3) 
```

### Multi Assignment

Iha python ita bele kria variabel barak no refere ba valor ida deit ka ita bele kria valor ida bele assign ba multi variabel

  Exemplu:

```
>>> naran = "Mario"
>>> tinan = 30
>>> altura = 168
```

  Print naran variabel: 

```
>>> print(naran)  
>>> print(tinan)  
>>> print(altura) 
```

  Fo sai resultadu:

```
Mario
30
168
```

### Tipu Variabel

  Tipu python variabel iha rua local variabel no global variabel.

  **Local  Variabel**

  Local variabel mak defini iha funsaun nia laran no iha scope funsaun nia laran.

  Exemplu:

```
# Deklara funsaun  
def func():  
	# defini lokal variabel 
	a = 20  
	print("Variabel a mak", a)  
	# bolu funsaun
func() 
```

  Fo sai rezultadu

```
Variabel a mak 20
```

**Global Variabel** 

Global Variabel bele uza jeral ka laos iha funsaun nia laran no bele uza mos iha funsaun nia laran. Python   global variable ita bele defini iha funsaun nia laran uza global keyword.

  Exemplu:

```
a = 20
# Deklara funsaun  
def func():  
	# defini lokal variabel 
	print("global a mak", a)      
    # bolu funsaun
func()
```

  Fo sai rezultadu

```
global a mak 20
```

### Python - Tipu Data

```
>>> my_var = 2
```

my_var mak identifika ona naran husi variabel no valor mak 2 

 Valor nebe ita fo iha variabel ne'e bele troka ba valor seluk. Atu asesu ba variabel importante ita hatene fo variabel nia naran.

```
>>> my_var="Antonio"
>>> print(my_var)
'Antonio'
```

Tipu data husi variabel nebe ita kria no fo nia valor bele identifika hanesan tuir mai ne'e bele integer, string ka float no boolean.

**String**

```
>>> a = "Jose"
>>> print(a)
'Jose'
>>> type(a)
<class 'str'>
```

 **Integer**

```
>>> b = 20
>>> print(b)
20
>>> type(b)
<class 'int'>
```

**Float**

```
>>> c = 2.0
>>> print(c)
2.0
>>> type(c)
<class 'float'>
```

 **Boolean**

```
>>> e = True
>>> print(e)
True
>>> type(e)
<class 'bool'

>>> e = False
>>> print(e)
False
>>> type(e)
<class 'bool'>
```



