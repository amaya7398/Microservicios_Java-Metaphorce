"Principios SOLID en Spring Boot"

Describir de manera clara cada uno de los princicpios SOLID.
Los principios pueden ser identificados dentro del framework de Spring Boot o dentro del código generado durante el curso.

Spring Boot, como framework de desarrollo de aplicaciones Java, promueve muchas de las mejores prácticas asociadas a los principios SOLID de forma implícita en su estructura y diseño...

:house: [INICIO](/README.md)

# S

### Principio de responsabilidad única (Single responsability principle)
  
Spring Boot fomenta la creación de clases y componentes con responsabilidades bien definidas.  
Por ejemplo:  
  
* Los controladores (Controllers) en Spring Boot se encargan de manejar las solicitudes HTTP y dirigirlas a las capas apropiadas.
* Los servicios (Services) se centran en la lógica de negocio.  
* Los repositorios (Repositories) se ocupan de la persitencia de datos.  
  
![Carpetas][imgCarpetas]  

[imgCarpetas]: /recursos/SOLID-S-folder.png

# O

### Principio de abierto/cerrado (Open/Closed principle)
  
Spring Boot se basa en la programación orientada a aspectos (AOP) y la inversión de control (IoC) para permitir  
la extensibilidad y la personalización sin modificar el código existente.
  
Mediante el uso de anotaciones como "@Configuration", "@Component", "@Data", entre otras, se pueden agregar funcionalidades adicionales,  
como la configuración de beans y la manipulación de aspectos, sin tener que modificar directamente las clases existentes.
  
![EnableEureka][img-O-1]  
![Configuration][img-O-2]  
![Data][img-O-3]  

[img-O-1]: /recursos/SOLID-O-1.png
[img-O-2]: /recursos/SOLID-O-2.png
[img-O-3]: /recursos/SOLID-O-3.png

# L

### Principio de sustitución de Liskov (Liskov substitution principle)
  
En Spring Boot, se hace uso extensivo de la herencia y la implementación de interfaces para garantizar la sustitución de objetos  
sin alterar el comportamiento esperado.  
Por ejemplo:  
  
* En el contexto de la inyección de dependencias, es común definir interfaces y utilizar la anotación "@Autowired"  
para inyectar implementaciones concretas.
  
Esto permite reemplazar fácilmente las implementaciones sin afectar el funcionamiento de las clases que dependen de ellas.  
  
![Autowired][img-L-1]  

[img-L-1]: /recursos/SOLID-L-autowired.png

# I

### Principio de segregación de interfaces (Interface segregation principle)
  
En Spring Boot se favorece la creación de interfaces cohesivass y específicas para cada funcionalidad.  
Por ejemplo:  
  
En lugar de tener una interfaz grande y genérica que contenga todos los métodos relacionados con una entidad, se pueden  
definir interfaces más pequeñass y especializadas que se ajusten a diferentes aspectos de la funcionalidad.  
Esto ayuda a evitar que las clases dependan de métodos que no necesitan y promueve la coherencia y modularidad del código.  
  
![img-I-1][img-I-1]  
![img-I-2][img-I-2]  
![img-I-3][img-I-3]  

[img-I-1]: /recursos/SOLID-I-1.png
[img-I-2]: /recursos/SOLID-I-2.png
[img-I-3]: /recursos/SOLID-I-3.png
  
* Un ejemplo fuera del bootcamp podría ser el siguiente: En el que se implementan las respectivas interfaces a usar  
  
![img-I-2][img-I-extra-1]  

[img-I-extra-1]: /recursos/SOLID-I-extra-1.png
# D

### Principio de inversión de dependencia (Dependency inversion principle)
  
En Spring Boot, se implementa el principio de inversión de dependencia a través del contenedor de inversión de control (IoC) y la inyección de dependencias.  
En lugar de que las clases creen directamente sus dependencias, Spring Boot se encarga de la creación y gestión de los objetos y los proporciona a través de la inyección de dependencias.  
  
Esto reduce el acoplamiento y permite una mayor flexibilidad al intercambiar implementaciones sin modificar las clases dependientes.

![img-D-1][img-D-1]  
![img-D-2][img-D-2]  
![img-D-3][img-D-3]  

[img-D-1]: /recursos/SOLID-D-1-clss.png
[img-D-2]: /recursos/SOLID-D-2-kxs.png
[img-D-3]: /recursos/SOLID-D-3-als.png

:house: [INICIO](/README.md)
