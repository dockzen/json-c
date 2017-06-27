# dockzen uses V0.12
$ git checkout json-c-0.12

# build instructions (amd64)
    $ sh autogen.sh  
    $ ac_cv_func_malloc_0_nonnull=yes ac_cv_func_realloc_0_nonnull=yes ./configure --prefix=${PWD}/install --exec-prefix=${PWD}/install/amd64  
    $ make clean  
    $ make  
    $ make install  

# build instructions (arm)  
    $ sh autogen.sh  
    $ ac_cv_func_malloc_0_nonnull=yes ac_cv_func_realloc_0_nonnull=yes ./configure --prefix=${PWD}/install --exec-prefix=${PWD}/install/arm --build=x86_64-linux --host=arm-linux-gnueabi CC=arm-linux-gnueabi-gcc-4.7  
    $ make clean  
    $ make  
    $ make install
  

# output

> install/  
> ├── amd64  
> │   └── lib  
> │       ├── libjson-c.a  
> │       ├── libjson-c.la  
> │       ├── libjson-c.so -libjson-c.so.2.0.2  
> │       ├── libjson-c.so.2 -libjson-c.so.2.0.2  
> │       ├── libjson-c.so.2.0.2  
> │       └── pkgconfig  
> │           └── json-c.pc  
> ├── arm  
> │   └── lib  
> │       ├── libjson-c.a  
> │       ├── libjson-c.la  
> │       ├── libjson-c.so -libjson-c.so.2.0.2  
> │       ├── libjson-c.so.2 -libjson-c.so.2.0.2  
> │       ├── libjson-c.so.2.0.2  
> │       └── pkgconfig  
> │           └── json-c.pc  
> └── include  
>     └── json-c  
>         ├── arraylist.h  
>         ├── bits.h  
>         ├── debug.h  
>         ├── json_config.h  
>         ├── json_c_version.h  
>         ├── json.h  
>         ├── json_inttypes.h  
>         ├── json_object.h  
>         ├── json_object_iterator.h  
>         ├── json_object_private.h  
>         ├── json_tokener.h  
>         ├── json_util.h  
>         ├── linkhash.h  
>         ├── printbuf.h  
>         └── random_seed.h  
