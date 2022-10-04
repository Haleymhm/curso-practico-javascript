# Test de JavaScript

¡Es hora de poner a prueba cuánto sabes sobre JavaScript!

Esta lectura es una prueba de JavaScript. A diferencia de un examen, nadie te obligará a nada. **Puedes hacer trampa y saltar a la siguiente clase**, ese es el camino fácil. Pero tengo mucha fe en ti, confío en que seguirás mis consejos y no avanzarás a la siguiente clase hasta superar esta prueba.

## Instrucciones para tomar esta prueba

- Evalúa muy críticamente tu conocimiento.
- Si logras resolver la prueba, no importa cuánto te cueste, puedo asegurarte que tienes todo para continuar a las siguientes clases y tomar el resto del curso.
- Si no lo logras, no te preocupes, absolutamente nadie puede juzgarte, solo tú. Vuelve al [Curso Básico de JavaScript](https://platzi.com/cursos/basico-javascript/), anota los temas clave donde puedes mejorar, ubica las clases donde puedes aprenderlos y estudia vigorosamente.
- Es completamente válido hacer búsquedas en Google, cursos y tutoriales de Platzi, incluso usar tu cuaderno de notas sin importar si es físico o virtual.

Recuerda que **el éxito no se mide por cuánto tiempo te toma aprender**, esa métrica es relativamente inútil. Mejor concéntrate en completar los cursos de tu ruta de aprendizaje profesional y desarrollar los proyectos que realmente demuestran que dominas cada tecnología.

¡Mucha suerte!


## Variables y operaciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una variable y para qué sirve?
``` Espacio de memoria para almacenar información (dependiendo el tipo y estructas de datos segun el lenguaje) ```
- ¿Cuál es la diferencia entre declarar e inicializar una variable?
``` 
    Declarar variable: inicarle al lenguaje el nombre de la variable a utilizar y el tipo de datos
    Inicializar variable: inicarle al lenguaje el nombre de la variable y asignar un valor inicial
```
- ¿Cuál es la diferencia entre sumar números y concatenar strings?
``` 
    Sumar Numeros: aplica operacion matemematica a 2 o mas variables numericas (integer, float)
    Concatenar Strings: Une 2 o mas variables de tipo Strings en una sola salida.
```

- ¿Cuál operador me permite sumar o concatenar?
``` + ```

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

- Nombre ** String **
- Apellido ** String **
- Nombre de usuario en Platzi ** String **
- Edad ** Number**
- Correo electrónico ** String **
- Mayor de edad ** Boolean **
- Dinero ahorrado ** Number **
- Deudas ** Number **

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.
- let firstname = 'Haleym'
- let fullname = 'Hidalgo'
- let username = '@haleymhm'
- let age = 42
- let mail = 'haleymhm@gmail.com'
- let is_adult = True
- let saved_money = 150000
- let debts = 12000

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

- Nombre completo (nombre y apellido)
- Dinero real (dinero ahorrado menos deudas)
```
let name =  firstname + ' ' + fullname;
print(name);

let saldo balance = saved_money - debts;
print('Su saldo real es: ' + saldo);
```

## Funciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una función?
``` Son bloques de codigo reutilizables ```
- ¿Cuándo me sirve usar una función en mi código?
``` Cuando una accion se requiera utilizar mas de una seccion del codigo ```
- ¿Cuál es la diferencia entre parámetros y argumentos de una función?
```
Parametros: valores que requiere una funcion para su ejecuacion
Argumentos: valores que se indican al momento de ejecutar una funcion
```

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

```
const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
```
```
function message (name, lastname, nickname){
    let completeName = name + ' ' + lastname;
    console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
}

```

## Condicionales

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un condicional?
```
Son bloques de codigo que se ejecutan cuando una variable cumple con una condicion o validacion defeinida
```
- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
```
** If (elseif else): ** nos permite hacer validaciones completamente distintas en cada validación o condional

** switch:** Comparan con la misma variable o condición que definimos en el switch
```
- ¿Puedo combinar funciones y condicionales?

### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

```
const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Solo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       break;
   case "ExpertPlus":
       console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
       break;
}
```
```
const tipoDeSuscripcion = "Basic";

if (tipoDeSuscripcion == "Free") {
    console.log("Solo puedes tomar los cursos gratis");
}elsef (tipoDeSuscripcion == "Basic") {  
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
}elsef (tipoDeSuscripcion == "Expert") {    case "":
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
}elsef (tipoDeSuscripcion == "ExpertPlus") {   case "":
  console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}
```

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
```
const tipoDeSuscripcion = "Basic";

if (tipoDeSuscripcion == "Free") {
    console.log("Solo puedes tomar los cursos gratis");
}
if (tipoDeSuscripcion == "Basic") {  
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
}
if (tipoDeSuscripcion == "Expert") { 
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
}
if (tipoDeSuscripcion == "ExpertPlus") {
  console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}
```
```
let mensajes = {
  Free: "Solo puedes tomar los cursos gratis",
  Basic: "Puedes tomar casi todos los cursos de Platzi durante un mes",
  Expert: "Puedes tomar casi todos los cursos de Platzi durante un año",
  ExpertPlus: "Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"
}
const tipoDeSuscripcion = "Basic";
if(!!mensajes[tipoDeSuscripcion]) {
  console.log(mensajes[tipoDeSuscripcion]);
}
```
## Ciclos

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un ciclo? ``` Es ej un bloque de codigo mientra se cumpla una condicion ```
- ¿Qué tipos de ciclos existen en JavaScript?
```
- ** for: ** esta compuesta por de tres expresiones: __inicialización__ Sucede antes de la primera ejecución del bucle. Esta expresión es comúnmente utilizada para crear contadores; __condición__  Expresión que es evaluada antes de la ejecución de cada iteración; __expresión-final__ Expresión que se ejecuta luego de cada iteración. Usualmente es utilizada para incrementar un contador. Pero también puede ser utilizada para decrementar el contador
- ** while: ** Es un blucle que empieza por evaluar la condición. Si la condición es verdadera (devuelve true), entonces las sentencias son ejecutadas. Si la condición es falsa (devuelve false), entonces las sentencias no son ejecutadas. Luego el bucle finaliza.
- ** do: ** similar al bucle __while __  solo que la condición se evalúa al final por lo que el bloque de codigo es ejecuta al menos una vez
```
- ¿Qué es un ciclo infinito y por qué es un problema?
- ¿Puedo mezclar ciclos y condicionales?

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```
for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}
```
```
let i = 0;
while (i < 5) {
    console.log("El valor de i es: " + i);
    i++;
}

let i = 10;
while (i >= 5) {
    console.log("El valor de i es: " + i);
    i--;
}
```


### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es `2 + 2`. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

> 💡 Pista: puedes usar la función prompt de JavaScript.
```
let keep_on = true;

let sum = 0;

while(keep_on){
    sum = prompt("¿Cuánto es 2+2?")
    if (suma==4){
        console.log("Felicidades");
        keep_on = false;
    }
}

```
## Listas

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un array?
- ¿Qué es un objeto?
- ¿Cuándo es mejor usar objetos o arrays?
- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).


## ¿Cómo te fue? 🏆

**¡Felicidades por completar la prueba de JavaScript!** Confío en que hayas completado cada paso y hayas pausado para repasar los temas de los ejercicios que se te complicaron.

Ahora sí, continúa a la siguiente clase, pero recuerda que **ya no puedes abandonar el curso**, debes completarlo hasta el final. No importa cuánto tiempo te tome. **Yo sé que tú puedes. Y tú deberías de saberlo también.**

¡Te espero en la siguiente clase para comenzar!