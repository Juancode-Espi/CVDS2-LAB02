# LAB02 AMAYA-ESPINOSA
## LA HERRAMIENTA MAVEN 

### Dentro de las utilidades de Maven encontramos:

+ Compilación de código
+ Empaquetado
+ Facilidad en el proceso de desarrollo
+ Promueve buenas practicas de desarrollo
+ Provee muchos projectos de ayuda y vive en constante actualización

### Fases de Maven:

1. validar: se valida que el proyecto es correcto y que toda la información necesaria está disponible.
2. compilar: compilar el código fuente del proyecto.
3. probar: testear el código compilado usando un marco de prueba unitario adecuado.\
	Estos tests no deberían necesitar que el codigo esté empacado.
4. empacar: tomar el código compilado y empacarlo en un formato distribuible como un JAR.
5. test de integración: procesar e implementar el paquete si es necesario en un entorno donde se puedan ejecutar pruebas de integración.
6. verificar: ejecutar cualquier verificación para verificar que el paquete sea válido y cumpla con los criterios de calidad
7. instalar: instala el paquete en el repositorio local, para usarlo como dependencia en otros proyectos localmente.
8. desplegar: hecho en un entorno de integración o lanzamiento, copia el paquete final en el repositorio remoto para compartirlo con otros desarrolladores y proyectos.
9. limpiar: limpia los artefactos creados por compilaciones anteriores.
10. sitio: genera documentación del sitio para este proyecto.

### Ciclo de vida de la construcción:

**Hay tres ciclos de vida de compilación integrados:** predeterminado, limpio y de sitio.\
El defaultciclo de vida maneja la implementación del proyecto, el cleanciclo de vida maneja\
la limpieza del proyecto, mientras que el siteciclo de vida maneja la creación de la\
documentación del sitio de su proyecto.

### Utilidad de los Plugins:

Los plugins son la característica central de Maven que permiten la reutilización de la lógica de compilación común en múltiples proyectos.\
Los plugins se utilizan para: crear archivos jar, crear archivos war, compilar código, código de prueba unitaria, crear documentación de proyecto, etc.
 
### Qué es y para que sirve el repositorio central de Maven:

El repositorio central de Maven es un sitio web donde se guardan todos los archivos Java. Puede buscar los jars que necesita allí.Cuando busque\
los archivos jar necesarios, puede incluir los archivos jar usando pom.xml o descargar directamente los archivos jar y agregarlos a su proyecto java.

## COMPILAR Y EJECUTAR:


### Objetivo del parámetro 'package':

** parámetro package:** construye el proyecto y empaqueta el JAR resultante dentro del directorio *target*\
`mvn package -Dmaven.test.skip=true` este comando hace lo mismo que `mvn package` con diferencia que omite las pruebas de unidad.

### Ejecución en maven:

`mvn exec:java -Dexec.mainClass="com.example.Main" [-Dexec.args="argument1"]"`

## HACER EL ESQUELETO DE LA APLICACION

### ¿Cuál(les) de las anteriores instrucciones se ejecutan y funcionan correctamente y por qué?

+ ***Sin parámetros***  nos dice que requerimos de un parámetro de tipo *RegularShapeType*.
+ ***Parámetro:qwerty***  nos dice que 'qwerty' no es un *RegularShapeType* válido.
+ ***Parámetro:pentagon***  nos dice que 'pentagon' no es un *RegularShapeType* válido.
+ ***Parámetro:Hexagon***  nos dice que se creo un 'Hexagon' de 6 lados exitosamente.




