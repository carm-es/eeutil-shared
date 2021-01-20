# mvn-repo

Repositorio de librerias externas (no publicadas en maven-central) necesarias para compilar los módulos de EEUTILS. 

Para que el Maven de su aplicación pueda descargarlas deberá **hacer referencia a la rama mvn-repo desde el pom.xml** de su proyecto EEUTIL. 

También es posible instalar la librerías externas en su repositorio local de Maven. Debe descargar esta rama y ejecutar los siguientes comandos, sustituyendo ``{{ruta_a_jar}}`` por la ruta a los ficheros jar descargados *(no recomendamos esta opción)*:

```sh
mvn install:install-file -Dfile={{ruta_a_jar}}/miniapplet-full_1_5.jar -DgroupId=es.gob.afirma -DartifactId=miniapplet-afirma -Dversion=5.0 -Dpackaging=jar
mvn install:install-file -Dfile={{ruta_a_jar}}/vistaDocumentoIGAE-3.0.23.jar -DgroupId=es.igae -DartifactId=vistaDocumentoIGAE -Dversion=3.0.23 -Dpackaging=jar 
mvn install:install-file -Dfile={{ruta_a_jar}}/jodconverter-2.2.2.jar -DgroupId=com.artofsolving -DartifactId=jodconverter -Dversion=2.2.2 -Dpackaging=jar
mvn install:install-file -Dfile={{ruta_a_jar}}/jodconverter-cli-2.2.2.jar -DgroupId=com.artofsolving -DartifactId=jodconverter-cli -Dversion=2.2.2 -Dpackaging=jar
mvn install:install-file -Dfile={{ruta_a_jar}}/jodconverter-core-3.0-beta-4-jahia2.jar -DgroupId=com.artofsolving -DartifactId=jodconverter-core -Dversion=3.0-beta-4-jahia2 -Dpackaging=jar
mvn install:install-file -Dfile={{ruta_a_jar}}/POLA.jar -DgroupId=com.pdfTools -DartifactId=pDFOptimizer-windows -Dversion=4.8 -Dpackaging=jar
mvn install:install-file -Dfile={{ruta_a_jar}}/POLA.jar -DgroupId=com.pdfTools -DartifactId=pDFOptimizer-linux -Dversion=4.8 -Dpackaging=jar
mvn install:install-file -Dfile={{ruta_a_jar}}/eeutil-csvstoragews-stub-1.2.jar -DgroupId=es.mpt.dsic -DartifactId=eeutil-csvstoragews-stub -Dversion=1.2 -Dpackaging=jar
mvn install:install-file -Dfile={{ruta_a_jar}}/eeutil-csvbroker-stub-1.2.jar -DgroupId=es.mpt.dsic -DartifactId=eeutil-csvbroker-stub -Dversion=1.2 -Dpackaging=jar
```

