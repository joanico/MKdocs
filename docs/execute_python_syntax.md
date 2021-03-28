## Python - Sintase Bazika

Iha ne’e sei aprende sintase bazika ho python3.Lian programasaun komputer kompostu husi liafuan ne’ebe defini ona no bolu liafuan-xavi (keyword), regra ida nebe preskrita kada liafuan-savi mak hanaran sintase(syntax)

Python3 interprete defini ona liafuan-xavi iha 33, atu hatene kada liafuan-xavi bele hare iha lista tuir mai hahu exekuta python.

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

Ezekuta programa sira ne'ebe diferente modu programasaun.

**a. Modu Interativu Programasaun**

Modu Interativu mak command line ne'ebé fó exekuta direta ka print imediata kada deklarasaun ne'ebe la ho file script hanesan parametru ida ne'ebe hatudu iha prompt tuir mai ne'e:

```
>>> print("Hello Timor")
```

Exekuta ho python verzaun 3 uza print deklarasaun ho parentes hanesan *print ("Hello, Timor!")* nia rezultadu hanesan ne'e:

```
Hello Timor
```

**b. Programasaun Modu Script (Script Mode Programming)**

Programasaun Modu Script mak ezukusaun programa ida nebe ita hakerek hanesan file ida no fo naran ho nia extensaun *.py, no ita bele hakerek file ne'e iha ita nia text editor ka vim.

Iha ezemplu ida ne'e uza vim iha terminal ubuntu nian hahu ketik iha terminal ~ nano teste.py

no hakerek script hanesan iha ezemplu:

```
print ("Hello, Timor!")
```

hanehan iha butaun CTRL + x no hanehan enter hodi rai ita nia file.Tuir mai exekuta file nebe ita rai hanesan iha exemplu

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

Python Identifikador mak naran ida ne'ebé uza hodi identifika variável, funsaun, klase, module ka objetu seluk. Identifikador hahú ho letra A to'o Z ka a to'o z ka underscore ( _ ) tuir zero ka letra barak liu ho underscores no díjitu (0 to'o ba 9).

Python la autoriza karakter hanesan @, $, no % iha identifikador. Iha neʼe mak fó naran konvensaun ba Python identifikador :

- Klase naran hahu ho letra boot. Indentifikador sira seluk ho letra kiik.

- Identifikador ida hahu ho underscore uniku ne'ebé indika katak identifikador ne'e privadu.

- Identifikador ida hahu ho underscores rua ne'ebé indika identifikador ne'ebé privadu maka'as.

- Karik identifikador mos termina ho underscores trailing rua, identifikador ne ' ebé mak defini lian ho naran espesiál.

### Lina no Identasaun (Lines and Indentation)

Python la fornese iha braces hodi hatudu bloku sira kona-ba kódigu ba klase no definisaun funsaun ka kontrola movimentu( flow control ). Espasu kada lina iha klase ka funsaun iha espasu 4 ka kada tab ida. Pur ezemplu −

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

Komentáriu iha PythonSinal Hash (#) iha python hatudu katak ida ne'e atu halo ka hakerek komentariu konaba ita nia script nebe ita halo.

```
#!/usr/bin/python
# Komentariu Dahuluk
print ("Hello, Python!") # Komentariu Daruak
```

Fó-sai rezultadu hanesan tuir mai ne'e:

```
Hello, Python!
```

Ita bele ketik komentáriu ida iha liña ne'ebe hanesan hafoin deklarasaun ka expresaun

```
name = "Madisetti" # Ida ne'e halo komentariu fila fali
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



