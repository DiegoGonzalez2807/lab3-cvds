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
  mvn archetype:generate -DgroupId=edu.eci.cvds -DartifactId=<Nombre> -Dpackage=edu.eci.cvds.<Nombre> -DarchetypeArtifactId=maven-archetype-quickstar

 ``` 
