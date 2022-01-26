## **Python - Variabel**

Variabel mak fatin memoria rezerva hodi rai valor sira. Signifika katak bainhira ita kria variabel ida ita rezerva hela fatin mamu iha memoria no tipu data ba variabel, bele rai interger decimal ka karakteristika iha variabel sira.

### Deklara variabel

  Python deklara variabel la partikularmente ho tipu data python waihira ita deklara ka kria variabel ida ita assign valor ba variabel simbolikamente hare husi operador (=).

  Por exemplu:

```
a = 1
```

<img src="https://i.postimg.cc/9fDgFS7r/Screen-Shot-2021-03-11-at-4-48-43-PM.png" alt="var" style="zoom: 50%;" />

### Object referencia

  Python object oriented ne'e integradu ona wainhira ita print diretamente no ita bele print data ho tipu oin-oin.

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

  Python naran variabel bele refere ba kualker naran husi variabel bele hakerek ho letra maiskula ka minuskula no bele hakerek digital husi 0 to'o 9 no uza simbolu sira hanesan underscore(__)

```
>>> naran = "Mario"
>>> tinan = 30
>>> altura = 168
```

  Print naran variabel :

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
naran = "A"  
Naran = "B"  
naRan = "C"  
NARAN = "D"  
n_a_r_a_n = "E"  
_naran = "F"  
naran_ = "G"  
_naran_ = "H"  
na56ra3 = "I"  
```

  Print :

```
print(naran, Naran, naRan, NARAN, n_a_r_a_n, _naran, naran_, _naran_, na56ra3) 
```

### Multi Assignment

 Iha python ita bele kria variabel barak no refere ba valor ida deit ka ita bele kria valor ida bele assign ba  multi variabel ka variabel oin-oin

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

 **Local Variabel** 

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

Global Variabel bele uza jeral ka laos iha funsaun nia laran no bele uza mos iha funsaun nia laran. Python global variabel ita bele defini iha funsaun nia laran uza global keyword.

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

Exemplu global variabel seluk:

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

Fo sai rezultadu

```
global a mak 20
```

Exemplu konaba deklara global no local variabel iha funsaun nia laran:

```
# Deklara funsaun  
def func():
    global a
    a = 20 
    h = 2  # defini lokal variabel 
    print("global", a, "no local", h)  
  
func() #bolu funsaun 
print(h) 
```

Iha kazu seluk koko print variabel h maibe mosu error tanba ita bolu variabel iha scope nia laran maibe ita print sai husi scope ka out of scope.

```
global 20 no local 2
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
<ipython-input-81-fc300bf1c91f> in <module>
      9     # bolu funsaun
     10 func()
---> 11 print(h)

NameError: name 'h' is not defined
```

### Python - Tipu Data

```
my_var = 2
```

`my_var` mak identifika ona naran husi variabel no valor mak 2 

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

