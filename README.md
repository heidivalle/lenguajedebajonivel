# lenguajedebajonivel

ASSEMBLER IDE 2.0 


<h2 class="heading to-animate">DEFINICIÓN</h2>
<p> Inicio como hacer correr un programa en assembler.</p>
<p>Lo primero que tienen que hacer para  correr un programa en assembler es primero crear un programa para este caso haremos el clásico hola mundo, para ello lo haremos un editor de texto para este ejemplo trabajaremos con el notepad++.
Que pueden descargar de forma gratuita desde su página oficial una vez descargado e instalado procederemos a hacer el programa, para ello en la parte de lenguaje del notepad++ seleccionen la parte que dice assembler</p>

<h2 class="heading to-animate">Y CREAMOS EL PROGRAMA QUE IMPRIMA EL HOLA MUNDO.</h2>
<p> .model small</p>
<p>  .stack 256</p></p>
 <p> .data</p>
 <p> msg db “hola mundo$” ;comentarios</p>
 <p> .code</p></p>
 <p> mov ax,@data</p>
 <p> mov ds,ax</p></p>
 <p> mov ah,09h</p>
 <p> lea dx,msg</p>
 <p> int 21h</p>
 <p> mov ah,4ch</p>
 <p> int 21h</p>
 <p> end</p>
<h2 class= "heading to-animate">ANTES DE CONTINUAR EXPLICAREMOS EL CODIGO </h2>
<p> Primero definimos el modelo de memoria con .model existen muchos tipos de memoria los más conocidos son el tyni que se usa para programas pequeños, el small para programas medianos y el large para programas largos. Después el tamaño de la pila que su función es un poco más avanzada y conocerán su función cuando hagan programas más complejos pero por ahora solo vean lo como el tamaño del programa, luego definimos las variables de datos con un .data que es donde están la variables  y declaramos una variable que se llame msg y lo podemos como tipo de dato que sea DB (define byte) existen más datos como el DW el DD que verán el funcionamiento después, luego ponemos él .code que es donde va el código, para más información acerca del lenguaje assembler se le recomienda leer el libro introducción al lenguaje ensamblador de peter Abel o los artículos de internet de abre los ojos al ensamblador:).</p>
<p>Luego guardamos el programa con la extensión .asm (verificar si tiene esa extensión), guardarlo en una carpeta donde tenga el masm, tasm, tasm y tlink.  (luego en el final pronde un link para que descarguen los programas mencionados). </p>
