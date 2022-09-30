# Welcome to ALX Low Level Programming
##  0x09. C - Static libraries
### Tasks
0. [A library is not a luxury but one of the necessities of life](https://github.com/gama1221/alx-low_level_programming/tree/main/0x09-static_libraries/libmy.a)
	- Create the static library libmy.a containing all the functions listed below:
        - If you haven’t coded all of the above functions create empty ones with the right prototype.
        - Don’t forget to push your main.h file to your repository. It should at least contain all the prototypes of the above functions.
```c++
    julien@ubuntu:~/0x09. Static Librairies$ ar -t libmy.a 
    0-isupper.o
    0-memset.o
    0-strcat.o
    1-isdigit.o
    1-memcpy.o
    1-strncat.o
    100-atoi.o
    2-strchr.o
    2-strlen.o
    2-strncpy.o
    3-islower.o
    3-puts.o
    3-strcmp.o
    3-strspn.o
    4-isalpha.o
    4-strpbrk.o
    5-strstr.o
    6-abs.o
    9-strcpy.o
    _putchar.o
    julien@ubuntu:~/0x09. Static Librairies$ nm libmy.a 

    0-isupper.o:
    0000000000000000 T _isupper

    0-memset.o:
    0000000000000000 T _memset

    0-strcat.o:
    0000000000000000 T _strcat

    1-isdigit.o:
    0000000000000000 T _isdigit

    1-memcpy.o:
    0000000000000000 T _memcpy

    1-strncat.o:
    0000000000000000 T _strncat

    100-atoi.o:
    0000000000000000 T _atoi

    2-strchr.o:
    0000000000000000 T _strchr

    2-strlen.o:
    0000000000000000 T _strlen

    2-strncpy.o:
    0000000000000000 T _strncpy

    3-islower.o:
    0000000000000000 T _islower

    3-puts.o:
                    U _putchar
    0000000000000000 T _puts

    3-strcmp.o:
    0000000000000000 T _strcmp

    3-strspn.o:
    0000000000000000 T _strspn

    4-isalpha.o:
    0000000000000000 T _isalpha

    4-strpbrk.o:
    0000000000000000 T _strpbrk

    5-strstr.o:
    0000000000000000 T _strstr

    6-abs.o:
    0000000000000000 T _abs

    9-strcpy.o:
    0000000000000000 T _strcpy

    _putchar.o:
    0000000000000000 T _putchar
                    U write
    julien@ubuntu:~/0x09. Static Librairies$ cat main.c 
    #include "main.h"

    int main(void)
    {
        _puts("\"At the end of the day, my goal was to be the best hacker\"\n\t- Kevin Mitnick");
        return (0);
    }
    julien@ubuntu:~/0x09. Static Librairies$ gcc -std=gnu89 main.c -L. -lmy -o quote
    julien@ubuntu:~/0x09. Static Librairies$ ./quote 
    "At the end of the day, my goal was to be the best hacker"
        - Kevin Mitnick
    julien@ubuntu:~/0x09. Static Librairies$
```
1. [Without libraries what have we? We have no past and no future](https://github.com/gama1221/alx-low_level_programming/tree/main/0x09-static_libraries/create_static_lib.sh)
	- Create a script called create_static_lib.sh that creates a static library called liball.a from all the .c files that are in the current directory.
```c++
    julien@ubuntu:~/0x09. Static Librairies$ ls *.c
    0-isupper.c  0-strcat.c  1-isdigit.c  1-strncat.c  2-strlen.c   3-islower.c  3-strcmp.c  4-isalpha.c  5-strstr.c  9-strcpy.c  _putchar.c
    0-memset.c   100-atoi.c  1-memcpy.c   2-strchr.c   2-strncpy.c  3-puts.c     3-strspn.c  4-strpbrk.c  6-abs.c
    julien@ubuntu:~/0x09. Static Librairies$ ./create_static_lib.sh 
    julien@ubuntu:~/0x09. Static Librairies$ ls *.a
    liball.a
    julien@ubuntu:~/0x09. Static Librairies$ ar -t liball.a
    0-isupper.o
    0-memset.o
    0-strcat.o
    100-atoi.o
    1-isdigit.o
    1-memcpy.o
    1-strncat.o
    2-strchr.o
    2-strlen.o
    2-strncpy.o
    3-islower.o
    3-puts.o
    3-strcmp.o
    3-strspn.o
    4-isalpha.o
    4-strpbrk.o
    5-strstr.o
    6-abs.o
    9-strcpy.o
    _putchar.o
    julien@ubuntu:~/0x09. Static Librairies$ 
```
## Author
1. [WhatsApp](https://wa.me/+251991732949)
2. [Telegram](https://t.me/gama2112)