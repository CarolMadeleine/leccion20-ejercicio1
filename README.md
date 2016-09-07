# leccion20-ejercicio1

##Código inicial

``` javascript

var num2 = 0;
 function suma(num1) {
 	  return function(num2) {
 	  return num1 + num2;
	  }
 }
 var suma2 = suma(2);
 console.log(suma2(5)); // Debería mostrar 7 de resultado
 var suma12 = suma(12);
 console.log(suma12(76)) // Debería mostrar 88 de resultado.
}
```

##Código final

``` javascript
function suma(num1) {
 return function(num2) {
 return num1 + num2;
 }
 }
 var suma2 = suma(2);
 console.log(suma2(5)); // Debería mostrar 7 de resultado
 var suma12 = suma(12);
 console.log(suma12(76)) // Debería mostrar 88 de resultado.
}
```

##Contexto

En el ejercicio inicial se ejecuta la función anonima a pesar que la variable num2 está declarada al inicio de manera global, 
pero al no estar dentro de la función ya no es necesario que sea declarada ya que la función funciona de igual manera. 
