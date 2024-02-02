# This is the excercise Challenge Nº4 from Alura LATAM 

----------
### Crea una lista vacía llamada "listaGenerica".

```JavaScript
let listaGenerica = [];
```
----------
### Crea una lista de lenguajes de programación llamada "lenguagesDeProgramacion con los siguientes elementos: 'JavaScript', 'C', 'C++', 'Kotlin' y 'Python'.

```JavaScript
let genericList = ['JavaScript', 'C', 'C++', 'Kotlin', 'Python'];
```
----------
### Agrega a la lista "lenguagesDeProgramacion los siguientes elementos: 'Java', 'Ruby' y 'GoLang'.

```JavaScript
let genericList = ['JavaScript', 'C', 'C++', 'Kotlin', 'Python'];

function setArray(list){
    list.push('Java', 'Ruby' , 'GoLang');
    console.log(list);
}

setArray(genericList);
```
----------
### Crea una función que muestre en la consola todos los elementos de la lista "lenguagesDeProgramacion.

```JavaScript
function getList(){
    console.log(genericList);
}
```
----------
### Crea una función que muestre en la consola todos los elementos de la lista "lenguagesDeProgramacion en orden inverso.

```JavaScript
function inverseList(){
    let listLength = genericList.length - 1; // As we now an Array starts with 0 so we add the length value minus 1 to our 'listLength'.
    for(let i = listLength; i >= 0 ; i--){   // We start our iterator from 'listLength' and go all the way to zero (first index)
        console.log(genericList[i]);
    }
}
```
----------
### Crea una función que calcule el promedio de los elementos en una lista de números.

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
----------
### Crea una función que muestre en la consola el número más grande y el número más pequeño en una lista.

```JavaScript
const listOfNumbers = [10, 5, 120, 71, 38, 0, -5 , 18, 45];

function MaxMin() {
  let firstIndex = listOfNumbers[0];
  let checkMax = firstIndex;
  let checkMin = firstIndex;
  let listLength = listOfNumbers.length;

  for (let i = 1; i < listLength; i++) {
    if (listOfNumbers[i] < checkMin) {
      checkMin = listOfNumbers[i];
    }
    if (listOfNumbers[i] > checkMax) {
      checkMax = listOfNumbers[i];
    }
  }
  return `el mínimo es ${checkMin} y el máximo es ${checkMax}`;
}
```
----------
### Crea una función que devuelva la suma de todos los elementos en una lista.
```JavaScript

const numbers = [1, 5, 6, 9, 154, 34, 10];

function sum(){
    let result = 0;
    length = numbers.length - 1;
    for(let i = length ; i > 0; i--){
        result += numbers[i];
    }
    return result;
}

```
----------
### Crea una función que devuelva la posición en la lista donde se encuentra un elemento pasado como parámetro, o -1 si no existe en la lista.
```JavaScript
const numbers = [1, 5, 6, 9, 154, 34, 10];

function getPos(number) {
  let length = numbers.length;
  for (let i = 0; i < length; i++) {
    if (number === numbers[i]) {
      return i;
    }
  }
  return -1;
}

```
----------
### Crea una función que reciba dos listas de números del mismo tamaño y devuelva una nueva lista con la suma de los elementos uno a uno.
```JavaScript
const evenNumbers = [2, 4, 148, 64, 128];
const oddNumbers = [7, 15, 19, 31, 63];
let joinArray = [];

function joinList(firstArray, secondArray){
    let bothLength= firstArray.length;
    let newArray = [];
    for(let i = 0; i < bothLength; i++){
        newArray.push(firstArray[i] + secondArray[i]);
    }
    return newArray;
}

joinArray = joinList(evenNumbers, oddNumbers);

```
----------
### Crea una función que reciba una lista de números y devuelva una nueva lista con el cuadrado de cada número.
```JavaScript
const evenNumbers = [2, 4, 148, 64, 128];
let joinArray = [];

function powNumber(Array, i){
    return Math.pow(Array[i], 2);
}

function joinList(firstArray) {
  let lengthArray = firstArray.length;
  let newArray = [];  
  for (let i = 0; i < lengthArray; i++) {
    newArray.push(powNumber(firstArray, i));
  }
  return newArray;
}

joinArray = joinList(evenNumbers);
```
----------
