# ft_printf

**Because `ft_putnbr()` and `ft_putstr()` aren’t enough!**

## Summary

The **ft_printf** project focuses on replicating the behavior of the standard C library function `printf()`. Through this task, you'll learn about variadic functions, memory management, and formatting outputs in C. The end goal is to create a custom `ft_printf()` function, integrate it into your `libft`, and elevate your coding skills.

---

## Features

- **Supported Conversions**:
  - `%c`: Print a single character.
  - `%s`: Print a string.
  - `%p`: Print a pointer in hexadecimal format.
  - `%d`, `%i`: Print integers in base 10.
  - `%u`: Print unsigned integers in base 10.
  - `%x`, `%X`: Print integers in hexadecimal (lowercase/uppercase).
  - `%%`: Print a percent sign.
  
- **Bonus Features** (Optional):
  - Manage flags like `-0.` and minimum field width for all conversions.
  - Implement flags `# +` (including space).

- **Compatibility**:
  - Works seamlessly with `libft` projects.
  - Passes evaluation by Deepthought and peer-review systems.

---

## Project Structure

### Source Code

- **`src/`**: Contains the main implementation and modular files:
  - **`ft_printf.c`**: The main function implementing `ft_printf`.
  - **`ft_parser.c`**: Parses format strings and extracts flags, widths, and precisions.
  - **`ft_handler_char.c`**: Handles `%c` and `%s` conversions.
  - **`ft_handler_int.c`**: Manages `%d`, `%i` conversions.
  - **`ft_handler_unsigned.c`**: Handles `%u`, `%x`, `%X`.
  - **`ft_utils.c`**: Helper functions like `ft_strlen`, `ft_itoa`, etc.

- **`ft_printf.h`**: Contains function prototypes, macros, and shared definitions.

### Build System

- **Makefile**: Automates building and testing:
  - Targets: `NAME`, `all`, `clean`, `fclean`, `re`, and `bonus`.
  - Outputs `libftprintf.a`, a static library ready for integration.

---

## Installation and Usage

1. Clone the repository:
git clone <repository_url> cd ft_printf

markdown
Code kopieren

2. Build the library:
make

arduino
Code kopieren

3. Include libftprintf.a in your project and link it during compilation:
```
#include "ft_printf.h"

int main(void)
{
    ft_printf("Hello, World! %d\n", 42);
    return 0;
}
```

gcc main.c libftprintf.a -o my_program
Requirements and Rules
Language: C (Adheres to 42's Norm standards).
Mandatory External Functions: malloc, free, write, va_start, va_arg, va_copy, va_end.
Memory Management: No leaks allowed.
Bonus: Bonus features are assessed only after passing the mandatory part perfectly.
Submission: Submit via the assigned Git repository. Ensure all files are correctly named and structured.
Key Learning Outcomes
Deep dive into variadic functions.
Mastery of formatting and parsing techniques.
A solid understanding of memory allocation and management in C.
Building a reusable and robust library for future projects.
Once completed, your ft_printf() becomes a valuable addition to your libft arsenal!

ft_printf – because building it yourself is way cooler than using the default. 😉





