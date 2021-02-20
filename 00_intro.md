{{meta {load_files: ["code/intro.js"]}}}

# Introducción

{{quote {author: "Ellen Ullman", title: "Close to the Machine: Technophilia and its Discontents", chapter: true}

Pensamos que estamos creando el sistema para nuestros propios propósitos. Creemos que
lo estamos haciendo a nuestra propia imagen... Pero la computadora no es realmente
como nosotros. Es una proyección de una pequeñísima parte de nosotros: esa
porción dedicada a la lógica, el orden, las reglas, y la claridad.

quote}}

{{figure {url: "img/chapter_picture_00.jpg", alt: "Imagen de un destornillador y una placa de circuito", chapter: "framed"}}}

Este es un libro sobre instruir ((computadora))s. Las computadoras son casi tan
comunes como los destornilladores hoy en día, pero son bastante más complejas,
y ponerlas a hacer lo que quieres que hagan no siempre es tarea sencilla.

Si la tarea que tienes para tu computadora es una común, bien definida,
como mostrarte tu correo electrónico o actuar como una calculadora,
puedes abrir la ((aplicación)) apropiada y ponerla a trabajar. Pero para
tareas únicas o abiertas, probablemente aún no exista tal aplicación.

Ahí es donde la ((programación)) puede entrar en juego. _Programar_ es la acción de
construir un _programa_—un conjunto de instrucciones precisas que le dicen a la
computadora qué hacer. Dado que las computadoras son bestias tontas y pedantes,
la programación es fundamentalmente tediosa y frustrante.

{{index [programming, "joy of"], speed}}

Afortunadamente, si puedes pasar eso por alto, y tal vez incluso disfrutes del rigor
de pensar en términos que las máquinas tontas puedan trabajar, la programación puede ser
gratificante. Te permite hacer en segundos cosas que tomarían
_todo el tiempo_ haciéndolas manualmente. Es una forma de poner tu herramienta, la computadora,
a hacer cosas que no podía hacer antes. Además proporciona un maravilloso
ejercicio de pensamiento abstracto.

La mayoría de la programación se hace con ((lenguajes de programación)). Un _lenguaje
de programación_ es un lenguaje construido artificialmente utilizado para instruir
computadoras. Es interesante que la manera más efectiva que hemos encontrado
para comunicarnos con una computadora sea tan similar a la manera en la que nos
comunicamos entre nosotros. Al igual que los lenguajes humanos, los lenguajes de computadora
permiten que las palabras y frases se combinen de nuevas formas, haciendo posible
la expresión de más y más conceptos nuevos.

{{index [JavaScript, "availability of"], "casual computing"}}

En algún momento las interfaces basadas en lenguajes, como las terminales de BASIC y DOS
de los 1980s y 1990s, donde el método principal de interactuar con
las computadoras. Estas han sido en su mayoría remplazadas por interfaces visuales,
que son más sencillas de aprender pero ofrecen menos libertad. Los lenguajes de computadora
siguen ahí, si sabes donde buscar. Uno de esos lenguajes,
JavaScript, está integrado en todos los ((navegadores)) web modernos y por lo tanto
está disponible en casi todos los dispositivos.

{{indexsee "web browser", browser}}

Este libro intentará familiarizarte lo suficiente con este lenguaje para
hacer cosas útiles y asombrosas con él.

## Sobre la programación

{{index [programming, "difficulty of"]}}

Además de explicar JavaScript, introduciré los principios
básicos de la programación. Sucede que programar es difícil. Las
reglas fundamentales son claras y simples, pero los programas construidos sobre
estas reglas tienden a hacerse lo suficientemente complejas como para introducir sus propias reglas
y complejidad. Estás construyendo tu propio laberinto, de cierta forma, y podrías
simplemente perderte en él.

{{index learning}}

Habrá momentos en los que leer este libro se sentirá terriblemente frustrante.
Si eres nuevo en la programación, habrá un montón de material nuevo por
digerir. Mucho de este material será _combinado_ de maneras que
requieren de realizar conexiones adicionales.

Está en ti realizar el esfuerzo necesario. Cuando tengas dificultades
para seguir el libro, no saltes a ninguna conclusión sobre tus propias
capacidades. Estás bien—solo necesitas perseverar. Toma un descanso,
vuelve a leer parte del material, y asegúrate de que lees y entiendes los
programas de ejemplo y los ((ejercicios)). Aprender es un trabajo duro, pero
todo lo que aprendas es tuyo y hará que el siguiente aprendizaje
sea más fácil.

{{quote {author: "Ursula K. Le Guin", title: "The Left Hand of Darkness"}

{{index "Le Guin, Ursula K."}}

Cuando la acción se vuelve improductiva, reúne información; cuando la información
se vuelve improductiva, duerme.

quote}}

{{index [program, "nature of"], data}}

Un programa es muchas cosas. Es una pieza de texto escrita por un programador,
es la fuerza que dirige, que pone a la computadora a hacer lo que hace, es
la información en la memoria de la computadora, y, sin embargo, controla las acciones
ejecutadas sobre esta misma memoria. Las analogías que intentan comparar programas
con objetos con los que estamos familiarizados tienden a quedarse cortos. Una que superficialmente
coincide es aquella con una máquina—montones de partes separadas suelen estar
involucradas, y para echar a andar las cosas, tenemos que considerar las
formas en las que estas partes se interconectan y contribuyen a la operación
de la totalidad de la máquina.

Una ((computadora)) es una máquina física que actúa como hospedaje para estas máquinas
inmateriales. Las computadoras por sí mismas solo pueden hacer cosas estúpidamente directas.
La razón de que sean tan útiles es que hacen estas cosas a
una ((velocidad)) increíblemente alta. Un programa puede copmbinar ingeniosamente un
número enorme de estas acciones simples para hacer tareas
muy complicadas.

{{index [programming, "joy of"]}}

Un programa es una construcción del pensamiento. Construirlo no tiene un costo, no
tiene peso, y crece fácilmente bajo nuestras manos que lo escriben.

Pero si no se tiene cuidado, el tamaño de un programa y su ((complejidad)) crecerá fuera de
control, confundiendo aún a la persona que lo creó. Mantener los programas
bajo control es el problema principal de la programación. Cuando un programa
funciona, es hermoso. El arte de la programación es la habilidad de
controlar la complejidad. El gran programa es domado—simplificando
su complejidad.

{{index "programming style", "best practices"}}

Algunos programadores creen que esta complejidad se maneja mejor usando
solo un conjunto pequeño de técnicas conocidas en sus programas. Han
construido reglas estrictas ("buenas prácticas") que prescriben la forma
que los programas deberían tener y mantenerse cuidadosamente dentro de su pequeña
zona segura.

{{index experiment}}

Esto no solo es aburrido, no es efectivo. Los nuevos problemas a menudo
requieren de nuevas soluciones. El campo de la programación es joven y aún
se desarrolla rápidamente, y es lo suficientemente variada como para dar lugar a estrategias
radicalmente distintas. Hay muchos errores terribles que se pueden hacer
en el diseño de programas, y deberías adelantarte a cometerlos para que los
puedas entender. Un instinto de cómo debe ser un buen programa se
desarrolla con la práctica, no se aprende de una lista de reglas.

## ¿Por qué importa el lenguaje?

{{index "programming language", "machine code", "binary data"}}

Al inicio, en el nacimiento de la computación, no había lenguajes
de programación. Los programas eran más o menos así:

```{lang: null}
00110001 00000000 00000000
00110001 00000001 00000001
00110011 00000001 00000010
01010001 00001011 00000010
00100010 00000010 00001000
01000011 00000001 00000000
01000001 00000001 00000001
00010000 00000010 00000000
01100010 00000000 00000000
```

{{index [programming, "history of"], "punch card", complexity}}

Ese es un programa para sumar los números del 1 al 10 e imprimir
el resultado: `1 + 2 + ... + 10 = 55`. Podía ejecutarse en una máquina,
simple e hipotética. Para programar en las primeras computadoras, era necesario
montar grandes arreglos de interruptores en la posición correcta o ponchar agujeros en
tiras de cartón e ingresarlas a la computadora. Probablemente te puedes
imaginar lo tedioso y propenso a errores de este procedimiento. Incluso para escribir
programas simples se requería mucha destreza y disciplina. Los complejos
eran prácticamente inconcebibles.

{{index bit, "wizard (mighty)"}}

Por supuesto, ingresar manualmente estos patrones arcaicos de bits (unos
y ceros) le daban al programador una profunda sensación de ser un poderoso
hechicero. Y eso tuvo que valer bastante en términos de satisfacción
laboral.

{{index memory, instruction}}

Cada línea del programa anterior contiene una sola instrucción. Podría
escribirse en español de esta forma:

 1. Guarda el número 0 en la posición de memoria 0.
 2. Guarda el número 1 en la posición de memoria 1.
 3. Guarda el valor de la posición de memoria 1 en la posición de memoria 2.
 4. Resta el número 11 del valor en la posición de memoria 2.
 5. Si el valor en la posición de memoria 2 es el número 0,
    continúa con la instrucción 9.
 6. Suma el valor de la posición de memoria 1 a la posición de memoria cero 0.
 7. Suma el número 1 al valor de la posición de memoria 1.
 8. Continúa con la instrucción 3.
 9. Imprime el valor de la posición de memoria 0.

{{index readability, naming, binding}}

Aunque eso ya es más legible que la sopa de bits, todavía
es un tanto opaco. Usar nombres en lugar de números para
las instrucciones y posiciones de memoria puede ayudar.

```{lang: "text/plain"}
 Asignar a “total” el valor 0.
 Asignar a “count” el valor 1.
[loop]
 Asignar a “compare” el valor “count”.
 Restar 11 de “compare”.
 Si “compare” es cero, continuar en [end].
 Sumar “count” a “total”.
 Sumar 1 a “count”.
 Continuar en [loop].
[end]
 Imprimir “total”.
```

{{index loop, jump, "summing example"}}

¿Puedes ver cómo trabaja el programa ahora? Las primeras dos líneas
asignan a dos posiciones de memoria sus valores iniciales: `total` será utilizado
para construir el resultado de la computación, y `count` dará seguimiento
del número que estamos procesando cada vez. Las líneas que usan
`compare` son probablemente las más extrañas. El programa quiere saber
si `count` es igual a 11 para decidir si puede detener
su ejecución. Como nuestra máquina hipotética es bastante primitiva, solo puede
preguntar si un número es cero y tomar una decisión basada
en ello. Así que usa la posición de memoria con la etiqueta `compare` para calcular
el valor de `count - 11` y toma una decisión basándose en ese valor.
Las siguientes dos líneas suman el valor de `count` al resultado e
incrementan `count` en 1 cada vez que el programa ha decidido que `count`
aún no es igual a 11.

Aquí está ese mismo programa en JavaScript:

```
let total = 0, count = 1;
while (count <= 10) {
  total += count;
  count += 1;
}
console.log(total);
// → 55
```

{{index "while loop", loop, [braces, block]}}

Esta version nos da unas cuantas mejoras. Sobre todo, no
hay necesidad de especificar la forma en la que queremos que el programa salte hacia adelante y atrás
de nuevo. La construcción `while` se encarga de eso. Continúa
ejecutando el bloque (rodeado de llaves) que lse sigue mientras la
condición que le asignaron sea verdadera. Esa condición es `count <= 10`, la cual
significa “_count_ es menor o igual a 10”. Ya no necesitamos
crear un valor temporal y comparar eso con cero, lo cual era solo un
detalle irrelevante para el programa. Parte del poder de los lenguajes de programación es
que pueden encargarse de detalles irrelevantes por nosotros.

{{index "console.log"}}

Al final del programa, después de que la contrucción `while` ha terminado,
la operación `console.log` es utilizada para escribir el resultado en pantalla.

{{index "sum function", "range function", abstraction, function}}

Finalmente, aquí está una muestra de cómo podría verse el programa si contáramos
con las operaciones convenientes `range` y `sum`, las cuales
respectivamente crean una ((colección)) de números dentro del intervalo y
calculan la suma de una colección de números:

```{startCode: true}
console.log(sum(range(1, 10)));
// → 55
```

{{index readability}}

La moraleja de esta historia es que el mismo programa puede expresarse de
forma larga o corta, legible o ilegible. La primer version del
programa era extremadamente opaca, mientras que esta última está casi
en inglés: `log` (imprime) la `sum` (suma) del `range` (intervalo) de números del 1 al 10. (En
los [siguientes capítulos](data) veremos cómo definir operaciones como `sum`
y `range`.)

{{index ["programming language", "power of"], composability}}

Un buen lenguaje de programación ayuda a los programadores permitiéndoles
hablar sobre las acciones que la computadora tiene que realizar en un nivel más
alto. Ayuda a omitir detalles, provee bloques de construcción convenientes
(como `while` y `console.log`), te permite definir tus propios
bloques de construcción (como `sum` y `range`), y hace que esos bloques
sean fáciles de componer entre sí.

## ¿Qué es JavaScript?

{{index history, Netscape, browser, "web application", JavaScript, [JavaScript, "history of"], "World Wide Web"}}

{{indexsee WWW, "World Wide Web"}}

{{indexsee Web, "World Wide Web"}}

JavaScript fue introducido en 1995 como una forma de agregar programas a las
páginas web, en el navegador web Netscape Navigator. El lenguaje ha sido adoptado
desde entonces por todos los demás navegadores web principales. Ha hecho posibles las
aplicaciones web—aplicaciones con las que puedes interactuar
directamente sin realizar una recarga de la página por cada acción. JavaScript también es
utilizado en más sitios web tradicionales para proveer varias formas
de interacción e inteligencia.

{{index Java, naming}}

It is important to note that JavaScript has almost nothing to do with
the programming language named Java. The similar name was inspired by
marketing considerations rather than good judgment. When JavaScript
was being introduced, the Java language was being heavily marketed and
was gaining popularity. Someone thought it was a good idea to try to
ride along on this success. Now we are stuck with the name.

{{index ECMAScript, compatibility}}

After its adoption outside of Netscape, a ((standard)) document was
written to describe the way the JavaScript language should work so
that the various pieces of software that claimed to support JavaScript
were actually talking about the same language. This is called the
ECMAScript standard, after the Ecma International organization that
did the standardization. In practice, the terms ECMAScript and
JavaScript can be used interchangeably—they are two names for the same
language.

{{index [JavaScript, "weaknesses of"], debugging}}

There are those who will say _terrible_ things about JavaScript. Many
of these things are true. When I was required to write something in
JavaScript for the first time, I quickly came to despise it. It would
accept almost anything I typed but interpret it in a way that was
completely different from what I meant. This had a lot to do with the
fact that I did not have a clue what I was doing, of course, but there
is a real issue here: JavaScript is ridiculously liberal in what it
allows. The idea behind this design was that it would make programming
in JavaScript easier for beginners. In actuality, it mostly makes
finding problems in your programs harder because the system will not
point them out to you.

{{index [JavaScript, "flexibility of"], flexibility}}

This flexibility also has its advantages, though. It leaves space for
a lot of techniques that are impossible in more rigid languages, and
as you will see (for example in [Chapter ?](modules)), it can be used
to overcome some of JavaScript's shortcomings. After ((learning)) the
language properly and working with it for a while, I have learned to
actually _like_ JavaScript.

{{index future, [JavaScript, "versions of"], ECMAScript, "ECMAScript 6"}}

There have been several versions of JavaScript. ECMAScript version 3
was the widely supported version in the time of JavaScript's ascent to
dominance, roughly between 2000 and 2010. During this time, work was
underway on an ambitious version 4, which planned a number of radical
improvements and extensions to the language. Changing a living, widely
used language in such a radical way turned out to be politically
difficult, and work on the version 4 was abandoned in 2008, leading to
a much less ambitious version 5, which made only some uncontroversial
improvements, coming out in 2009. Then in 2015 version 6 came out, a
major update that included some of the ideas planned for version 4.
Since then we've had new, small updates every year.

The fact that the language is evolving means that browsers have to
constantly keep up, and if you're using an older browser, it may not
support every feature. The language designers are careful to not make
any changes that could break existing programs, so new browsers can
still run old programs. In this book, I'm using the 2017 version of
JavaScript.

{{index [JavaScript, "uses of"]}}

Web browsers are not the only platforms on which JavaScript is used.
Some databases, such as MongoDB and CouchDB, use JavaScript as their
scripting and query language. Several platforms for desktop and server
programming, most notably the ((Node.js)) project (the subject of
[Chapter ?](node)), provide an environment for programming JavaScript
outside of the browser.

## Code, and what to do with it

{{index "reading code", "writing code"}}

_Code_ is the text that makes up programs. Most chapters in this book
contain quite a lot of code. I believe reading code and writing ((code))
are indispensable parts of ((learning)) to program. Try to not just
glance over the examples—read them attentively and understand them.
This may be slow and confusing at first, but I promise that you'll
quickly get the hang of it. The same goes for the ((exercises)). Don't
assume you understand them until you've actually written a working
solution.

{{index interpretation}}

I recommend you try your solutions to exercises in an actual
JavaScript interpreter. That way, you'll get immediate feedback on
whether what you are doing is working, and, I hope, you'll be tempted
to ((experiment)) and go beyond the exercises.

{{if interactive

When reading this book in your browser, you can edit (and run) all
example programs by clicking them.

if}}

{{if book

{{index download, sandbox, "running code"}}

The easiest way to run the example code in the book, and to experiment
with it, is to look it up in the online version of the book at
[_https://eloquentjavascript.net_](https://eloquentjavascript.net/). There,
you can click any code example to edit and run it and to see the
output it produces. To work on the exercises, go to
[_https://eloquentjavascript.net/code_](https://eloquentjavascript.net/code),
which provides starting code for each coding exercise and allows you
to look at the solutions.

if}}

{{index "developer tools", "JavaScript console"}}

If you want to run the programs defined in this book outside of the
book's website, some care will be required. Many examples stand on their
own and should work in any JavaScript environment. But code in later
chapters is often written for a specific environment (the browser or
Node.js) and can run only there. In addition, many chapters define
bigger programs, and the pieces of code that appear in them depend on
each other or on external files. The
[sandbox](https://eloquentjavascript.net/code) on the website provides
links to Zip files containing all the scripts and data files
necessary to run the code for a given chapter.

## Overview of this book

This book contains roughly three parts. The first 12 chapters discuss
the JavaScript language. The next seven chapters are about web
((browsers)) and the way JavaScript is used to program them. Finally,
two chapters are devoted to ((Node.js)), another environment to
program JavaScript in.

Throughout the book, there are five _project chapters_, which describe
larger example programs to give you a taste of actual programming. In
order of appearance, we will work through building a [delivery
robot](robot), a [programming language](language), a [platform
game](game), a [pixel paint program](paint), and a [dynamic
website](skillsharing).

The language part of the book starts with four chapters that introduce
the basic structure of the JavaScript language. They introduce
[control structures](program_structure) (such as the `while` word you
saw in this introduction), [functions](functions) (writing your own
building blocks), and [data structures](data). After these, you will
be able to write basic programs. Next, Chapters [?](higher_order) and
[?](object) introduce techniques to use functions and objects to write
more _abstract_ code and keep complexity under control.

After a [first project chapter](robot), the language part of the book
continues with chapters on [error handling and bug fixing](error),
[regular expressions](regexp) (an important tool for working with
text), [modularity](modules) (another defense against complexity), and
[asynchronous programming](async) (dealing with events that take
time). The [second project chapter](language) concludes the first part
of the book.

The second part, Chapters [?](browser) to [?](paint), describes the
tools that browser JavaScript has access to. You'll learn to display
things on the screen (Chapters [?](dom) and [?](canvas)), respond to
user input ([Chapter ?](event)), and communicate over the network
([Chapter ?](http)). There are again two project chapters in this
part.

After that, [Chapter ?](node) describes Node.js, and [Chapter
?](skillsharing) builds a small website using that tool.

{{if commercial

Finally, [Chapter ?](fast) describes some of the considerations that
come up when optimizing JavaScript programs for speed.

if}}

## Typographic conventions

{{index "factorial function"}}

In this book, text written in a `monospaced` font will represent
elements of programs—sometimes they are self-sufficient fragments, and
sometimes they just refer to part of a nearby program. Programs (of
which you have already seen a few) are written as follows:

```
function factorial(n) {
  if (n == 0) {
    return 1;
  } else {
    return factorial(n - 1) * n;
  }
}
```

{{index "console.log"}}

Sometimes, to show the output that a program produces, the
expected output is written after it, with two slashes and an arrow in
front.

```
console.log(factorial(8));
// → 40320
```

Good luck!
