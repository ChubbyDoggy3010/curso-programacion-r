# Sesión 1

1. Lo que quería conseguir:
  Construir una base de análisis (y modificarla para delimitar valores) a partir de
  nfl_data.csv para entender qué características permiten pronosticar el éxito de un jugador en la NFL. Asimismo,
  demostrar por qué lo que solicitó el jefe analista (solo incluir a los jugadores que habían completado las 5 prue-
  bas en el Combine) no es factible y no cumple o aporta a nuestro objetivo principal.

3. Archivos y código: sesion1_trabajo.Rmd (carga nfl_data.csv, construye
   la base de análisis y, al final, la parte A) Primero, se construyó una base de análisis de 3197 jugadores (des-
   pués de quitar jugadores repetidos y quitar a los de equipos especiales). Después, se creó otra tabla para comparar
   la tabla completa a la propuesta del jefe (resultando en 1,596 jugadores), base_alt (mi propuesta de las tres pruebas, resultando en 2,481
   jugadores), y base_sin_bench (la propuesta sin el press de banca, con 2,061 jugadores).
   
4. Comprobaciones que hice: (filas en cada paso, ¿compiló?, ¿con qué comprobaste la propuesta del analista jefe?)
   Para comprobar, conté las filas en cada paso (14,163 en la base de datos nfl_data.csv; 2,232 con drafts de 2000 a 2014; 3,200 sin equipos especiales; 3,197 sin repetidos. Después, para la
   propuesta de análisis del jefe comparé la base y base completa: organizando a los jugadores por posición, media y mediana
   de carear_av, proporción de los que sí fueron a Pro Bowl y jugadores de primera ronda. Cambios que conservé o descarté: (qué hiciste con la propuesta y por qué) Después de analizar los resultados de la
   propuesta, decidí descartarla. Deja un poco menos de la mitad de los jugadores y la cantidad de jugadores en ciertas posiciones (como QB's; bajan de 170 a 4) se pierden. Asimismo, se pierden más de la mitad de los de primera ronda. En su lugar, decidí conservar
   a quienes hicieron al menos 3 pruebas del combine el cual deja a 2,481 jugadores. Además, si solo fuera a quitar la condición de press de banca, recupero 465 jugadores, pero sigo perdiendo a quienes no hicieron alguna de las otras pruebas, así que el problema no desaparece del todo.
  
10. Lo que puedo afirmar:
   La base de análisis tiene 3,197 jugadores elegidos entre 2000 y 2014 en ocho posiciones. Los faltantes del Combine no son faltantes por azar: dependen de la posición (equipos especiales), así que borrar a quien le falte una prueba sesga la base. 
