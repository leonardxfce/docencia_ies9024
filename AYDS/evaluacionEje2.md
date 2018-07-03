# Examen Eje 2


1. Leonardo, un programador en la misma empresa que vos, 
desarrollo la parte del login del sistema y lo para hacerlo creo una clase de la siguiente manera

| Clase Login	          |
|-------------------------|
|	String nombre | 
|	String usuario |
|	String nombreDeTabla |
|	String nombreDeBD |
|	String numeroIPdeBD |
|	String contraseñaBD | 
|	JOptionPane ventanaLogin         |
|	JOPtionPane ventanaError             |
|----------------------------------------|
|	public void mostrarPantallaDeLogin() |
|	public void conectarseAlaBD()        |
|	public void compararDatos()          |
|	public void mostrarVentanaError      |

* Esta clase esta no esta aplicando los principios GRASP. Tu tarea es:
	* Indicar cuales principios GRASP no estan aplicados
	* Elaborar un diseño mejorado de la parte del Login 

2. Marcelo necesita que el sistema que se le esta desarrollando pueda 
cargar datos sobre la materia prima que usa en su fabrica. En las entrevistas
que se tuvo con él se logro recabar la siguiente informacion:

> "La materia prima de nuestra fabrica, normalmente se pesa, se cataloga por su
tipo por ejemplo: duraznos, aceitunas, uvas, etc. Cada materia prima ademas se
registra con una fecha de entrada. Y existe la posiblidad que la materia prima tenga
un proveedor, en caso no tenerlo es de produccion propia. Las principales acciones
que hacemos a la materia prima es pesarla, o sea dar su peso, y quitarle la cascara,
ramas o hojas, depende del caso, que eso lo llamamos quitar peso."

* En base la informacion propocianda:
	* Diseñar la clase MateriaPrima aplicando los principios de Alta Cohesion y Experto en la informacion
	* ¿Que principo de GRASP de debe utilizar para terminar de diseñar la funcionalidad pedida por Marcelo para que funcione con JavaFX y MySQL?
	* Tener en cuenta en este caso que ya se creo la clase MateriaPrima, y se esta desarrollando el sistema siguiendo MVC.

3. Estas a 2 semanas de terminar el desarrollo pedido durante el año de la fabrica de Marcelo y el sistema desarrollado se ve de la siguiente forma

`
MateriaPrima ----- ConexionMySQL
Insumo ------ ConexionMySQL
ElementoSeguridad ----- ConexionMySQL
`

4. El IES es comprado por Microsoft y se les exige a los alumnos dejar de utilizar las BD de Oracle como lo es MySQL. El sistema actual esta 
"altamente acoplado" a MySQL, como resolverias la situacion. 

* ¿Que principos GRASP se deberian haber aplicado
* Propone vos un nuevo diseño aplicando los princpios GRASP correctos. Una ayuda... deberias usar Interfaces

4. El coordinador de la carrera decide que el futuro son las aplicaciones moviles, por lo cual se les exige todos los alumnos tirar a 
la hoguera el IDE Netbeans y utlizar AndroidStudio. Cada alumno estaba desarrollando su sistema utilizando JavaFX. por lo cual
el sistema se ve de la siguiente forma
`
PantallaFX  -----------> Insumo
`
> Para esta situacion Marcelo esta utilizando la version JavaFX, pero desde ahora hay que mantener las 2 versiones, lo cual nos dice
que dependiendo del cliente (Marcelo o Enzo) debemos "crear" una interfaz diferente. 

* ¿Como resolverias esta situacion a traves de GRASP, que principios usarias?
* Representar esa solcion con un diagrama

5. La profesora preferida de los alumnos de sistemas les pide una tarea a sus alumnos y ellos deseperados corren a realizarla
En la clase de Redes la profesora les explica las carateristicas principales de un Router

> "Un router CISCO, tiene un conector RJ45, 4 bocas Ethernet y 2 antenas Wifi" 

* ¿Que clase podrias diseñar con esta informacion?
* ¿Que principios utilizarias para justificar tu diseño?
	* Importante, aunque su profesora mas querida les dio una informacion "particular" pero las clases se diseñan de manera "general"

6. Javascript es un lenguaje de programacion que soporta orientacion a objetos, normalmente en el
se pueden crear clases las cuales pueden manipular el HTML, dentro del HTML se pueden generar eventos
como por ejemplo el "click" sobre un boton , el "input" sobre una caja de texto, o un "mouseover" cuando 
el mouse pasa sobre algun elemento.
La forma mas comun de programar en Javascript es hacer todas las cosas juntas, por ejemplo juntar la manipulacion
del HTML y manejar los eventos de sistema en la misma funcion.
Dada esta situacion se te solicita hacer una calculadora en javascript con HTML y el diseño de clases se ve
de la siguiente manera
`
HTMLCalculadora  ----> ???? -----> LogicaCaluladora
`
* Cual principio GRASP deberias utilizar para completar este diseño de sistemas
* Completa el diagrama utilizando la clase ,producto de aplicar el principio GRASP

7. Con motivo del mundial se les solicita desarrollar un juego
relacionado con el deporte del futbol, aplicando lo visto en AyDS
usted empieza a desarrollar el diagrama de clases y esta de la siguiente 
manera:
`
Delantero   
Pelota
Arbitro
`
* Utilice GRASP para terminar este diagrama de clases
* Nombre los distintos principios que aplico

8. El Banco Nacion lo llama por telefono para que revise su sistema de
cajeros automaticos, el encargado de sistemas del Banco Nacion le muestra la 
siguiente clase

|ATM |
|---- |
| Pesos billete |
| PanatallaTactil pantalla |
| TecladoNumerico teclado |
| Boveda boveda |
| Mastercard tarjeta |
| Epson impresoraInterna |
| int cantidadDeDinero |
| ---- | 
| darDinero() |
| mostrarOpcionesDeRetiro() | 
| leerContraseña() |
| contarDineroTotal() |
| imprimirTicket() |


> El gerente general del Banco le pide que este sistema debe permitir nuevas
tarjetas y tambien debe permitir dolares

* Que problemas relacionados con GRASP tiene actualmente este sistema
* Que princpios se deben aplicar para implementar los pedidos del banco

9. Esta diseñando una aplicacion para dar a conocer 
los distintos grupos/cantantes relacionados al mundo de la musica de 
Corea del Sur. El programador con el que usted esta realizando el sistema es Corea y le presenta
el siguiente diagrama

| Artista |
| ------ |
| String nombre | 
| String genero | 
| int integrantes | 
| int cantidadDeDiscos | 
| String[] canciones | 
| ---------- |
| getNombre() |
| setNombre() |
| getIntegrantes() |
| setIntegrantes() |

* ¿ Los metodos de esta clase son "altamente cohesivos"?
* En caso de no serlo, realice devuelta este diagrama corrigiendo o proponiendo cambios

10. Segun lo abordado que principios GRASP identifica en
el patron MVC 
`
Modelo  ---- Controlador ---- Vista
`
11. Nombrar los principios SOLID. ¿ Para que sirven en general ?
12. Cuales son las 4 caracteristicas principales de la software de calidad. Describir alguna de ellas
13. Que significa DRY. Que problemas traeria si no se corrige
14. Que es YAGNI y que importancia tiene el en el desarrollo en general
15. Como se traduce al codigo el principio de KISS.

















