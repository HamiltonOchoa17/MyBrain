Son métodos para encontrar similitudes en Strings, esto de usa para encontrar formatos en i/o de Textos, su mayor uso son para encontrar formatos específicos como Emails, teléfonos, Numero de teléfono

Se puede realizar chequeo para determinar los paramentos de un código 


```python
def isPhoneNumber(text):

if len(text) != 12:
		return False
	for i in range(0, 3):
		 if not text[i].isdecimal():
			return False
	if text[3] != '-':
		return False
	for i in range(4, 7):
		if not text[i].isdecimal():
			return False
	if text[7] != '-':
		return False
	for i in range(8, 12):
		if not text[i].isdecimal():
		return False
	return True
print('415-555-4242 is a phone number:')
print(isPhoneNumber('415-555-4242'))
print('Moshi moshi is a phone number:')
print(isPhoneNumber('Moshi moshi')
```


Auque este código nos permita realizar la comparación de números telefónicos, este se queda corto cuando se le ingresas valores especifico como (123)-456-5678. Para esto se creo la  libreria [[Regexes]]