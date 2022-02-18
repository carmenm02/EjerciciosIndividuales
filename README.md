# EjerciciosIndividuales
A continuación encontrará los 4 ejercicios sobre la algorítmica propuestos.
# Ejercicio 8
1-Algoritmo precio con IVA

#Calculamos el precio final

Entrada
 coste: REAL 
 impuesto: REAL 
 
Resultado: REAL #precio final

Precondición
 c ≥ 0
 impuesto sobre venta > 0
 
Realización
 Resultado <-- c + (c x i)

Poscondición
 Resultado = c + (c x i)
 
fin cálculo 

2-Algoritmo interés generado

#Vamos a calcular el interés generado con un capital inicial, tiempo e interés dado.

Entrada
 c: REAL #importe del capital inicial
 t: REAL #tiempo expresado en meses
 i: REAL #tasa de interés

Resultado: REAL

Precondición
 c ≥ 0
 t > 0
 i > 0
 
Realización
 Resultado <-- c x t x i
 
Poscondición
 Resultado = c x t x i

fin calculo interés generado


# Ejercicio 9
1-Algoritmo media arimética

#vamos a calcular un algoritmo que calcule la media aritmética de tres números dados

Entrada
 n1, n2, n3: REAL #los números con los que se obtendrá la media
 
Precondición
 n1, n2, n3 ≥ 0

Realización
 Resultado <-- (n1 + n2 + n3) / 3
 
Poscondición
 Resultado = (n1 + n2 + n3) / 3
 
fin cálculo media aritmética
2-Algoritmo media aritmética

#vamos a calcular un algoritmo que calcule la media aritmética de distintos números con diversos coeficientes de ponderación.

Entrada

 n1, n2, n3.....nk: REAL #los números con los que se obtendrá la media aritmética

 k: REAL #media aritmética de las notas

 c1, c2, c3....ck: REAL #coeficientes de poderación

Precondición
 
 n1, n2, n3...nk ≥ 0
 
 k ≥ 1 #la cantidad total de notas no puede ser igual a 0
 
 c1, c2, c3 ...ck ≥ 0
 
 Realización
  Resultado <-- Σ(nxc) / k
  
 Poscondición
  Resultado <-- Σ(nxc) / k
  
 fin cálculo media arirmética
 # Ejercicio 10
  Algoritmo área triángulo

#vamos a calcular el área del tríangulo dado un lado y la altura relativa a este.

Entrada
 l:REAL #lado triángulo (el cual ejerce como base)
 h: REAL #altura relativa al lado dado
 
Precondición
 l > 0
 h > 0

Realización
 Resultado <-- (l x h) / 2
 
Poscondición
 Resultado = (l x h) / 2
 
fin calcular área triángulo
 
# Ejercicio 11
 Algoritmo horas_extra   
  #Establece la remuneración de `horas_ext' adicionales para     
  #un salario mensual bruto de `salario_mensual_bruto'.  
  
 Entrada    
  salario_mensual_bruto : REAL        
    #Importe del salario mensual bruto   
  horas_ext : ENTERO        
    #Cantidad de horas extra del mes a pagar
    
 precondición 
  salario_mensual_bruto > 0    
  horas_ext ≥ 0

constante
  CANTIDAD_SEMANAS : ENTERO ← 52       
    #Cantidad de semanas de trabajo 
  CANTIDAD_HORAS_SEMANA : ENTERO ← 35      
    #Cantidad legal de horas de trabajo semanales 
  CANTIDAD_HORAS_MAX_1 : ENTERO ← 8      
    #Umbral de cambio de precio de remuneración
  PRECIO_1 : REAL ← 1,25     
    #Tarifa de remuneración de CANTIDAD_HORAS_MAX_1 primeras   
    #horas extra    
  PRECIO_2 : REAL ← 1,50      
    #Tarifa de remuneración de las otras horas extra
    
 variable
  horas_ext_1 : ENTERO    
    #Cantidad de horas extra con PRECIO_1 %
  horas_ext_2 : ENTERO    
    #Cantidad de horas extra con PRECIO_2 %  
  precio_hora : REAL
    #Precio hora de la remuneración bruta básica
    
 realización
    calcular el precio_hora de la remuneración bruta básica 
    
    Resultado ← precio_hora x    
             (               
                inf(horas_ext, CANTIDAD_HORAS_MAX_1) x PRECIO_1              
             +               
                sup(horas_ext – CANTIDAD_HORAS_MAX_1, 0) x PRECIO_2             
              )
 postcondición
 ...
 fin horas_extra

# Ejercicio 12

Algoritmo abrir
    # Inicializar `c' mediante un `saldo_inicial' y un     
    # `descubierto_MAX' durante una `duración_max'.

Entrada
  c : CUENTA
  saldo_inicial : REAL
  descubierto_MAX : REAL
  duración_max : FECHA
 
Precondición
  saldo_inicial > 0
  descubierto_MAX ≥ 0
  duración_max ≥ 0

realización
  c.descubierto ← descubierto_MAX
  c.saldo ← saldo_inicial
  c.fecha_descubierto ← 0
  c.duración_max ← duración_max
 
 postcondición
  c.descubierto = descubierto_MAX 
  c.saldo = saldo_inicial
  c.duración_max = duración_max
  c.fecha_descubierto = 0
fin abrir
