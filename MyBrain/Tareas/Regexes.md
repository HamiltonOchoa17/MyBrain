Las expresiones regulares, llamadas expresiones regulares para abreviar, son descripciones de un patrón de texto. Por ejemplo, \d en una expresión regular representa un carácter de dígito. 

para esto se tiene que importa la librería re

```python
import re
```

se crea un objeto de la librería re con la función .compile() esto facilita el uso de otros métodos le la librería 

```python
phoneNumRegex = re.compile(r'\d\d\d-\d\d\d-\d\d\d\d')
mo = phoneNumRegex.search('My number is 415-555-4242.')
print('Phone number found: ' + mo.group())
	Phone number found: 415-555-4242

```


Se le da un formato el objeto phoneNumRegex donde \d indica que es un decimal






