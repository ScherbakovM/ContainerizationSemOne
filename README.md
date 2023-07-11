# ContainerizationSemOne

Команды выполняюся от имени суперпользователя
### Смена корневой директории 


### Создаём папку для нашей новой корневой директории


``mkdir GB``

![image](https://github.com/ScherbakovM/ContainerizationSemOne/assets/109952823/4fc30aad-1fed-4225-8e0b-71b6212b1713)

### для новой директори нужно скопировать командную оболочку в нашу директорию  в данном случае bash 

### создаём для неё вложенную папку 

``mkdir GB/bin``

![image](https://github.com/ScherbakovM/ContainerizationSemOne/assets/109952823/7670abd1-af9f-4239-9fd9-f8341e2653b7)

### копируем в неё bash 

``cp /bin/bash GB/bin``

![image](https://github.com/ScherbakovM/ContainerizationSemOne/assets/109952823/8831fcfc-e95f-4612-bcc3-9683109efa54)

### далее для того чтобы bash работал в нашей новой корневой директории необходимо подгрузить для него все необходимые зависимости 

Список зависимостей можно вывести командой 

``ldd /bin/bash``

результат 

`` linux-vdso.so.1 (0x00007ffc34b62000)  
  libtinfo.so.6 => /lib/x86_64-linux-gnu/libtinfo.so.6 (0x00007f7a58157000)
  libc.so.6 => /lib/x86_64-linux-gnu/libc.so.6 (0x00007f7a57e00000)
  /lib64/ld-linux-x86-64.so.2 (0x00007f7a582fb000)``

 ![image](https://github.com/ScherbakovM/ContainerizationSemOne/assets/109952823/dfd2d7a7-62e4-4c88-9a8d-d9f220cea7d7)






