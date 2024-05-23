## Python List Slicing

Python iha lista bolu slicing hanesan prátika komún no dala barak uza hanesan meius ida ba programmer sira hodi rezolve problema efisiente sira. Konsidera lista python nian, nune'e atu hetan asesu ba elementu oioin iha lista ida, ita presiza ko'a lista, dalan ida atu halo ida ne'e mak uza slicing operator simples.

Iha operator ida ne'e, ida ita bele espesífika atu hahú ko'a/slice iha ne'ebé no remata iha ne'ebé no mós espasu hakat dala hira, no ikus liu sei fó sai rezultadu iha lista ne'ebé eziste ona.

### Syntax:

```
Lst [Initial:End:IndexJump]
```

Karik List iha leten maka espresaun iha leten sei ezekuta parte husi lista index hahú no remata no espasu ka hakat medida indexJump.

### Indexing

**1. Positive Indexes**

```
# Hahu ho lista
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
# copy sai lista ka fo sai lista
print(List[::])

Fó sai rezultadu
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

**2. Negative Indexes**

```
# INDEX
# post = [ 0| 1 | 2 | 3 | 4 | 5]
# Nega = [-5|-4 |-3 |-2 | -1]

# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
# Fó sai lista ho negativu
print(List[-10::1])
```
Fó sai rezultadu
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]


**3. Slicing**

```
# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
print(List[1:5]) # 1 reprezenta index hahu no 5 reprezenta index remata no rezultadu hatudu katak [1, 2, 3, 4] sei foti deit valór antes index 5 ba kotuk
```
F sai rezultadu 
[1, 2, 3, 4]


```
# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# Fó sai rezultadu hanesan range 
print(List[3:9:2]) # 3 reprezenta index hahu to remata 9 no 2 step
```
Fosai rezultadu 
[3, 5, 7]


```
# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# Fó sai rezultadu hanesan range
print(List[::]) # :: reprezenta index hahú no index remata ka fó sai lista tomak la slice

```
Fó sai rezultadu
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

```
# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# Fó sai rezultadu hanesan range
print(List[::2]) # :: reprezenta index hahu no remata no 2 etapa
```

Fó sai rezultadu
[0, 2, 4, 6, 8]

```
# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# reverze lista husi 0 ba 9
print(List[::-1])
# reverse lista no fo hakat ka etapa 3
print(List[::-3])
 
print(List[:1:-2])
```
Fó sai rezultadu

[9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
[9, 6, 3, 0]
[9, 7, 5, 3]

```
# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# Ida nee fo sai rezultadu ho lista mamuk tanba hahu ho index sanulu maibe iha lista la too sanulu no step 2 la iha rezultadu tanba la iha falor nebe hakat liu index sanulu 
# karik bele kria ezemplu seluk hanesan print(List[4::2]) sei fo sai rezultadu [4, 6, 8]
print(List[10::2])
 
# Iha list slicing index hahu to remata ita la bele fo hanesan iha exemplu kraik nee nia sei la bele fo rezultadu.
# Karik atu fo sai rezultadu iha index hahu no remata la bele hanesan print(List[1:4:1]) sei fo sai rezultadu [1, 2, 3]
print(List[1:1:1])
 
# Iha list slicing index negative mos hanesan hahu to remata ita la bele fo hanesan iha exemplu kraik nee nia sei la bele fo rezultadu.
# Karik atu fo sai rezultadu iha index hahu no remata la bele hanesan print(List[-1:-4:-1]) sei fo sai rezultadu [9, 8, 7]
print(List[-1:-1:-1])
 
# Iha slice mos ita labele fo valor remata to zero
print(List[:0:])
```

Fosai rezultadu
[]
[]
[]
[]

```
# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# Fó sai rezultadu hahú husi index 4 too remata no hakat espasu 2
print(List[1:3])

# Fó sai rezultadu hahú husi index 1 too remata 4 no hakat espasu 2
print(List[1:4:1])

# Fó sai rezultadu reverse no remata iha index 4 no hakat espasu ida
print(List[-1:-4:-1]) 
```
Fó sai rezultadu
[1, 2]
[1, 2, 3]
[9, 8, 7]

```
colors = ['red', 'green', 'blue', 'orange']
print(colors[1:3])
```

Fó sai rezultadu
['green', 'blue']

**4. Assign data**|

```
# Hahu ho lista 
List = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
# Fo sai lista 
print(List[::])
```

Fó sai rezultadu
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

```
# assign valor ba array nia laran
List[4:6] = [10, 11]
print(List)
```
Fó sai rezultadu
[0, 1, 2, 3, 10, 11, 6, 7, 8, 9]

**5. Slice String**

```
b = "Hello, World!"
print(b[2:5])
```
Fó sai rezultadu
llo

```
print(b[-1::-1])
```

Fó sai rezultadu
!dlroW ,olleH

```
print(b[:5])
```

Fó sai rezultadu
Hello

```
print(b[-5:-2])
```

Fó sai rezultadu
orl

**6. Python slice() Function**

```
b = "Hello, World!"
s = slice(5) # sei foti letra 4 antes index 5 ba kotuk
print(b[s])
```

Fó sai rezultadu
Hello

```
b = "Hello, World!"
s = slice(3, 6) # sei foti letra hahu husi index 3 too antes index 6 ba kotuk
print(b[s])
```
Fó sai rezultadu
lo,

```
b = "Hello, World!"
s = slice(3, 10, 2) # sei foti letra hahu husi index 3 too antes index 10 ba kotuk no fo sai deit letra husi espasu 2
print(b[s])
```

Fó sai rezultadu
`l,Wr`
