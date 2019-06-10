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
<p> Guarde el programa con el nombre de hola.asm. </p>
<p> LUEGO ENTRAR AL DOS. </p>
<p>Y ENTRAR A LA RUTA DONDE ESTÁ GUARDADO EL PROGRAMA QUE ES D:\asm. </p>

<h2 class="heading to-animate"> 1.	primera compilación usando el masm(Microsoft macro assembler). </h2>
<h3> 1.1 Colocamos masm hola; y verificamos que no tenga errores.</h3>
<p>En este caso vemos que dice 0 severe Errors(0 errores severos) y 0 warning errors(0 errores peligrosos).</p>
<p>Algunos programas pueden tener 0 errores severos y 1 peligro, pero cuando hay 0 o n peligros el programa igual corre por q solo es una advertencia pero si tiene solo 1 error severo el programa no puede correr (eso se darán cuenta con la practica   ), luego colocamos el link hola;</p>
<p> Por último colocamos hola </p>
 <p> Si verifican la carpeta donde está el programa vemos que se crearon dos nuevos archivos</p>
 
 <h3>	1.2. COMPILACIÓN CON EL tasm(TURBO ASSEMBLER) </h3>
<p>Se sigue el mismo procedimiento de la anterior compilación con el masm.</p>
<p>Solo que en vez de colocar masm se coloca tasm y en vez de link tlink.</p>
 <p>Los warning y errores son los mismos que el masm</p>
<p>Las diferencias se los dejo de tarea, pero se darán cuenta que por un pequeñísimo margen el tasm es mejor que el masm por que tiene funcione propias del compilador y ademas nos permite hacer más saltos que para el masm son errores de compilacion.</p>
<h3>1.3 Ejecución usando el emulator 8086. </h3>
<p>Como siempre se deja lo más fácil al final, el emu8086 es un ide tipo eclipse, codeblock etc para assembler donde primero creamos un programa en blanco seleccionando la parte de NEW.</p>

<p> Luego seleccionamos la parte que dice documento en blanco y copiamos el código para hacer corre el programa nos situamos en la flecha verde que dice emulate y le damos click para hacer correr y luego le damos Run.</p>
  
<p>Lo malo del emu8086 es que no tiene todas a las interrupciones del assembler como ser rastreo de teclado modo gráfico y modo de video archivos y algunas más pero para empezar a aprender el lenguaje ensamblador en muy buena herramienta.</p>


<h2 class="heading to-animate"> 2. REGISTROS DE LA UCP </h2>

<p>La UCP tiene 14 registros internos, cada uno de 16 bits. Los primeros cuatro, AX, BX, CX, y DX son registros de uso general y también pueden ser utilizados como registros de 8 bits, para utilizarlos como tales es necesario referirse a ellos como, por ejemplo: AH y AL, que son los bytes alto (high) y bajo (low) del registro AX. Esta nomenclatura es aplicable también a los registros BX, CX y DX.</p>
<p> Los registros son conocidos por sus nombres específicos: </p>

<h3>REGISTROS DE USO GENERAL</h3>
	AX: Acumulador
	BX: Registro base 
	CX: Registro contador 
	DX: Registro de datos 
        DS Registro del segmento de datos
        ES Registro del segmento extra
        SS Registro del segmento de pila
        CS Registro del segmento de código
        BP Registro de apuntadores base
        SI Registro índice fuente
        DI Registro índice destino
        SP Registro del apuntador de la pila
        IP Registro de apuntador de siguiente instrucción
        F Registro de banderas



