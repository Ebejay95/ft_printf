# ft_printf

**Custom implementation of the `printf` function in C.**

This project is a replica of the `printf` function from the C standard library that provides a deep understanding of formatted output, variadic functions and memory management.

## structure

### src/

The `src` folder contains the central source code files that implement the functionality of `ft_printf`. Each file is responsible for parsing and handling different format specifications:

- **ft_printf.c**: The main implementation of the `ft_printf` function. This file controls the formatting process and ensures that the different types are handled correctly.
- **ft_parser.c**: This file contains the logic to parse the format string and extract the appropriate flags, widths and precisions.
- **ft_handler_char.c**: Handles the output of characters (`%c`) and strings (`%s`).
- **ft_handler_int.c**: Handles the processing of integer values (`%d`, `%i`).
- **ft_handler_unsigned.c**: Implements the handling of unsigned integers (`%u`) as well as the conversion to hexadecimal numbers (`%x`, `%X`).
- **ft_utils.c**: Helper functions that are needed in several parts of the implementation, such as `ft_strlen`, `ft_itoa`, and similar.

### ft_printf.h

The header file contains the function prototypes and necessary macros to link the implementation in the different files.

### Makefile

The Makefile automates the build process, compiles the source code files and creates the static library `libftprintf.a`, which can be included in other projects.

## Features

- **Format specifications**: Supports basic format specifications such as `%c`, `%s`, `%d`, `%i`, `%u`, `%x`, `%X`, and `%%`.
- **Flags and precision**: Handles flags such as `-`, `0`, `#`, ` `, `+` and supports width and precision specifications.
- Memory management**: Implements optimized memory management for efficient output.

## Usage

To compile the project, use the following command:

```
make
```
