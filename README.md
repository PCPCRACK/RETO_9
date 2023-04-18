# RETO_9
1. De los retos anteriores seleciones 3 funciones y escribalas en forma de lambdas.

1.1 

```python
if __name__ == "__main__":
    N = float(input("N° de gallinas? "))#pregunta cuantos de cada uno
    M = float(input("N° de gallos? "))
    K = float(input("N° de pollitos? "))
    suma = (lambda N,M,K:(N*6)+(M*7)+(K*1))(N,M,K) #multiplica y suma todo
    print("La cantidad de carne de aves en kilos es ",suma) #imprime el resultado
```
1.2
```python
if __name__ == "__main__":
    P = float(input("N° de Panes? ")) #pregunta cuantos de cada uno
    M = float(input("N° de Bolsas de leche? "))
    H = float(input("N° de Huevos ? "))
    B = float(input("Valor billete "))
    suma = (lambda P,M,H,B: B-((P*300)+(M*3300)+(H*350)))(P,M,H,B) #multiplica y suma y luego resta el billete
    if suma>0: #si suma es mayor a cero
        print("Las vueltas son ",suma)
    else :
        print("Quedaste debiendo ",suma)
```
1.3
```python
if __name__ == "__main__":
    a = float(input("Prestamo inicial "))
    b = float(input("Tasa de interes "))
    c = float(input("Tiempo en meses "))
    valor_final = (lambda a,b,c: a*((1 + b/12)**c))(a,b,c)
    print("El valor final del préstamo es: ", valor_final)
```

2. De los retos anteriores seleciones 3 funciones y escribalas con argumentos no definidos (*args).

2.1
```python
#una función que calcule la cantidad de carne de aves en kilos 

def suma(*arg):
    for nums in arg:
         suma = (arg[0]*6)+(arg[1]*7)+(arg[2]*1)#multiplica y suma todo
    return suma 
    

if __name__ == "__main__":
    N = float(input("N° de gallinas? "))#pregunta cuantos de cada uno
    M = float(input("N° de gallos? "))
    K = float(input("N° de pollitos? "))
    print("La cantidad de carne de aves en kilos es ",(suma(N,M,K)))
```
2.2
```python
#Una función matemática para calcular el volumen y el área superficial
from math import sqrt #se importa de  las librerias la raiz cuadrada y pi
from math import pi

def cirVandAr(*arg):
    V = (4/3)*pi*(arg[0])**3 
    A = 4*pi*((arg[0])*2)**2
    return V,A

def ConoVandAr(*arg):
    V = 1/3*(arg[1])*pi*(arg[0])**2
    g = sqrt(((arg[0])**2)+((arg[1])**2))
    A = pi*(arg[0])*(g+(arg[0]))
    return V,A

if __name__ == "__main__":
    a = float(input("Radio esfera "))#se pide el radio de la esfera
    b = float(input("Radio cono "))#se pide el radio del cono
    c = float(input("Altura cono "))#se pide la altura del cono
    print("El volumen en cm3 y Area de la esfera en cm2 es ",(cirVandAr(a)))
    print("El volumen en cm3 y Area del cono en cm2 es ",(ConoVandAr(b,c)))
```
2.3
```python
#Hacer un programa que me diga las vueltas (o lo que quedo debiendo)

def suma(*arg):
    return (arg[3])-(((arg[0])*300)+((arg[1])*3300)+((arg[2])*350)) #multiplica y suma y luego resta el billete
    

if __name__ == "__main__":
    P = float(input("N° de Panes? ")) #pregunta cuantos de cada uno
    M = float(input("N° de Bolsas de leche? "))
    H = float(input("N° de Huevos ? "))
    B = float(input("Valor billete "))
    suma = suma(P,M,H,B) #llama la funcion
    if suma>0: #si suma es mayor a cero
        print("Las vueltas son ",suma)
    else :
        print("Quedaste debiendo ",suma)
```
3. Escriba una función recursiva para calcular la operación de la potencia.
```python
def PotenciaRecursivo(n : int,p : int)-> int:
  print(n,p)
  if p == 0: #si p es igual a 0 retorna 1
    return 1
  else:
    # Condicion de la funcion recursiva
    return n*PotenciaRecursivo(n,p-1) 


if __name__ == "__main__":
    num = int(input("Ingrese numero: ")) #pide valores enteros
    p = int(input("potencia: "))
    PotenciaDeNum = PotenciaRecursivo(num,p) #llama la funcion
    print(str(num) + " elevado a " + str(p) + " es "+ str(PotenciaDeNum)) #imprime
```
4. Utilice la siguiente plantilla de code para contar el tiempo:
```python
import time
start_time = time.time()
# instrucciones sobre las cuales se quiere medir tiempo de ejecución
end_time = time.time()
timer = end_time - start_time
print(timer)
```

Realice pruebas para calcular fibonacci con iteración o con recursión. Determine desde que número de la serie la diferencia de tiempo se vuelve significativa.
**Importante:** Revisar este [hilo](https://stackoverflow.com/questions/8220801/how-to-use-timeit-module).

5. Crear cuenta en [stackoverflow](https://stackoverflow.com/) y adjuntar imagen en el repo

6. Cosas de adultos....ir a [linkedin](https://www.linkedin.com/) y crear perfil....NO IMPORTA que estén iniciando, si tienen tiempo para redes poco útiles como fb, insta, o tiktok tienen tiempo para crear un perfil mamalon. Dejar enlace en el repo.
