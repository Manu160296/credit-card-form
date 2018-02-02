# RETO : "Identificación de funciones"

* **Curso:** _JS Deep: Crea tu propia libreria usando JavaScript_
* **Unidad:** _Fundamentos de JavaScript_

***

## Variables Locales :
* Tienen como scope el cuerpo de la funcion callback  de la linea 1 :
~~~
$inputCard
~~~

~~~
$inputMonth
~~~

~~~
$inputYear
~~~

~~~
$buttonNext
~~~

~~~
regexOnlyNumbers
~~~

~~~
labelErrorOrSuccessMessages
~~~

* Tiene como scope el cuerpo de la funcion `soloNumeros()`:
~~~
regex
~~~ 

* Tiene como scope el cuerpo de la funcion `isValidCreditCard(numberCard)`:
~~~
creditCardNumber 
~~~
* Tienen como scope la estructura `if` que está dentro de la funcion isValidCreditCard(numberCard)`:

~~~
arr 
~~~

~~~
sumaTotal 
~~~

## Funciones Locales : 
Se encuentran dentro de una función por lo que su scope se limita al cuerpo de la funcion en la que se encuetran ; las siguientes funciones son locales y su scope es la funcion callback de la línea 1 : 

~~~
activeButton()
~~~

~~~
desactiveButton()
~~~

~~~
longitud(input)
~~~

~~~
soloNumeros(input) 
~~~

~~~
isValidCreditCard(numberCard)
~~~

~~~
Funcion callback del evento "input"
~~~

## Funciones CallBack :
Son funciones que se pasan como argumento a otras funciones :
~~~
Linea 1  : $(document).ready(function(){...})
~~~

~~~
Línea 14 : funcion anónima  manejadora del evento input
~~~

~~~
Línea 45 : soloNumeros(longitud(numberCard))
~~~

## Funciones Statements :

~~~
activeButton()
~~~

~~~
desactiveButton()
~~~

~~~
longitud(input) 
~~~

~~~
soloNumeros(input) 
~~~

~~~
isValidCreditCard(numberCard)
~~~

## Funciones Expressions :
No se encontraron .

## Execution stack (Pila de ejecución) : 

~~~
$(document).ready(function{...})
~~~

~~~
console.log
~~~

~~~
$inputCard.on('input', function() {...});
~~~

~~~
 isValidCreditCard($(this).val().trim());
~~~

~~~
soloNumeros(longitud(numberCard))
~~~

De acuerdo a los valores `true` o `false ` se podrian ejecturar cualquiera de estas funciones :

~~~
activeButton()
~~~

~~~
desactiveButton()
~~~

## Event Queue(Cola de Eventos) :

~~~
$inputCard.on('input', function() {
    isValidCreditCard($(this).val().trim());
  });
~~~





