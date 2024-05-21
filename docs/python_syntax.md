## Python - Sintase Bazika

Iha ne’e sei aprende sintase bázika ho python 3. Lian programasaun komputador kompostu husi liafuan ne'ebé define ona no bolu liafuan xave (keyword), regra ida ne'ebé preskrita kada liafuan xave mak hanaran sintase(syntax)

Python3 intérprete define ona liafuan xave iha 33, atu hatene kada liafuan xave bele hare iha lista tuir mai hahú ezekuta python.

```
~ » python                                                                                                                                  niko@Joanicos-Air
Python 3.7.2 (default, Dec  5 2020, 20:22:04) 
[Clang 12.0.0 (clang-1200.0.32.27)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

no hakerek :

```
>>> help("keywords")

Here is a list of the Python keywords.  Enter any keyword to get more help.

False               class               from                or
None                continue            global              pass
True                def                 if                  raise
and                 del                 import              return
as                  elif                in                  try
assert              else                is                  while
async               except              lambda              with
await               finally             nonlocal            yield
break               for                 not                 
>>> 
```

### Programa Python dahuluk

Ezekuta programa sira ne'ebé diferente modu programasaun.

**a. Modu Interativu Programasaun**

Modu Interativu mak command line ne'ebé fó exekuta direta ka print imediata kada deklarasaun ne'ebe la ho file script hanesan parametru ida ne'ebé hatudu iha prompt tuir mai ne'e:

```
>>> print("Hello Timor")
```

Exekuta ho python verzaun 3 uza print deklarasaun ho parentes hanesan *print ("Hello, Timor!")* nia rezultadu hanesan ne'e:

```
Hello Timor
```

**b. Programasaun Modu Script (Script Mode Programming)**

Programasaun Modu Script mak ezekusaun programa ida ne'ebé ita hakerek hanesan filé ida no fó naran ho nia estensaun *.py, no ita bele hakerek filé ne'e iha ita-nia testu editór ka vim.

Iha ezemplu ida ne'e uza vim iha terminál ubuntu nian hahú ketík iha terminál ~ nano teste.py

no hakerek skript hanesan iha ezemplu:

```
print ("Hello, Timor!")
```

hanehan iha butaun CTRL + x no hanehan enter hodi rai ita nia filé.Tuir mai ezekuta filé ne'ebé ita rai hanesan iha ezemplu

```
~ python teste.py
```

Fó-sai rezultadu hanesan tuir mai ne'e:

```
Hello, Timor!
```

Maneira seluk atu ezekuta python script ida ita halo mudansa iha file teste.py

```
!/usr/bin/python

print ("Hello, Timor!")
```

Agora koko hala'o programa ida hanesan sekuénsia hirak ne'e iha terminal.

```
~ chmod +x teste.py   # Ida ne'e atu halo file exekutabel
~ ./teste.py
```

Fó-sai rezultadu hanesan tuir mai ne'e:

```
Hello, Timor!
```

### Python Identifikador (Python Identifiers)

Python Identifikador mak naran ida ne'ebé uza hodi identifika variavel, funsaun, klase, módulu ka objetu seluk. Identifikador hahú ho letra A to'o Z ka a to'o z ka underscore ( _ ) tuir zero ka letra barak liu ho underscores no díjitu (0 to'o ba 9).

Python la autoriza karakter hanesan @, $, no % iha identifikador. Iha ne'e mak fó naran konvensaun ba Python identifikador :

- Klase naran hahú ho letra boot. Indentifikador sira seluk ho letra ki'ik.

- Identifikador ida hahú ho underscore úniku ne'ebé indika katak identifikador ne'e privadu.

- Identifikador ida hahú ho underscores rua ne'ebé indika identifikador ne'ebé privadu maka'as.

- Karik identifikador mós termina ho underscores trailing rua, identifikador ne'ebé mak define lian ho naran espesiál.

### Lina no Identasaun (Lines and Indentation)

Python la fornese iha braces hodi hatudu bloku sira kona-ba kódigu ba klase no definisaun funsaun ka kontrola movimentu( flow control ). Espasu kada liña iha klase ka funsaun iha espasu 4 ka kada tab ida. Pur ezemplu −

```
class teste():
	print("Ita nia familia")
	
class teste():
	print("Ita nia familia")
	
	def funs():
	print("hatudu ita nia funsaun")

```

### Kotasaun iha Python (Quotation in Python)

Python simu de'it quotes simples ('), dupla (") no triplu (""" ka """) quotes atu tuir string literals, bainhira tipu quote hahú no termina string.

Triplu quotes sira uza hodi span string ba iha liña oin-oin. Pur ezemplu hotu-hotu tuir mak legál.

```
liafuan = 'Liafuan'
sentence = "Ida ne'e sentense."
paragrafo = """Ida mak paragrado.""”
```

### Kometariu iha Python (Comments in Python)

Komentáriu iha Python Sinal Hash (#) iha python hatudu katak ida ne'e atu halo ka hakerek komentariu konaba ita nia script ne'ebé ita halo.

```
#!/usr/bin/python
# Komentariu Dahuluk
print ("Hello, Python!") # Komentariu Daruak
```

Fó-sai rezultadu hanesan tuir mai ne'e:

```
Hello, Python!
```

Ita bele ketik komentáriu ida iha liña ne'ebé hanesan hafoin deklarasaun ka espresaun

```
name = "Madisetti" # Ida ne'e halo komentáriu fila fali
```

Ita bele halo komentáriu barak iha liña hanesan tuir mai ne'e :

```
# Ida ne'e komentariu dahuluk.
# Ida ne'e komentariu daruak.
# Ida ne'e komentariu datoluk.
# Kometariu remata.
```

Sekuensia string ho triplu quotes bele uza hanesan komentáriu iha lina barak:

```
'''Ida ne'e mak halo komentariu iha lina oin-oinka komentariu sira ne'ebe ita hakerek barak liu bele uza triplu quotes ida ne'e'''
```



