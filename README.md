# python_et_big_data

**exemple de variable**

```python
s = "bonjour"
n = 45
f = 12.36

print(s)
print(n)
print (f)
  
```
sortie
```
bonjour
45
12.36
```

**type de variable**

```python

print (type(f))
  
```
sortie
```
<type 'float'>
```
**nombre complex**

```python
z=1+8j
print (z)
print (z.real)
print (z.imag)
  
```
sortie
```
(1+8j)
1.0
8.0
```
**ultilisation module**

```python
import math
y= math.cos(2*math.pi)
print y
```
sortie
```
1.0
```
**connaitre le contenu d'un module**

```python
import math
print (dir((math)))
```
sortie
```
['__doc__', '__name__', '__package__', 'acos', 'acosh', 'asin', 'asinh', 'atan', 'atan2', 'atanh', 'ceil', 'copysign', 'cos', 'cosh', 'degrees', 'e', 'erf', 'erfc', 'exp', 'expm1', 'fabs', 'factorial', 'floor', 'fmod', 'frexp', 'fsum', 'gamma', 'hypot', 'isinf', 'isnan', 'ldexp', 'lgamma', 'log', 'log10', 'log1p', 'modf', 'pi', 'pow', 'radians', 'sin', 'sinh', 'sqrt', 'tan', 'tanh', 'trunc']

```
**de l'aide**

```python
import math
help(math)
```
sortie
```
Help on built-in module math:

NAME
    math

FILE
    (built-in)

DESCRIPTION
    This module is always available.  It provides access to the
    mathematical functions defined by the C standard.

FUNCTIONS
    acos(...)
        acos(x)
        
        Return the arc cosine (measured in radians) of x.
        .....................................
        .....................................
```

**start:stop**

```python
s=[1,2,3,4,5,6,7,8,9]
s[5]=78
print(s[2:8])
```
sortie
```
[3, 4, 5, 78, 7, 8]
```
**start:stop:step**
```python
s=[1,2,3,4,5,6,7,8,9]
s[5]=78
print(s[2:8:2])
```
sortie
```
[3, 5, 7]
```
**generer une liste avec nombre entier**
```python
a=range(1,45,2)
print a
```
sortie
```
[1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25, 27, 29, 31, 33, 35, 37, 39, 41, 43]
```
**convertir une chaine en liste**

```python
s="bonjour"
print s
en_liste=list(s)
print en_liste
```
sortie
```
bonjour
['b', 'o', 'n', 'j', 'o', 'u', 'r']
```
**Trier**

```python
a=[2,5,9,7,2,3,45,4,78]
print sorted(a)
```
sortie
```
[2, 2, 3, 4, 5, 7, 9, 45, 78]
```
#data stucture

**list**
```python
ls=[2,5,9,7,2,3,45,4,78]
print sorted(ls)
```
**tulipe**
```python
t=(2,5,9,7,2,3,45,4,78)
print sorted(t)
```
**dictionnaire**
```python
dic ={"un":1,"deux":2}
print type(dic)
print dic
```
**fonction**
```python
#definition
def fonction_add(a,b):
    """faire l'addiction de a et b"""
    return a+b

#ultilisation
print(fonction_add(4,8))
```
**class**
```python
class Personne(object):
    """un test pour une personne"""
    def __init__(self,nom,age):
        self.nom=nom
        self.age=age


    def __str__(self):

        return "(nom: %s, age: %d)" %(self.nom,self.age)
    
    def faire_addiction(self,x,y):
        return x +y

a =Personne("Marie",45)
print a
print (a.faire_addiction(8,7))
```
**exception**
```python
def divide(a,b):
    try:
        return a/b
    except Exception as e:
        print("erreur %s" % e)

divide(8.,0)
```