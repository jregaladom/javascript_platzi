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
  Es una espacio temporal en memoria, se define con una palabra recerbada let, const, var y un nombre.

- ¿Cuál es la diferencia entre declarar e inicializar una variable?
  Al declarar la variable se recerba ese espacio temporal de memoria, al inicializar se asignan valor a ese espacio reservado.

- ¿Cuál es la diferencia entre sumar números y concatenar strings?
  Sumar es una operación matematica y concatener es la unión de arreglo de caracteres

- ¿Cuál operador me permite sumar o concatenar?
  Es el operador +, nos permite hacer la suma o concatener string, dependiendo del tipo de dato en el que realice la función determinará si realiza la operación matematica en tipo de datos númericos o concatenar con tipos de datos string.

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

- Nombre (String)
- Apellido (String)
- Nombre de usuario en Platzi (String)
- Edad (number)
- Correo electrónico (String)
- Mayor de edad (boolean)
- Dinero ahorrado (number)
- Deudas (number)

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

let nombre = "Jose Juan";
let apellido = "Regalado";
let nombreUsuario = "jregalado";
let edad = "32";
let correoElectronico = "jregaladomoncada@gmail.com";
let mayorEdad = true;
let dineroAhorrado = "50.50";
let deudas = "500000";

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

- Nombre completo (nombre y apellido)
  let nombreCompleto = nombre+' '+ apellido;

- Dinero real (dinero ahorrado menos deudas)
  let dineroReal = dineroAhorrado - deudas;

## Funciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una función?
  Es la encapsulación de instrucciones que puede ser llamada con un nombre y valores de entrada (opcional), la función puede realizar los pasos que contiene internamente y devolver algún resultado (opcional)

- ¿Cuándo me sirve usar una función en mi código?
  Cuando se pretende realizar repedidamente una serie de acciones.

- ¿Cuál es la diferencia entre parámetros y argumentos de una función?
  Los parametros son las variables de entrada de una función, necesarias para relizar cada una de las instrucciones que contiene esa función. Los argumentos son los valores que se asignan a esos parametros cuando se realiza el llamado de la función.

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

```
const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");


function saludo(name,lastName,nickname){
    const completeName = name + " " + lastName;
    console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
}
```

## Condicionales

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un condicional?
  Es una comparación de valores, la forma que realiza la ejecución de un bloque de codigo bajo una valuadación

- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
  If, swtich

- ¿Puedo combinar funciones y condicionales?
  Sí

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

if(tipoDeSuscripcion == "Free"){
     console.log("Solo puedes tomar los cursos gratis");
} else if(tipoDeSuscripcion == "Basic"){
     console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} else if(tipoDeSuscripcion == "Expert"){
     console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
} else if(tipoDeSuscripcion == "ExpertPlus"){
      console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}
```

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

if(tipoDeSuscripcion == "Free"){
console.log("Solo puedes tomar los cursos gratis");
}

if(tipoDeSuscripcion == "Basic"){
console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
}

if(tipoDeSuscripcion == "Expert"){
console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
}

if(tipoDeSuscripcion == "ExpertPlus"){
console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}

> 💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays y un solo condicional. 😏

## Ciclos

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un ciclo?
  Es la ejecución de un bloque de código mientras se cumpla cierta validación, en caso de que se deje de cumplir el bloque de codigo dejará de ser ejecutado.

- ¿Qué tipos de ciclos existen en JavaScript?
  For, foreach, while, do while

- ¿Qué es un ciclo infinito y por qué es un problema?
  Es la ejecución infinita de una condición, la no cumplir con una valiadación negativa esté nunca se detiene. Puede llegar a ser un problema al desbordar la memoria del equipo en donde se ejecuta.

- ¿Puedo mezclar ciclos y condicionales?
  Sí.

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```
for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}
```

### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es `2 + 2`. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

> 💡 Pista: puedes usar la función prompt de JavaScript.

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
