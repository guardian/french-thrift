French Thrift
=============

[Apache Thrift](https://github.com/apache/thrift) but without reserved keywords.
There is no need of them in an IDL.

Each compiler implementation should escape the reserved ones in their target language.

Only latest stable version, `0.9.3` is currently supported. 

How to build
=============

* OS X

Install depedencies and build tools

```shell
brew install libtool
brew install autoconf
brew install automake
brew install bison
brew link bison --force
brew install openssl
brew link openssl --force
```

Configure without the target you don't need, i.e

```shell
 $ ./configure --disable-debug --without-php --without-python --without-ruby --without-perl --without-cpp
```

Compile
```
$ make
```

Install (need super user)
```
# make install
```
