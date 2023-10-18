<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

## Actividad:
1. **Practicar con listas, tuplas, conjuntos y diccionarios en Python.**
Genera un nuevo cuaderno en Google Colab y añade cuatro bloques de código, asignándoles títulos respectivos: "Listas", "Tuplas", "Conjuntos" y "Diccionarios". A continuación, comparte el cuaderno empleando la configuración de "Acceso general - Cualquier persona con el enlace - Editor". A continuación, resuelve los ejercicios que se presentan a continuación:

### Listas
- Crea una lista que contenga los números del 1 al 10.
- Imprime la lista en el orden en que fue creada.
- Ordena la lista en orden ascendente.
- Ordena la lista en orden descendente.
- Encuentra el número más pequeño en la lista.
- Encuentra el número más grande en la lista.
- Cuenta el número de veces que aparece el número 5 en la lista.
- Elimina el número 5 de la lista.
- Agrega el número 11 a la lista.
- Imprime la lista nuevamente.

### Tuplas
- Crea una tupla que contenga las palabras "Hola", "mundo" y "Python".
- Imprime la tupla en el orden en que fue creada.
- Ordena la tupla en orden alfabético.
- Encuentra la primera palabra en la tupla.
- Encuentra la última palabra en la tupla.
- Cuenta el número de palabras en la tupla.
- Elimina la palabra "mundo" de la tupla.
- Agrega la palabra "Hola" a la tupla.
- Imprime la tupla nuevamente.

### Conjuntos
- Crea un conjunto que contenga los números del 1 al 10.
- Imprime el conjunto.
- Agrega el número 11 al conjunto.
- Elimina el número 5 del conjunto.
- Cuenta el número de elementos en el conjunto.
- Comprueba si el número 5 está en el conjunto.
- Comprueba si el número 11 está en el conjunto.
- Crea un conjunto que contenga las palabras "Hola", "mundo" y "Python".
- Imprime el conjunto.
- Comprueba si la palabra "Hola" está en el conjunto.
- Comprueba si la palabra "mundo" está en el conjunto.

### Diccionarios
- Crea un diccionario que asigne los nombres de los días de la semana a sus números correspondientes.
- Imprime el diccionario.
- Obtén el número del día de la semana "Lunes".
- Obtén el día de la semana del número 2.
- Elimina el día de la semana "Lunes" del diccionario.
- Imprime el diccionario nuevamente.

# Solución

### **Listas**
```python:
lista = [1,2,3,4,5,6,7,8,9,10]
print(lista)
lista.sort()
print(lista)
lista.reverse()
print(lista)
print(lista[9])
print(lista[0])
print(lista.count(5))
lista.remove(5)
print(lista)
lista.append(11)
print(lista)

```

### **Tuplas**
```python:
tupla = ("Hola", "Mundo", "Python")
print(tupla)
#no se puede ordenar
print(tupla[0])
print(tupla[2])
len(tupla)
print(len(tupla))
lista = list(tupla)
lista[1] = ' '
print(lista)
lista[1] = 'Hola'
tupla = tuple(lista)
print(tupla)

```

### **Conjuntos**
```python:
conjunto = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
print(conjunto)
conjunto.add(11)
print(conjunto)
conjunto.remove(5)
print(conjunto)
len(conjunto)
print(5 in conjunto)
print(11 in conjunto)
conjunto2 = {"Hola", "Mundo", "Python"}
print(conjunto2)
print("Hola" in conjunto2)
print("Mundo" in conjunto2)

```

### **Diccionarios**
```python:
diccionario = {
    'Lunes': 1,
    'Martes': 2,
    'Miercoles': 3,
    'Jueves': 4,
    'Viernes': 5,
    'Sabado': 6,
    'Domingo': 7}
print(diccionario)
print(diccionario.get('Lunes'))
del diccionario['Lunes']
print(diccionario)

```