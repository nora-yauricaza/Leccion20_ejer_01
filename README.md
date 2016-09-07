## Leccion20_ejer_01

Nota: Solo modificar una línea para que se obtenga el resultado deseado.

var num2 = 0;

function suma(num1) {

	  return function() {
	  
		  return num1 + num2;
		  
	  }
	  
} 
var suma2 = suma(2);

console.log(suma2(5)); // Debería mostrar 7 de resultado

var suma12 = suma(12);

console.log(suma12(76)) // Debería mostrar 88 de resultado.


Cuando ejecutamos solo el ejecuta 2 y 12, porque faltaba ingresar el parámetro num2


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

La solucion fue ingresar el parametro num2.

return function(num2), para que sumen num1 + num2 y el resutado es: 7 y 88.
