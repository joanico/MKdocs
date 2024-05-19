##**Python - Variabel**

**Saida mak Variabel ?**

Variabel mak fatin memoria rezerva ida hodi rai valor sira. Signifika katak bainhira ita kria variabel ida ita rezerva hela fatin mamu iha memoria, valor sira nebe ita rai bele ho tipu data interger ka karakteristika sira.

### Deklara variabel

Atu deklara variabel iha python partikularmente ita indentifika `Naran` no `Valor`

`Naran` mak hodi identifika  variabel

`Valor` bele identifika depois operador (=)  

  Por exemple:

  ```
  a = 1
  ```

![var](https://i.postimg.cc/KYvB4scS/Screen-Shot-2021-03-10-at-6-10-06-PM.png)

Notas: a mak identifika ona naran husi variabel no valor mak 1 

### Naran Variabel

Python naran variabel bele refere ba kualker naran husi variabel bele hakerek ho letra maiskula ka minuskula no bele hakerek digital husi 0 to’o 9 no uza simbolu sira hanesan underscore(__)

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

Iha python bele kria variabel barak no refere ba valor ida deit ka ita bele kria valor ida bele assign ba multipla variabel ka variabel oin-oin.

  Exemplu:

Assign valor ida ba multipla variabel ka bele kria multipla variabel fo valor ida edit.

  ```
  a = b = c = 10
  
  print(a)
  print(b)
  print(c)
  ```

Assign multipla valor ba multipla variabel 

  ```
  x, y, z = 10, 15, "hello"
  
  print (x)
  print (y)
  print (z)
  ```

### Tipu Variabel

Tipu python variabel iha rua local variabel no global variabel.

**Local Variabel**

Local variabel mak defini iha funsaun nia laran no iha local scope.

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

Global Variabel bele uza jeral ka laos iha funsaun nia laran ka global scope no bele uza mos iha funsaun nia laran ka local scope maybe tenki uza global keyword. 

  Exemplu:

  ```
  a = 20 # Global variabel
  # Deklara funsaun  
  def func():  
      print("global a mak", a)  
      # bolu funsaun
  func()
  ```

  Fo sai rezultadu

  ```
global a mak 20
  ```

Exemplu global variabel iha funsaun nia laran uza global keyword:

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
  
func() # bolu funsaun 
```
