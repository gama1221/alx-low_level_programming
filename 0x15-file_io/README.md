# Welcome to ALX Low Level Programming
## 0x15. C - File I/O
### Tasks
0. [Tread lightly, she is near](https://github.com/gama1221/alx-low_level_programming/tree/main/0x15-file_io/0-read_textfile.c)
        - Write a function that reads a text file and prints it to the POSIX standard output.
                - Prototype: ssize_t read_textfile(const char *filename, size_t letters);
                - where letters is the number of letters it should read and print
                - returns the actual number of letters it could read and print
                - if the file can not be opened or read, return 0
                - if filename is NULL return 0
                - if write fails or does not write the expected amount of bytes, return 0
1. [Under the snow](https://github.com/gama1221/alx-low_level_programming/tree/main/0x15-file_io/1-print_binary.c)
        - Create a function that creates a file.
                - Prototype: int create_file(const char *filename, char *text_content);
                - where filename is the name of the file to create and text_content is a NULL terminated string to write to the file
                - Returns: 1 on success, -1 on failure (file can not be created, file can not be written, write “fails”, etc…)
                - The created file must have those permissions: rw-------. If the file already exists, do not change the permissions.
                - if the file already exists, truncate it
                - if filename is NULL return -1
                - if text_content is NULL create an empty file
2. [Speak gently, she can hear](https://github.com/gama1221/alx-low_level_programming/tree/main/0x15-file_io/2-append_text_to_file.c)
        - Create a function that creates a file.
                - Prototype: int create_file(const char *filename, char *text_content);
                - where filename is the name of the file to create and text_content is a NULL terminated string to write to the file
                - Returns: 1 on success, -1 on failure (file can not be created, file can not be written, write “fails”, etc…)
                - The created file must have those permissions: rw-------. If the file already exists, do not change the permissions.
                - if the file already exists, truncate it
                - if filename is NULL return -1
                - if text_content is NULL create an empty file
3. [cp](https://github.com/gama1221/alx-low_level_programming/tree/main/0x15-file_io/3-cp.c)
        - Write a program that copies the content of a file to another file.
                - Usage: cp file_from file_to
                - if the number of argument is not the correct one, exit with code 97 and print Usage: cp file_from file_to, followed by a new line, on the POSIX standard error
                - if file_to already exists, truncate it
                - if file_from does not exist, or if you can not read it, exit with code 98 and print Error: Can't read from file NAME_OF_THE_FILE, followed by a new line, on the POSIX standard error
                - where NAME_OF_THE_FILE is the first argument passed to your program
                - if you can not create or if write to file_to fails, exit with code 99 and print Error: Can't write to NAME_OF_THE_FILE, followed by a new line, on the POSIX standard error
                - where NAME_OF_THE_FILE is the second argument passed to your program
                - if you can not close a file descriptor , exit with code 100 and print Error: Can't close fd FD_VALUE, followed by a new line, on the POSIX standard error
                - where FD_VALUE is the value of the file descriptor
                - Permissions of the created file: rw-rw-r--. If the file already exists, do not change the permissions
                - You must read 1,024 bytes at a time from the file_from to make less system calls. Use a buffer
                - You are allowed to use dprintf
4. [elf](https://github.com/gama1221/alx-low_level_programming/tree/main/0x15-file_io/100-elf_header.c)
        - Write a program that displays the information contained in the ELF header at the start of an ELF file.
                - Usage: elf_header elf_filename
                - Displayed information: (no less, no more, do not include trailing whitespace)
                - Magic
                - Class
                - Data
                - Version
                - OS/ABI
                - ABI Version
                - Type
                - Entry point address
                - Format: the same as readelf -h (version 2.26.1)
                - If the file is not an ELF file, or on error, exit with status code 98 and display a comprehensive error message to stderr
                - You are allowed to use lseek once
                - You are allowed to use read a maximum of 2 times at runtime
                - You are allowed to have as many functions as you want in your source file
                - You are allowed to use printf
## Author
1. [WhatsApp](https://wa.me/+251991732949)
2. [Telegram](https://t.me/gama2112)