# CVDS LABORATORIO 3 PBT
## Integrantes  
  - DIEGO ALEJANDRO GONZALEZ GUALTEROS
  - CRISTIAN ANDRES CASTELLANOS FINO  
## CLASES DE EQUIVALENCIAS  
### CREAR UN PROYECTO CON MAVEN
  Para crear un proyecto en maven seguimos la estructura descrita en la parte de abajo. Para este laboratorio se nos dan los siguientes datos.  
  - Grupo: edu.eci.cvds
  - Artefacto: ClasesEquivalencia
  - Paquete: edu.eci.cvds.tdd
  - archetypeArtifactId: maven-archetype-quickstart
  Luego el codigo para crear el repositorio maven seria
  ```
  mvn archetype:generate -DgroupId=edu.eci.cvds -DartifactId=ClasesEquivalencias -Dpackage=edu.eci.cvds.tdd 
    -DarchetypeArtifactId=maven-archetype-quickstar
 ``` 
 ### ACTUALIZAR Y CREAR DEPENDENCIAS EN EL PROYECTO  
  Para este paso lo primero que hearemos sera instalar la extension de JUnit en el proyecto maven, para esto buscamos en [JUnit](https://mvnrepository.com/search?q=JUnit) el programa, le damos click al que queramos, elegimos la version que deseemos, y copiamos el codigo que nos presenta para maven.
  ``` 
<dependency>
    <groupId>org.junit.jupiter</groupId>
    <artifactId>junit-jupiter-api</artifactId>
    <version>5.8.0-RC1</version>
    <scope>test</scope>
</dependecy>
  ```
  Agregamos este codigo en el archivo _pom.xml_ en la seccion de dependencias, con esto habremos instalado JUnit en nuestro proyecto.
### COMPILAR Y EJECUTAR
  Para compilar un proyecto en maven usamos el comando ```mvn compile ```
  Se queremos ejecutar pruebas unitarias hacemos uso del comando ```mvn test```
## EJERCICIO "REGISTRADURIA"
### EJECUTAR LAS PRUEBAS
  ¿Cual es la diferencia entre ```mvn test``` y ``` mvn pakage```? .  
  Su diferencia es que ```mvn test``` compila y ejecuta el proyecto con sus respectivas pruebas, en cambio ```mvn package ``` compila el programa, pasa las pruebas y si este las pasa, el programa empaqueta el proyecto en un archivo ```.jar ```
## FINALIZAR EL EJERCICIO
  Para este ejercicio podemos hacer uso de cinco casos de equivalencia. En caso que la persona no este viva, en caso que la persona sea menor de edad, en caso que la edad de la persona sea invalida, en caso que el numeor de cedula de la persona este duplicado, en caso que la informacion ingresada sea correcta.

