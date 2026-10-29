# Pronosticar el éxito en la NFL

Proyecto del curso "Programar con criterio en la era de la IA".
Pregunta: ¿qué características de un jugador, conocidas en el draft,
permiten pronosticar su éxito profesional?

Autor/a: Fátima Díez Ontiveros

## Datos
- Archivo: nfl_data.csv del repositorio phcs971/nfl-draft-dataset
  (licencia MIT), leído desde una URL fijada a la versión 54730ea.
- Contenido: datos del draft y del Combine de la NFL; filas y 59 columnas 
- Base de análisis: entran 3,197 jugadores (los que fueron elegidos en el draft)

## Variables principales
- Éxito observado: carear_av (valor de carrera), el cual mide el valor acumulado del jugador en toda su carrera. Asimismo, incluye si fue al Pro Bowl o no (pro_bowl).
- Predictores: las pruebas del Combine (40 yardas, salto largo/vertical, press de banca y shuttle), la posición del jugador y la ronda del draft en la que fueron seleccionados. Estos se conocen antes o durante el draft, así que pueden servir para pronosticar su éxito. 

## Decisiones de limpieza
1. Solo tomar en cuenta los jugadores elegidos en el draft (son los únicos con carear_av)
2. Solo analizar datos del draft de 2000 a 2014 (delimitado a 3,232), porque la mayoría de los jugadores más "recientes" respecto al draft no han terminado su carrera y parecerían peores. Asimismo, estos datos son los más parecidos a la NFL actual, con siete rondas de draft y quince generaciones, suficientes para el proyecto.
3. No se incluyen equipos especiales (pateadores y despejadores, 32 jugadores; quedan 3,200):porque casi no hacen las pruebas físicas y su carear_av se mide de otra manera.
4. Quitar filas repetidas (3 jugadores aparecían dos veces; quedan 3,197): contarlos dos veces les daría mas "peso" en el análisis.
5. No exigir las cinco pruebas del Combine completas: hacerlo reduce el número a 1,596 y elimina a muchos jugadores de ciertas posiciones (especialmente QBs). En su lugar, conservo a quienes hicieron al menos 3 pruebas.  

## Carpetas
- sesion-1/ a sesion-5/: trabajos de cada sesión
