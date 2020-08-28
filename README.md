# apba-servicemix-archetype

### Introducción

Arquetipo Maven para crear bundles de integración a desplegar sobre [Apache ServiceMix 6.0.0](http://servicemix.apache.org/downloads/servicemix-6.0.0.html)

Contiene una plantilla con una estructura básica de proyectos y código de ejemplo elemental, que muestra mejores prácticas a seguir.

Está basado en los bundles de ejemplo [aismanager-sample-bundles](https://github.com/adtapba/aismanager-sample-bundles)

### Uso

Comando [Maven](http://maven.apache.org/):
```
mvn archetype:generate -B -DarchetypeGroupId=es.apba.infra.esb \
                          -DarchetypeArtifactId=servicemix-archetype \
                          -DarchetypeVersion=[Versión arquetipo] \
                          -DgroupId=es.apba.infra.esb.[Código sistema minúsculas] \
                          -DartifactId=[Código sistema minúsculas] \
                          -Dversion=1.0.0-SNAPSHOT \
                          -DsystemCodeCamelCase=[Código sistema Camel Case]
```
Ejemplo:
```
mvn archetype:generate -B -DarchetypeGroupId=es.apba.infra.esb \
                          -DarchetypeArtifactId=servicemix-archetype \
                          -DarchetypeVersion=1.0.0 \
                          -DgroupId=es.apba.infra.esb.nuevosistema \
                          -DartifactId=nuevosistema \
                          -Dversion=1.0.0-SNAPSHOT \
                          -DsystemCodeCamelCase=nuevoSistema
```
