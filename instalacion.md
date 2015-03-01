# Debian Wheezy i386


Guía de instalación [Instalación](https://www.debian.org/releases/stable/i386/) desde un CD [Debian Wheezy](http://cdimage.debian.org/debian-cd/7.8.0/i386/iso-cd/), se aconseja la arquitectura i386 para no tener problemas con las dependencias, después de actualizar cambiar los repositorios apuntando a la versión **testing** (*Jessie*). Esto lo podemos realizar desde el **sources.list** con el siguiente comando en una terminal:

`sudo nano /etc/apt/sources.list`

cambiando la parte del nombre **Wheezy** por el de **Jessie** o **testing**, en las siguientes líneas del archivo y aconsejable también añadir los **non-free** y **backports** como se ve en la siguiente captura:

![Sources.list](https://github.com/Makova/Android-Galicia/blob/master/imagenes/SourceList.png)

O desde **Synaptic**:

![Synaptic](https://github.com/Makova/Android-Galicia/blob/master/imagenes/synaptic.png)

He preferido utilizar Debian en la versión considerada como testing (Jessie) por disponer de paquetes y programas más actualizados que la rama stable (Wheezy), de esta manera nos aseguramos que las herramientas y programas para trabajar con emulación, cocina y Android studio será menos complicada.
También se podría haber utilizado Ubuntu 14.04 con un entorno más liviano como Gnome-classic o XFCE, pero Debian por algo es "papa" de Ubuntu y derivadas, teniendo mucha información y una gran comunidad detrás. El hecho de apuntar los repositorios de Debian Wheezy a la rama testing (Jessie) es como estar en la stable de Ubuntu 14.04, en lo que a actualizaciones se refiere.

# Java de Oracle

Yo siempre he instalado [Java de Oracle](http://www.oracle.com/technetwork/java/javase/downloads/index.html) desde la propia web, pero también se puede por repositorios de [Webupd8](http://www.webupd8.org/2012/01/install-oracle-java-jdk-7-in-ubuntu-via.html) o desde Synaptic los OpenJDK mantenidos por la comunidad.
Recomiendo la versión 7 de Java por no dar problemas en el desarrollo con Android. También especificar la monglatura de Java, JDK y JRE:

>+ JDK > "Java Development Kit" (Kit de desarrollo Java) > Versión para los desarrolladores. Incluye el compilador de Java (javac), JRE y JVM.

>+ JRE > "Java Runtime Environment" (Entorno de ejecución Java) > Versión para los usuarios. Conjunto de utilidades de Java, que actúa como un "intermediario" entre el sistema operativo y Java. Incluye JVM.

>+ JVM > "Java Virtual Machine" (Máquina Virtual de Java) > Programa que ejecuta el código Java previamente compilado (bytecode) mientras que las librerías de clase estándar son las que implementan el API de Java. Ambas JVM y API deben ser consistentes entre sí, de ahí que sean distribuidas de modo conjunto.



