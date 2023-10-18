<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->

## Actividad: Resolver utilizando funciones en Python

### **1. Calculadora Básica:**
- Crea una función llamada calculadora que tome tres argumentos: dos números y un operador (+, -, *, /). La función debe realizar la operación indicada en los dos números y devolver el resultado.

**Ejemplo de uso:**
```python:
resultado = calculadora(5, 3, '+')  # Debe devolver 8
```

### **2. Conteo de Vocales:**
- Crea una función llamada contar_vocales que tome una cadena como argumento y devuelva el número de vocales (a, e, i, o, u) que contiene la cadena.

**Ejemplo de uso:**
```python:
num_vocales = contar_vocales("Hola, mundo!")  # Debe devolver 4
```

### **3. Primo o No Primo:**
- Escribe una función llamada es_primo que tome un número entero positivo como argumento y determine si es un número primo (es decir, solo es divisible por 1 y por sí mismo). La función debe devolver True si es primo y False si no lo es.

**Ejemplo de uso:**
```python:
resultado = es_primo(17)  # Debe devolver True
```

### **4. Contador de Palabras:**
- Escribe una función llamada contar_palabras que tome una cadena como argumento y devuelva el número de palabras en esa cadena. Supón que las palabras están separadas por espacios.

**Ejemplo de uso:**
```python:
num_palabras = contar_palabras("Hola, este es un ejemplo.")  # Debe devolver 5
```

### **5. Cálculo de Potencia:**
- Escribe una función llamada potencia que tome dos números enteros como argumentos, uno como base y otro como exponente, y devuelva el resultado de elevar la base al exponente.

**Ejemplo de uso:**
```python:
resultado = potencia(2, 3)  # Debe devolver 8 (2^3 = 2 * 2 * 2)
```

# Solución

### Ejercicio 1 (Calculadora Básica):
```python:
def calculadora(n1,n2,op):
    resultado = 0
    if op == '+':
        resultado = n1 + n2
    elif op == '-':
        resultado = n1 - n2
    elif op == '*':
        resultado = n1 * n2
    elif op == '/':
        resultado = n1 / n2
    return resultado

num1 = int(input("Ingrese el primer numero: "))
num2 = int(input("Ingrese el segundo numero: "))
op = input("Ingrese el operador: ")
x = calculadora(num1,num2,op)
print(x)

```

### Ejercicio 2 (Conteo de Vocales):
```python:
def contar_vocales(palabras):
    contador = 0
    palabras = palabras.lower()
    for vocales in palabras:
        if vocales in 'aeiou':
            contador += 1
    return contador

palabras = input("Ingrese una o más palabras: ")
resultado = contar_vocales(palabras)
print("Número de vocales:", resultado)

```

### Ejercio 3 (Primo o No Primo):
```python:
def es_primo(num):
    if num <= 1:
        return False
    elif num <= 3:
        return True
    elif num % 2 == 0:
        return False
    else:
        for i in range(3, int(num**0.5) + 1, 2):
            if num % i == 0:
                return False
        return True

numero = int(input("Ingrese un numero: "))
resultado = es_primo(numero)
if resultado:
    print(f"{numero} es primo.")
else:
    print(f"{numero} no es primo.")

```

### Ejercicio 4 (Contador de Palabras):
```python:
def contar_palabras(cadena):
    palabras = cadena.split()
    return len(palabras)

cadena = input("Ingrese una o más palabras: ")
resultado = contar_palabras(cadena)
print("Número de palabras:", resultado)

```

### Ejercicio 5 (Calculo de Potencia):
```python:
def potencia(base, exponente):
    resultado = base ** exponente
    return resultado

numBase = 2
numExponente = 3
resultado = potencia(numBase, numExponente)
print(f"{numBase} elevado a la {numExponente} es igual a {resultado}")

```