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
3. Escriba una función recursiva para calcular la operación de la potencia.
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
