Control de flujo
================

Introduccion
------------

Las estricturas de control nos sirven para tomar desiciones en el codigo
y ejecutar un bloque de codigo dependiendo del cumplimiento o no de alguna condicion


if (si condicional)
------------------

Esta es la estructura de control mas basica 

```javascript
if(condicion){
    // Codigo a ejecutar si la condicion es verdadera
}
```

En el ejemplo superior el codigo dentro del bloque se ejecutara si la condicion
se evalua a un boleano con valor verdadero **(true)**

if (si condicional) else (en caso contrario)
---------------------------------------------
Despues de la condicion if podemos colocar un else con otro bloque de codigo
para ejecutar en caso de que la condicion no se cumpla

```javascript
if(condicion){
    // Ejecutar este bloque de codigo si es verdadera la condicion
} else {
    // Ejecutar este otro bloque si no
}
```

else if
-------

```javascript
if(condicion){
    // Ejecutar si la condicion es 
} else if(condicion2){
    // Este codigo se ejecuta si la primera condicion es falsa y la segunda verdadera
}
```

switch case
-----------

```javascript
var nombre = 'Franchesca'
switch(nombre){
    case 'Jorge': console.log('Hola Jorge');
        break;
    case 'Yolanda': console.log('Hola Yolanda');
        break;
    case 'Zadday': console.log('Hola Zadday');
        break;
    case 'Franchesca': console.log('Hola Franche');
        break;
    case 'Barbara': console.log('Hola Barbara');
        break;
    default: console.log('Hola desconocido');
}
```

Operador Ternario
-----------------
```javascript

var edad = 12;
var  edadEscolar = edad < 22 ? 'Si esta en edad escolar' : 'No esta en edad escolar';
console.log(edadEscolar);
```
Es equivalente a ->
```javascript
if(edad < 22){
    edadEscolar = 'Si esta en edad escolar';
    
} else {
    edadEscolar = 'No esta en edad escolar';
}
```

Falsy & Truly values
--------------------

Existen varios valores que ese evaluan como verdadero o falso sin ser extrictamente los valores boleaos 'true' y 'false'.

Los siguientes valores seran tomados como verdaderos en una condicioiom
1. Numero diferente de cero (1)
2. Un objeto ({})
3. Un array ([])
4. Un string no vacio ('a')
5. el boleano true (obviamente)

Los siguientes valores son evaluados como false
1. 0
2. ''
3. null
4. undefined
5. false

if('yolanda'){
    // Este codigo se ejecuta porque el string se evalua como 'true'
}


if(''){ 
    // Este codigo no se ejecuta porqe un string vacio se evalua como 'false'
}