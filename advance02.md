# Avance 02 de la PG02

# 1.  Definir que tipo de distribucion se va a usar

- En este ejemplo se va realizar el uso de la Distribucion Binomial

* Definir el exito "Aquellas personas que tienen menos de 1 o 0, ofreceles una tarjeta más"

entonces mi exito es encontrar aquellas personas que tienen 3 o 2 o 1 o 0 tarjetas

El exito es un criterio que se define.  En este caso mi exito va ser todas las personas no bancarizadas osea que no tienen ninguna da las tarjetas 

Entonces la probabilidad dentro de mi base de datos va ser encontrar la frecuencia con la que aparecen los ceros entre el total
P(E) = f(0)/n

por ejemplo seleccionar una variable de la base de datos :

Edad

definir el exito: personas que sea adolescentes; eso significa personas menores a 19 años

numero de visitas al cine

definiendo el exito: como aquellas personas que van 1 vez al mes 


# 2. Construir la variable aleatoria

* cualquier variable aleatoria que se distribuye como una binomial con parametros de    
     - VA ~ Bin(p, n) : se define como el numero de éxitos en n observaciones  es decir varia los exitos y n es fijo.

     Ejemplo: 

    definiendo nuestra variable aletoria:

    VA: numero de personas encuestadas que no estan bancarizadas; es decir que tienen el numero de tarjetas igual a 0 en el estudio X con 202 personas.


# 3. Identifico parametros 

sabemos que nuestra variable aleatoria se distribuye como una binomial con parametros p y n; 

    donde 

- p => P(E); es la probabilidad de exito : Exito es definido como encontrar una persona que no este bancarizada

- n => es el numero de observaciones : es el numero de personas que se encuentran en el estudio X

# 4. Construir la densidad (funcion de masa de probabilidad)

 dbinom(0:n, p, n) -> se muestra la graficas respectiva.

 # 5. Validar las propiedades de la distribucion

    - calcular la esperanza de la variable aleatoria   
    Esperanza
    E(X)
    Vrianza
    V(X)
    Coeficiente de variacion 
    CV(X)

    Estas formulas deberian coincidir

# 6. Construir un ejemplo para validar 

Por ejemplo 

CASO 1:

En una feria inmobiliaria se desaea saber la probabilidad de mas del 50% de los asistentes estén bancarizados. Se sabe que asisten 200 personas. 
Y : asistentes bancarizados
X : asistentes no bancarizados
P(Y > 100) = P(X <= 100)

X ~ Bin(p , 200) -> P(X <= 100); pbinom(100, p(E), n, lower.tail = TRUE)


