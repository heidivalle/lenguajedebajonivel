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
