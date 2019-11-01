# GCC ver detalles de compilacion
~~~
$ gcc -v -###
~~~

# Descargar gcc del sitio oficial
~~~
$ curl -LO https://gcc.gnu.org/pub/gcc/releases/gcc-9.2.0/gcc-9.2.0.tar.xz
~~~

# DOC CONFIGURE
~~~
$ https://gcc.gnu.org/install/configure.html
~~~

# PARA AVR USAREMOS
~~~
 --target=avr  la plataforma a la que va dirigido.
 --disable-nls para soportar compilacion cruzada.
 --enable-languages=c,c++
~~~

# COMPILAR avr-gcc
~~~
$ tar xvf gcc-9.2.0.tar.xz
$ cd gcc-9.2.0
$ mkdir build
$ cd build
$ ../configure --target=avr --disable-nls --enable-languages=c,c++
$ make -j4
$ make install
~~~
