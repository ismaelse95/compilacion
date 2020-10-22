# Compilación de Python3 con Makefile

Para empezar a instalar Python3 lo primero que tendremos que hacer es instalar la dependencia que nos pedirá cuando hagamos la compilación en este caso es `zlib1g-dev`.

~~~
ismael@ismael:$ sudo install zliblg-dev
~~~

Pasamos a descargar el paquete con la extencion `.tar.xz` y cuando tengamos el paquete lo descomprimimos.

~~~
ismael@ismael:$ sudo tar -xf Python-3.9.0.tar.xz
~~~

Después crearemos el directorio en `/opt/`.

~~~
ismael@ismael:$ sudo mkdir /opt/Python3
~~~

Por último ejecutamos el configure y los dos comandos para instalar con make.

~~~
ismael@ismael:/opt/Python3$ ./configure
~~~

~~~
ismael@ismael:/opt/Python3$ make
~~~

~~~
ismael@ismael:/opt/Python3$ make install
~~~

Para desinstalar solo tendremos que ejecutar el siguiente comando.

~~~
ismael@ismael:/opt/Python3$ make uninstall
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
