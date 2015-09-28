# Análisis de código

A continuación se presenta el análisis de los resultados de las pruebas que ejecuto SONAR sobre el proyecto Appoteca como nos fue entregado:

#Evidencias de deuda técnica
####Reporte de métricas sonar.
####Grupo 5 Appoteca.
####Gestión de proyectos de desarrollo de software 2015-20.

#Introducción
El proyecto que se analizó con SonarQube se llama AppMarketPlace. Es un sistema que tiene como fin permitir a los desarrolladores promocionar sus aplicaciones a través de una tienda virtual. Permite tanto a desarrolladores como usuarios a registrarse en el sistema, los desarrolladores pueden subir sus aplicaciones con el contenido asociado como imágenes, videos y descripciones para que los usuarios puedan ver esta información y poder comprar dicha aplicación. Adicionalmente permite generar reportes para que los desarrolladores puedan ver sus ventas y los usuarios sus compras respectivamente. 



#Análisis


##Documentación: 

![alt text](http://s29.postimg.org/qfzl24ld3/Screen_Shot_2015_08_29_at_9_20_44_AM.png "Logo Title Text 1")
Se refiere a las líneas de código ya sea comentarios o código.  En cuanto a AppMarketplace, se tiene un total de 65.2% de documentación, lo cual nos muestra que hay cierta documentación (según sonar), pero analizando el código, dicha documentación no es suficientemente clara y no explica claramente o no se da suficiente información como para explicar qué hace cada método, a continuación se muestran ejemplos de la documentación que hay:




  #### */

   #### * @author Jhonatan

   ####*/



  #### /**
   
  #### * @generated
    

   #### */
   
   
Como grupo, en cuanto a esta métrica estamos de acuerdo en que si bien la documentación actual no está completa, nos comprometemos a realizar la debida documentación de cáda desarrollo que hagamos en el proyecto de ahora en adelante.
   
   
   ## Lines of code: 
   

   
   ![alt text](http://s29.postimg.org/cxsopu97r/Screen_Shot_2015_08_29_at_9_35_45_AM.png "Logo Title Text 1")
   Esta métrica representa el total de líneas de código generadas dentro del proyecto, en caso AppMarketplace hay un total de 2119 líneas de código, divididas en 1690 líneas de código en Java, 321 líneas de JavaScript y 108 líneas de código Web . Por ahora no es un proyecto de gran dimensión pero al avanzar el curso se incluirán más requerimientos, los cual hará que esta métrica incremente significativamente.
   
  Files: Representa el número de archivos que contiene el proyecto, en este caso, AppMarketplace cuenta con un total 53 archivos.

Functions: Número total de métodos en toda la aplicación, actualmente en AppMarketplace hay 211 funciones.

Classes: Número total de clases en el proyecto Incluyendo interfaces, enums y anotaciones. En este proyecto hay un total de 37 clases.

Accessors: Número total de métodos get y set utilizados en el proyecto, en total son 98.


##Duplications:
   ![alt text](http://s29.postimg.org/nuu0elvzb/Screen_Shot_2015_08_29_at_9_41_42_AM.png "Logo Title Text 1")

 Se refiere al número total de grupos de código repetidos, para que un grupo de código se considere como duplicado debe haber al menos 10 líneas de código sucesivas y repetidas. La indexación y los espacios son ignorados por lo que en un proyecto puede tener bastantes líneas duplicadas. En AppMarketplace hay un 13.9 % de líneas de código duplicadas que representan un total de 456 líneas de código separado en 14 grupos y 10 archivos. Esta métrica nos dice que hay un buen número de código repetido en este proyecto, pero esto pertenece a código generado por lo que no hay necesidad de hacer cambios en el código y podemos tomarlo como punto de partida a nuestros desarrollos posteriores.

##Complexity: 
  ![alt text](http://s29.postimg.org/a2fliz57r/Screen_Shot_2015_08_29_at_9_50_38_AM.png "Logo Title Text 1")
  
  Esta métrica se refiere a la complejidad ciclomática del código. Nos da  una visión de la complejidad de un programa. Esta métrica muestra el número de pruebas a realizar para asegurar que se ejecuta una sentencia al menos una vez. Como podemos ver, la complejidad es de 327 lo cual nos dice que el todo el proyecto tanto el web como el backend no tienen mucha complejidad y los algoritmos se encuentran bien implementados y son óptimos. 

##Technical debt:
  ![alt text](http://s29.postimg.org/zcad62bzb/Screen_Shot_2015_08_29_at_10_06_07_AM.png "Logo Title Text 1")
   se refiere al esfuerzo para arreglar todos los problemas en el código fuente. Hay muchas causas que aumentan la deuda técnica, entre esas está el afán, la presión, falta de conocimiento, falta de documentación, falta de buenas prácticas, falta de pruebas unitarias, etc. Para calcular la deuda técnica se basa principalmente en código duplicado, pruebas unitarias con errores, falta de pruebas unitarias, falta de documentación del código. En El caso AppMarketPlace la deuda técnica es de 1 día, lo cual nos dice que hay que pagar un total de 1 día para arreglar los problemas y errores en la aplicación (web y backend). Aquí hay un factor interesante, ya que dependiendo del tamaño del proyecto se puede saber si hay muchos problemas o no, es decir si el proyecto es pequeño y la deuda técnica es de 1 día o si el proyecto es grande y la deuda técnica es igual, hay una gran diferencia en ambos proyectos en cuanto al grado de diferencia de la deuda técnica, esta métrica la veremos a continuación.

Technical debt ratio: El valor de esta métrica depende del tamaño del proyecto y dependiendo de esta métrica se obtiene la calificación del código que va desde A que es muy bueno hasta E que es la peor calificación. En AppMarketPlace la proporción de deuda técnica es de 0.8 % lo cual nos da a entender que si bien hay que tomarse 1 día para arreglar los problemas en el código, no hay tantos problemas y no es muy alta esta métrica como para alarmarse, con el estado del código como nos fue entregado, podemos empezar a agregar nuevas funcionalidades sin preocuparnos del código que ya tenemos, ya que se encuentra en buen estado y cuenta con buenas prácticas de programación.

##Issues: 

Al mirar los issues del proyecto en SonarQube, se tienen en cuenta los bugs que pueden impactar el comportamiento de todo el sistema en términos de desempeño, bugs de seguridad, problemas de duplicación de código, parámetros que no se utilizan y están definidos, etc. En AppMarketPlace, hay un total de 77 issues en donde hay 6 que son críticos, 64 importantes, 0 blocker y 14 menores. 

####Bloquer:
Mirando estos datos de issues, hay un aspecto positivo y es que no hay ningún issue de tipo blocker que son los bugs con mayor probabilidad a hacer fallar el programa, por este lado estamos tranquilos. 
####Critical:
Tan sólo hay 6 issues críticos , estos tienen una probabilidad baja de afectar el comportamiento del sistema, estos issues son de manejo de excepciones en java ya que en algún evento podrían afectar la experiencia de los usuarios del AppMarketplace.Como grupo nos comprometemos a arreglar estos issues antes de empezar a desarrollar nuevos requerimientos.  
####Major:
Un aspecto importante a tener en cuenta es el que hay 64 issues de tipo importante, estos no afectan el rendimiento del sistema, pero si impactan la productividad de los desarrolladores que trabajen sobre este código, incluye aspectos duplicados, parámetros no utilizados, y código sin pruebas unitarias. En este aspecto hay que revisar si es posible hacer una revisión al código y hacer un refactoring para reducir este tipo de issues. 	


  

   
   
   

