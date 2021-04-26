# Juliana-Giraldo-SabanaResearch

## CONCEPTOS

1. ¿Qué es encapsulamiento? ¿Qué ventajas ofrece?

RTA/ El encapsulamiento es un principio muy utlizado en Java y además una buena práctica de programación que consiste en limitar el acceso a las clases que hemos creado previamente para asi tener un mayor control sobre ellas, es decir, este principio hace que los atributos de las clases se puedan editar sólo a través de métodos. De manera general, se hace teniendo las propiedades como privadas y métodos que la controlan públicos. Estos métodos que nos permiten interactuar con los atributos de una clase se llaman métdos de acceso, también conocidos como getters y setters. Los setters se utilizan para definir los atributos de la clase, mientras que los getters se utilizan para poder acceder a estos atriutos, como si fueran una llave de acceso. 

El encapsulamiento tiene bastantes ventajas, pero las principales son: mantenibilidad, estabilidad y seguridad. El encapsulamiento nos asegura que estas caracteristicas se cumplan ya que al restringir el acceso a los atributos de una clase nos asegura que no cambiaran a  lo largo del tiempo por un agente externo generando una alteración a nuestro código, es decir, hace que nuestro código se mantenga con el tiempo y que ningún programador o persona externa pueda cambiar dichos atributos. La función principal del encapsulamiento es precisamente esa: limitar las interacciones de otra persona con nuestro código, y solo darle acceso a las cosas que con las que podra interactuar sin alterar el código interno que hace funcionar el programa o los atributos ya predefinidos por así decirlo.

2. ¿Qué es ocultación de información? ¿Por qué aplicarla? ¿Cómo se implementa en Java?

RTA/ La ocultación de la información, como su nombre lo indica, se encarga de esconder o hacer inaccesible datos o procesos a otras estructuras; pueden ser a otras clases, paquetes, etc. Esto con el objetivo de estas entidades comuniquen entre ellas solo la información importante o esencial. Es como si fueran entidades independientes que solo se transmiten entre sí la información que nosotros consideremos necesaria. Esta práctica se aplica principalmente para facilitar las pruebas, el manejo y las modificaciones que requiera el software. Se puede decir que la ocultación de información sirve como un criterio eficaz para dividir cualquier pieza del software en modulos de funcionalidad o interfaces, una independiente de la otra pero a la misma vez relacionadas. 

La ocultación de información se implementa en Java mediante tres niveles de acceso, los cuales son: Público (Public); Todos pueden acceder a los datos o métodos de una clase que se definen con este nivel, este es el nivel más bajo, esto es lo que tu quieres que la parte externa vea. Protegido (Protected); Podemos decir que estás no son de acceso público, solamente son accesibles dentro de su clase y por subclases y Privado (Private); En este nivel se puede declarar miembros accesibles sólo para la propia clase. Por último se imlemnetan los métodos getters y setters mencionados anteriormente.

3. ¿Cuáles son las acciones los tres momentos importantes de las excepciones? ¿Cuál es el objetivo de cada una? ¿Cómo se implementa en Java cada acción?

RTA/ Las tres momentos importantes de las excepciones son el try, el catch y el finally. El objetivo principal del try es capturar el error si se produce para posteriormente corregirlo, es decir, captura el código en el cual una posible excepción puede aparecer. Luego, el catch se encarga de definir el conjunto de instrucciones necesarias o de tratamiento del problema capturado con el bloque try anterior. Y por último, el finally se encarga de definir un conjunto de instrucciones necesarias tanto si se produce error o excepción como si no y que por tanto se ejecuta siempre.

Los tres momnetos de las excepciones se implementan de la siguiente forma:

 try{
    //Código que puede provocar errores
 }
 
 catch (Exception e) {
    //gestión del error e tipo Exception
}

finally {
    //código de finally
}


4. ¿Qué es sobre-escritura de métodos? ¿Por qué aplicarla? ¿Cómo impedir que se sobre-escriba un método?

RTA/ La sobre-escritura de métodos u override es una caracteristica que le permite a una subclase proporcionar una implementación especifica de un método que ya está provisto por una de sus superclases o clase padre. El override es muy útil cuando queremos que un método que ya existe se comporte de una manera diferente o especifica de acuerdo al contexto de un programa, también es muy útil a la hora de trabajar clases abstractas e interfaces. 

Para impedir que se sobre-escriba un método solo basta con hacer ese método final, y ya con esto ninguna clase podra hacer override de ese método. Por ejemplo:

public final String nombreMetodo();

## MAPA DE MEMORIA

![image](https://user-images.githubusercontent.com/78317998/115974662-cc012e80-a523-11eb-87d1-fa9897c8f14d.png)

## IMPLEMENTACIÓN

1. Pruebas SabanaReasearchTest parcial 1

![image](https://user-images.githubusercontent.com/78317998/116023093-1f04df80-a611-11eb-8c81-4e9443a49836.png)

2. Pruebas BonoTest parcial 1

![image](https://user-images.githubusercontent.com/78317998/116023238-5d020380-a611-11eb-81d9-1b02fc68ca57.png)

3. Pruebas ProjectTest parcial 2

![image](https://user-images.githubusercontent.com/78317998/116023328-8458d080-a611-11eb-93a4-fb8fdcadab2f.png)

4. Pruebas BonoTest parcial 2

![image](https://user-images.githubusercontent.com/78317998/116023474-c4b84e80-a611-11eb-95f6-6cdf6fde6b21.png)


## DISEÑO

![image](https://user-images.githubusercontent.com/78317998/116015211-1ce55580-a5fe-11eb-9206-eab5bf96bcd3.png)



1. Método summarize()

/**
   * Resume la informacion del tiempo invertido de un estudiante en un proyecto o la duración de cada iteración en un proyecto.
   *
   * @return la duración de un estudiante o iteración en un  proyecto.

 */

2. Diagramas de secuencia

![image](https://user-images.githubusercontent.com/78317998/115964705-58432f80-a4eb-11eb-92b3-a263dcbe984d.png)


![image](https://user-images.githubusercontent.com/78317998/115965017-c3d9cc80-a4ec-11eb-855f-874d2b1fb485.png)


3. Diagrama de clases actualizado

![image](https://user-images.githubusercontent.com/78317998/115966646-3601df80-a4f4-11eb-9c14-f694e1713b78.png)


4. Método synthetize()

/**
   * Resume la informacion de un estudiante o de una iteración dentro de un proyecto.
   *
   * @return la duración de un estudiante o iteración en un  proyecto.

 */
 
 Método getActivitiesDuration()
 
 /**
   * Calcula la duración de las actividades de un estudiante o iteracion en un proyecto.
   *
   * @return la duración de las actividades de un estudiante o iteración en un  proyecto.

 */

## EXTENDIENDO

![image](https://user-images.githubusercontent.com/78317998/115973099-3613d680-a518-11eb-973d-4f5a1a11c3bd.png)

De los diseños resultantes del punto I y II, ¿Qué debe cambiar? ¿Qué no debe cambiar?

RTA/ En cuanto a los diagramas de secuencia del punto anterior lo que deberia cambiar es la forma de calcular la duración de una actividad o iteración, ya que ahora al tener prerequisitos se debe aplicar un condicional que indique si esa actividad o iteración tiene algun prerequisito, y en el caso de que esto sea cierto se deberia recurrir al método getEstimatedEndDate(), ya sea de una actividad o iteración para así modificar o "actualizar" la duración de dicha clase. Por el contrario, lo que no deberia cambiar son los métodos summarize() y synthetize(), ya que independientemente de como se obtenga la duración de la iteración o proyecto estos métodos llamaran al método que genere la duración mediante un loop.

Por otro lado, el diagrama de clases del punto anterior lo que deberia cambiar, o mejor dicho adicionar, es una clase abstracta que se refiera a la dependencia o prerequisito ya sea de una actividad o de una iteración y que esta a su vez tenga un método abstracto llamado "getEstimatedEndDate()" que retorne la fecha de finalización estimada para dicha actividad o iteración, también se de debe añadir una relación de uno a varios entre la clase iteración y la clase abstracta dependencia, dando a entender que una iteración puede tener muchas dependencias. Por último, lo que no deberia cambiar del diagrama de clases son las demás clases involucradas que no tienen ninguna relación directa con la clase abstracta dependencia, como por ejemplo: Student, Project y la interfaz ISynthetizer.

Teniendo en cuenta los cambios necesarios ¿Que fue bueno y que fue malo de su diseño?

RTA/ Considero que en general los diagramas de secuencia y el complemento del diagrama de clases fue pertinente para este proyecto de sabana research debido a que es una buena guia para basarse al momento de realizar el código, y aunque haya necesitado algunos cambios, estos se pudieron integrar con facilidad a los diseños ya establecidos sin tener que cambiar todo el diseño. Sin embargo, considero también que el diseño pudo haber sido mejor si por ejemplo se implementara una interfaz que abstrayera la duración de las actividades para las clases Activity e Iteration y que estas no repetieran el método getActivitiesDuratio(), entre otros cambios que podrían mejorar un poco más el código.
