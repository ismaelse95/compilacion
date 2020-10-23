# Compilación de Python3 con Makefile

Para empezar a compilar el programa lo primero que tendremos que hacer es descargar el paquete python3 en la versión 3.7.3 que es la versión stable de debian 10 y despues pasamos a descomprimirlo.

~~~
ismael@ismael:$ sudo tar -xf Python-3.7.3.tar.xz
~~~

Después crearemos el directorio en `/opt/`.

~~~
ismael@ismael:/opt$ sudo mkdir Python3
~~~

Ahora para seguir con la compilación vamos a mirar en el fichero README para ver que pasos hay que seguir y en esa ayuda nos pone lo siguiente.

~~~
On Unix, Linux, BSD, macOS, and Cygwin::

    ./configure
    make
    make test
    sudo make install
~~~

Por último ejecutamos el configure y los dos comandos para instalar con make como nos dice en el README.

~~~
ismael@ismael:/opt/Python3$ sudo ./configure
~~~

~~~
ismael@ismael:/opt/Python3$ sudo make
~~~

~~~
ismael@ismael:/opt/Python3$ sudo make install
~~~

Al ejecutar `make install` nos saldrá el error que le falta el paquete `zlib1g-dev` para solucionar este fallo lo instalamos y hacemos de nuevo el `make install`.

~~~
ismael@ismael:$ sudo apt install zlib1g-dev
~~~

# Compilación de Nano con Makefile

Para empezar a instalar Python3 lo primero que tendremos que hacer es instalar la dependencia que nos pedirá cuando hagamos la compilación en este caso es `libncursesw5-dev`.

~~~
ismael@ismael:$ sudo install libncursesw5-dev
~~~

Pasamos a descargar el paquete con la extencion `.tar.xz` y cuando tengamos el paquete lo descomprimimos.

~~~
ismael@ismael:$ sudo tar -xf nano-5.3.tar.xz
~~~

Después crearemos el directorio en `/opt/`.

~~~
ismael@ismael:$ sudo mkdir /opt/nano
~~~

Por último ejecutamos el configure y los dos comandos para instalar con make.

~~~
ismael@ismael:/opt/nano$ ./configure
~~~

~~~
ismael@ismael:/opt/nano$ make
~~~

~~~
ismael@ismael:/opt/nano$ make install
~~~

Para desinstalar solo tendremos que ejecutar el siguiente comando.

~~~
ismael@ismael:/opt/nano$ make uninstall
~~~
