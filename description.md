<ul>

<li><a title="" href="#referencia-rapida-del-lenguaje-javascript">Referencia rápida del lenguaje JavaScript</a>
<ul>
<li><a title="" href="#declaracion-de-funciones">Declaración de Funciones</a></li>
<li><a title="" href="#operadores-matematicos">Operadores matemáticos</a></li>
<li><a title="" href="#operadores-logicos">Operadores lógicos</a></li>
<li><a title="" href="#comparaciones">Comparaciones</a></li>
<li><a title="" href="#alternativa-condicional">Alternativa Condicional</a></li>
<li><a title="" href="#variables">Variables</a></li>
<li><a title="" href="#repeticion-indexada">Repetición indexada</a></li>
</ul>
</li>

<li><a title="" href="#biblioteca-simplificada">Biblioteca simplificada</a>
<ul>
<li><a title="" href="#longitudunstring"><code>longitud(unString)</code></a></li>
<li><a title="" href="#convertirenmayusculaunstring"><code>convertirEnMayuscula(unString)</code></a></li>
<li><a title="" href="#comienzaconunstring-otrostring"><code>comienzaCon(unString, otroString)</code></a></li>
<li><a title="" href="#imprimirunstring"><code>imprimir(unString)</code></a></li>
<li><a title="" href="#tirardado"><code>tirarDado()</code></a></li>
<li><a title="" href="#listasiguales"><code>listasIguales</code></a></li>
<li><a title="" href="#longitudunalista"><code>longitud(unaLista)</code></a></li>
<li><a title="" href="#agregarunalista-unelemento"><code>agregar(unaLista, unElemento)</code></a></li>
<li><a title="" href="#removerunalista"><code>remover(unaLista)</code></a></li>
<li><a title="" href="#posicionunalista-unelemento"><code>posicion(unaLista, unElemento)</code></a></li>
</ul>
</li>

</ul>

<h2 id="referencia-rapida-del-lenguaje-javascript"> Referencia rápida del lenguaje JavaScript</h2>

El lenguaje JavaScript es utilizado ampliamente para construir software en todo el mundo, siendo una de las principales tecnologías de la Web. En Mumuki sólo usamos una muy pequeña parte del mismo, que listamos a continuación:

<h3 id="declaracion-de-funciones">Declaración de Funciones</h3>

> A partir de la [Lección 1: Funciones y tipos de datos](../../guides/flbulgarelli/fundamentos-javascript-funciones-tipos-de-datos)

Las funciones en JavaScript se declaran mediante la _palabra clave_ `function`, y su cuerpo va entre llaves `{` y `}`:

```javascript
function nombreDeLaFuncion(parametro1, parametro2, parametro3) {
  return ...;
}
```

Toda función debe tener al menos un retorno, que se expresa mediante `return`.

<h3 id="operadores-matematicos">Operadores matemáticos</h3>

> A partir de la [Lección 1: Funciones y tipos de datos](../../guides/flbulgarelli/fundamentos-javascript-funciones-tipos-de-datos)

```javascript
4 + 5
10 - 5
8 * 9
10 / 5
```

<h3 id="operadores-logicos">Operadores lógicos</h3>

> A partir de la [Lección 1: Funciones y tipos de datos](../../guides/flbulgarelli/fundamentos-javascript-funciones-tipos-de-datos)

```javascript
true && false
true || false
! false
```

<h3 id="comparaciones">Comparaciones</h3>

> A partir de la [Lección 1: Funciones y tipos de datos](../../guides/flbulgarelli/fundamentos-javascript-funciones-tipos-de-datos)

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


<h3 id="alternativa-condicional">Alternativa Condicional</h3>

> A partir de la [Lección 1: Funciones y tipos de datos](../../guides/flbulgarelli/fundamentos-javascript-funciones-tipos-de-datos)

Los `if`s en JavaScript encierran la condición entre paréntesis y su cuerpo entre llaves:

```javascript
if (hayPersonasEnEspera()) {
  llamarSiguientePersona();
}
```

Además, los `if`s pueden opcionalmente tener un `else`:

```javascript
if (hayPersonasEnEspera()) {
  llamarSiguientePersona();
} else {
  esperarSiguientePersona();
}
```

Por último, podemos combinar varios `if`s para tomar decisiones ante múltiples condiciones:

```javascript
if (hayPersonasEnEspera()) {
  llamarSiguientePersona();
} else if (elPuestoDebeSeguirAbierto()) {
  esperarSiguientePersona();
} else {
  cerrarPuesto();
}
```


<h3 id="variables">Variables</h3>

> A partir de la [Lección 3: Variables y procedimientos](../../guides/flbulgarelli/mumuki-guia-fundamentos-javascript-variables-y-procedimientos)

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

<h3 id="repeticion-indexada">Repetición indexada</h3>

> A partir de la [Lección 7: Recorridos](../../guides/mumukiproject/mumuki-guia-javascript-practica-de-listas-y-registros)

Las listas pueden ser _recorridas_, visitando y haciendo algo con cada uno de sus elementos. Para ello contamos con la estructura de control `for..of`, que encierra su generador
entre paréntesis (`(` y `)`) y su cuerpo entre llaves (`{` y `}`):

```javascript
let patrimoniosDeLaHumanidad = [
  {declarado: 1979, nombre: "Parque nacional Tikal", pais: "Guatemala"},
  {declarado: 1983, nombre: "Santuario histórico de Machu Picchu", pais: "Perú"}
  {declarado: 1986, nombre: "Parque nacional do Iguaçu", pais: "Brasil"},
  {declarado: 1995, nombre: "Parque nacional de Rapa Nui", pais: "Chile"},
  {declarado: 2003, nombre: "Quebrada de Humahuaca", pais: "Argentina"}
]


let cantidadPatrimoniosDeclaradosEnEsteSiglo = 0;
for (let patrimonio of patrimoniosDeLaHumanidad) {
  if (patrimonio.declarado >= 2000) {
    cantidadPatrimoniosDeclaradosEnEsteSiglo += 1;
  }
}
```


<h2 id="biblioteca-simplificada"> Biblioteca simplificada</h2>

Dentro de Mumuki usamos una biblioteca de funciones inspirada en la que ya viene con JavaScript,
pero simplifiacada para que sea más sencilla y segura de usar. A continuación listamos las principales funciones que se
pueden usar, indicando el equivalente _real_ en JavaScript cuando corresponda.

<a id="longitudunstring"></a>
### `longitud(unString)`

> A partir de la [Lección 1: Funciones y tipos de datos](../../guides/flbulgarelli/fundamentos-javascript-funciones-tipos-de-datos)
>
> Versión simplificada de [`length`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/String/length)

Uso:

```javascript
ム longitud("hola")
4
```

<a id="convertirenmayusculaunstring"></a>
### `convertirEnMayuscula(unString)`

> A partir de la [Lección 1: Funciones y tipos de datos](../../guides/flbulgarelli/fundamentos-javascript-funciones-tipos-de-datos)
>
> Versión simplificada de [`toUpperCase`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/String/toUpperCase)

Convierte un `unString` en mayúsculas:

```javascript
ム convertirEnMayuscula("hola")
"HOLA"
```

<a id="comienzaconunstring-otrostring"></a>
### `comienzaCon(unString, otroString)`

> A partir de la [Lección 1: Funciones y tipos de datos](../../guides/flbulgarelli/fundamentos-javascript-funciones-tipos-de-datos)
>
> Versión simplificada de [`startsWith`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/String/startsWith)

Dice si `unString` empieza con `otroString`:

```javascript
ム comienzaCon("aprendiendo a programar", "aprendiendo")
true

ム comienzaCon("aprendiendo a programar", "aprend")
true

ム comienzaCon("aprendiendo a programar", "programar")
false

ム comienzaCon("aprendiendo a programar", "tomar el té")
false
```

<a id="imprimirunstring"></a>
### `imprimir(unString)`

> A partir de la [Lección 3: Variables y procedimientos](../../guides/flbulgarelli/mumuki-guia-fundamentos-javascript-variables-y-procedimientos)
>
> Versión simplificada de [`console.log`](https://developer.mozilla.org/es/docs/Web/API/Console/log)

Imprime por pantalla `unString`:

```javascript
ム imprimir("¡estoy imprimiendo!")
¡estoy imprimiendo!
```

<a id="tirardado"></a>
### `tirarDado()`

> A partir de la [Lección 3: Variables y procedimientos](../../guides/flbulgarelli/mumuki-guia-fundamentos-javascript-variables-y-procedimientos)

Devuelve al azar un número entre 1 y 6:

```javascript
ム tirarDado()
5
ム tirarDado()
1
ム tirarDado()
2
```

<a id="listasiguales"></a>
### `listasIguales`

> A partir de la [Lección 5: Listas](../../guides/flbulgarelli/mumuki-guia-fundamentos-javascript-vectores)


```javascript
ム listasIguales(unaLista, otraLista)

```

<a id="longitudunalista"></a>
### `longitud(unaLista)`

> A partir de la [Lección 5: Listas](../../guides/flbulgarelli/mumuki-guia-fundamentos-javascript-vectores)
>
>  * [`length` de listas](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Array/length)

Nos dice cuan largo es `unaLista`:

```javascript
ム longitud([true, false, false, true])
4
ム longitud([5, 6, 3])
3
```

<a id="agregarunalista-unelemento"></a>
### `agregar(unaLista, unElemento)`

> A partir de la [Lección 5: Listas](../../guides/flbulgarelli/mumuki-guia-fundamentos-javascript-vectores)
>
> Versión simplificada de [`push`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Array/push)

Inserta `unElemento` al final de `unaLista`.
Este es un procedimiento que no devuelve nada pero modifica a `unaLista`:

```javascript
ム let cancionesFavoritas = ["La colina de la vida", "Zamba por vos"]
// agrega el elemento "Seminare" a la lista  cancionesFavoritas
ム agregar(cancionesFavoritas, "Seminare")
// ahora la lista tiene un elemento más:
ム cancionesFavoritas
["La colina de la vida", "Zamba por vos", "Seminare"]
```

<a id="removerunalista"></a>
### `remover(unaLista)`

> A partir de la [Lección 5: Listas](../../guides/flbulgarelli/mumuki-guia-fundamentos-javascript-vectores)
>
> Versión simplificada de [`pop`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Array/pop)

Quita el último elemento de unaLista.
Este es un procedimiento que no devuelve nada pero modifica a unaLista:

```javascript
ム let listaDeCompras = ["leche", "pan", "arroz", "aceite", "yerba"]
// removemos el último elemento
ム remove(listaDeCompras)
// la "yerba" ya no está en lista de compras
ム listaDeCompras
["leche", "pan", "arroz", "aceite"]
```

<a id="posicionunalista-unelemento"></a>
### `posicion(unaLista, unElemento)`

> A partir de la [Lección 5: Listas](../../guides/flbulgarelli/mumuki-guia-fundamentos-javascript-vectores)
>
> Versión simplificada de [`indexOf`](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Array/indexOf)

Nos dice en qué posición se encuentra `unElemento` dentro de `unaLista`.
Si el elemento no está en la lista, devuelve `-1`

```javascript
ム let premios = ["dani", "agus", "juli", "fran"]
ム posicion(premios, "dani")
0
ム posicion(premios, "juli")
2
ム posicion(premios, "feli")
-1
```
