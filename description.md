# Referencia rápida del lenguaje JavaScript

El lenguaje JavaScript es utilizado ampliamente para construir software en todo el mundo, siento una de las principales tecnologías de la Web. En Mumuki sólo usamos una muy pequeña parte del mismo, que listamos a continuación:

## Declaración de Funciones

> A partir de la [Lección 1: Funciones y tipos de datos]()

Las funciones en JavaScript se declaran mediante la _palabra clave_ `function`, y su cuerpo va entre llaves `{` y `}`:

```javascript
function nombreDeLaFuncion(parametro1, parametro2, parametro3) {
  return ...;
}
```

Toda función debe tener al menos un retorno, que se expresa mediante `return`.

## Operadores matemáticos

> A partir de la [Lección 1: Funciones y tipos de datos]()

```javascript
4 + 5
10 - 5
8 * 9
10 / 5
```

## Operadores lógicos

> A partir de la [Lección 1: Funciones y tipos de datos]()

```javascript
true && false
true || false
! false
```

## Comparaciones

> A partir de la [Lección 1: Funciones y tipos de datos]()

```javascript
// para cualquier tipo de dato
"hola" === "hola"
"hola" !== "chau"

// para números
4 >= 5
4 > 5
4 <= 5
4 < 5
```


## Variables

> A partir de la [Lección 2: Variables y procedimientos]()

Las variables nos permiten _recordar_ valores y se declaran mediante la palabra reservada `let` y se les da un valor inicial usando `=`:

```javascript
let pesosEnMiBilletera = 100;
let diasQueFaltanParaElVerano = 10;
```

La mismas se asignan mediante `=`:

```javascript
pesosEnMiBilletera = 65;
diasQueFaltanParaElVerano = 7;
```

En ocasiones las asignaremos usando el valor anterior:

```javascript
pesosEnMiBilletera = pesosEnMiBilletera * 2;
diasQueFaltanParaElVerano = diasQueFaltanParaElVerano - 1;
```

La asignación anterior se puede compactar combinando el signo `=` y la operación:

```javascript
pesosEnMiBilletera *= 2;
diasQueFaltanParaElVerano -= 1;
```


# Biblioteca simplificada

Dentro de Mumuki usamos una biblioteca de funciones inspirada en la que ya viene con JavaScript,
pero simplifiacada para que sea más sencilla y segura de usar. A continuación listamos las principales funciones que se
pueden usar, indicando el equivalente _real_ en JavaScript cuando corresponda.

## `absoluto`

> Versión simplificada de []()

Uso:

```javascript
absoluto(unNumero)
```

Ejemplo:

```javascript
ム absoluto(unNumero)

```

## `agregar`

> Versión simplificada de []()

Uso:

```javascript
agregar(unaLista, unElemento)
```

Ejemplo:

```javascript
ム agregar(unaLista, unElemento)

```

## `anio`

> Versión simplificada de []()

Uso:

```javascript
anio(unStringFecha)
```

Ejemplo:

```javascript
ム anio(unStringFecha)

```


## `listasIguales`

> Versión simplificada de []()

Uso:

```javascript
listasIguales(unaLista, otraLista)
```

Ejemplo:

```javascript
ム listasIguales(unaLista, otraLista)

```

## `arraysIguales`

> Versión simplificada de []()

Uso:

```javascript
arraysIguales(unaLista, otraLista)
```

Ejemplo:

```javascript
ム arraysIguales(unaLista, otraLista)

```


## `comienzaCon`

> Versión simplificada de []()

Uso:

```javascript
comienzaCon(unString, otroString)
```

Ejemplo:

```javascript
ム comienzaCon(unString, otroString)

```





## `convertirEmMayuscula`

> Versión simplificada de []()

Uso:

```javascript
convertirEmMayuscula(x)
```

## `esMultiploDe`

> Versión simplificada de []()

Uso:

```javascript
esMultiploDe(unNumero, esteOtro)
```

## `imprimir`

> Versión simplificada de []()

Uso:

```javascript
imprimir(s)
```

## `longitud`

> Versión simplificada de []()

Uso:

```javascript
longitud(lista)
```

## `minimo`

> Versión simplificada de []()

Uso:

```javascript
minimo(numeros)
```

## `maximo`

> Versión simplificada de []()

Uso:

```javascript
maximo(numeros)
```


## `poner`

> Versión simplificada de []()

Uso:

```javascript
poner(a, e) / insert
```


## `posicion`

> Versión simplificada de []()

Uso:

```javascript
posicion(lista, elemento)
```

## `remover`

> Versión simplificada de []()

Uso:

```javascript
remover(lista)
```

## `productoria`

> Versión simplificada de []()

Uso:

```javascript
productoria(array)
```

## `promedio`

> Versión simplificada de []()

Uso:

```javascript
promedio(listaDeNumeros)
```

## `rango`

> Versión simplificada de []()

Uso:

```javascript
rango(s, e)
```


## `siguiente`

> Versión simplificada de []()

Uso:

```javascript
siguiente(x)
```

## `sumatoria`

> Versión simplificada de []()

Uso:

```javascript
sumatoria(array)
```

## `anterior`

> Versión simplificada de []()

Uso:

```javascript
anterior(x)
```


## `tirarDado`

> Versión simplificada de []()

Uso:

```javascript
tirarDado()
```

