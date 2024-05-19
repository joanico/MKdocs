###Python Mutable no Immutable

Koseitu set mutable mak ita bele muda objetu sira iha lista no dictionary nia laran 

```
>>> mutable_obj = ['a', 'b', 'c', 'd'] # Mutable list
>>> mutable_obj[1] = 'e' # Troka objetu iha indese 1 ba e
>>> print(mutable_obj)
['a', 'e', 'c', 'd']

>>> mutable_obj = {'a': 1, 'b': 2, 'c': 3} # Mutable dictionary
>>> mutable_obj['a'] = 'e' # Troka valor objetu iha indese key 1 ba e
>>> print(mutable_obj)
{'a': 'e', 'b': 2, 'c': 3}
>>> mutable_obj.keys()
dict_keys(['a', 'b', 'c'])

>>> mutable_obj.values()
dict_values(['e', 2, 3])
```

 Koseitu set immutable mak ita bele muda objetu sira iha number, string no tuple nia laran 

```
>>> immutable_obj = ('a', 'b', 'c', 'd') # Immuatable tuple
>>> immutable_obj[1] = 'e'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object does not support item assignment

'tuple' object does not support item assignment


>>> immutable_obj = 'a' # Immuatable string
>>> immutable_obj['a'] = 'e'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'str' object does not support item assignment

'str' object does not support item assignment

```

