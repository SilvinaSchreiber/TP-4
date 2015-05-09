Respuestas TP-4
====================
####1) 
* La expresión `for` de la función `main` itera hasta que c es igual a EOF(*señal que informa que no puso seguir leyendo*).
* La coma es un operador, que no es conmutativa por el orden de evaluación.
* Otra expresión equivalente es el `ml=mc=0`.

####2) 
* Son necesarios los paréntesis porque es una función int devuelve el carácter que se halle en la entrada estándar.
* Si no los usamos el programa detecta un error en la pragmática del programa y da un warning. Sin los paréntesis no se puede ingresar nada por teclado.

####3) 
* Evalúa `feof(stdin)` y lo niega, su es verdadero llama a `perror` e invoca el argumento "ERROR!"

####4) 
* La función perror transforma el número de error en la expresión entera de errno a un mensaje de error. Escribe una secuencia de caracteres al stream estándar de errores.

####5) 
* La expresiones equivalente es `ferror`. Esta sirve para determinar si el flujo está en un estado de error.
* Las expresiones no son mutuamente excluyentes.
* La pragmática de este programa es determinar si hubo un error o no.

####6) 
* En el formato `%.1f`:
  - `%` indica que comienza una especificación de conversión.
  - `.1` indica que se va a imprimir 1 caracter después del punto decimal.
  - `f` indica que se escribirá un numero de punto flotante.

####7) 
* Porque el resultado que se muestra en el `printf`es un float. Se castea para mayor precisión y se cambia el tipo de dato.

####10) 
* Este programa no funciona para el caso vacio. Problema en la división por 0.

####11)
* La expresión que calcula el promedio no es precisa, ya que cuenta los `'\n'` 

####12)
* Lo que debemos hacer es: 

<pre><code>for(nl = 0, nc = 0; ( c = getchar()) != EOF;)                                
  if(c == '\n')                                                                
    ++nl;                                                                                    
  else                                                                         
    ++nc; 
</code></pre>
