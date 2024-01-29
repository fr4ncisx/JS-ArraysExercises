# This is the excercise from Alura (Spanish)

## Crea una lista vacía llamada "listaGenerica".

```JavaScript
let genericList = [];
```

## Crea una lista de lenguajes de programación llamada "lenguagesDeProgramacion con los siguientes elementos: 'JavaScript', 'C', 'C++', 'Kotlin' y 'Python'.

```JavaScript
let genericList = ['JavaScript', 'C', 'C++', 'Kotlin', 'Python'];
```

## Agrega a la lista "lenguagesDeProgramacion los siguientes elementos: 'Java', 'Ruby' y 'GoLang'.

```JavaScript
let genericList = ['JavaScript', 'C', 'C++', 'Kotlin', 'Python'];
```

## Crea una función que muestre en la consola todos los elementos de la lista "lenguagesDeProgramacion.

```JavaScript
function getList(){
    console.log(genericList);
}
```

## Crea una función que muestre en la consola todos los elementos de la lista "lenguagesDeProgramacion en orden inverso.

```JavaScript
function inverseList(){
    let listLength = genericList.length - 1; // As we now an Array starts with 0 so we add the length value minus 1 to our 'listLength'.
    for(let i = listLength; i >= 0 ; i--){   // We start our iterator from 'listLength' and go all the way to zero (first index)
        console.log(genericList[i]);
    }
}
```
## Crea una función que calcule el promedio de los elementos en una lista de números.

```JavaScript
const listOfNumbers = [];

function listAvg() {
  let listLength = listOfNumbers.length - 1;
  let final = 0;
  if (listOfNumbers.length != 0) {
    for (let i = listLength; i >= 0; i--) {
      final += parseInt(listOfNumbers[i]);
    }
    final = final / listOfNumbers.length;
  }
  return final;  
}
```
## Crea una función que muestre en la consola el número más grande y el número más pequeño en una lista.

```JavaScript



```

## Crea una función que devuelva la suma de todos los elementos en una lista.

## Crea una función que devuelva la posición en la lista donde se encuentra un elemento pasado como parámetro, o -1 si no existe en la lista.

## Crea una función que reciba dos listas de números del mismo tamaño y devuelva una nueva lista con la suma de los elementos uno a uno.

## Crea una función que reciba una lista de números y devuelva una nueva lista con el cuadrado de cada número.
