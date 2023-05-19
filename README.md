# Libft
## Your very first own library
Functions in the library:
| Function Name | Function Description                                     |
| ------------- | ------------------------------------------------------- |
| isalpha       | Checks if a character is an alphabetic character         |
| isdigit       | Checks if a character is a decimal digit                 |
| isalnum       | Checks if a character is an alphabetic or numeric digit  |
| isascii       | Checks if a character is an ASCII character              |
| isprint       | Checks if a character is a printable character           |
| strlen        | Calculates the length of a string                        |
| memset        | Fills a block of memory with a specified value           |
| bzero         | Sets a block of memory to zero                           |
| memcpy        | Copies a block of memory from one location to another    |
| memmove       | Copies a block of memory, handling overlapping regions   |
| strlcpy       | Safely copies a string into a fixed-size buffer          |
| strlcat       | Safely concatenates two strings into a fixed-size buffer |
| toupper       | Converts a character to uppercase                        |
| tolower       | Converts a character to lowercase                        |
| strchr        | Finds the first occurrence of a character in a string     |
| strrchr       | Finds the last occurrence of a character in a string      |
| strncmp       | Compares two strings up to a specified number of characters |
| memchr        | Searches a block of memory for a specific character      |
| memcmp        | Compares two blocks of memory                            |
| strnstr       | Searches for a substring within a string                 |
| atoi          | Converts a string to an integer                          |
| calloc        | Allocates and initializes a block of memory              |
| strdup        | Creates a duplicate of a string                          |

### Bonus

You must integrate the <code>t_list</code> struct into libft.h for the bonus to work, the struct is set to this values:
```
typedef struct s_list
{
void *content;
struct s_list *next;
} t_list;
```
Bonus functions:
| Function Name  | Function Description                                       |
| -------------- | --------------------------------------------------------- |
| ft_lstnew      | Allocates (with malloc(3)) and returns a new node.         |
| ft_lstadd_front| Adds the node ’new’ at the beginning of the list.          |
| ft_lstsize     | Counts the number of nodes in a list.                      |
| ft_lstlast     | Returns the last node of the list.                         |
| ft_lstadd_back | Adds the node ’new’ at the end of the list.                |
| ft_lstdelone   | Takes as a parameter a node and frees the memory of the    |
|                | node’s content using the function ’del’ given as a         |
|                | parameter and free the node. The memory of ’next’ must     |
|                | not be freed.                                              |
| ft_lstclear    | Deletes and frees the given node and every successor of     |
|                | that node, using the function ’del’ and free(3). Finally,  |
|                | the pointer to the list must be set to NULL.               |
| ft_lstiter     | Iterates the list ’lst’ and applies the function ’f’ on the |
|                | content of each node.                                      |
| ft_lstmap      | Iterates the list ’lst’ and applies the function ’f’ on the |
|                | content of each node. Creates a new list resulting of the  |
|                | successive applications of the function ’f’. The ’del’     |
|                | function is used to delete the content of a node if needed. |


# ft_printf
## Because ft_putnbr() and ft_putstr() aren't enough
You have to implement the following conversions:
- %c Prints a single character.
- %s Prints a string (as defined by the common C convention).
- %p The void * pointer argument has to be printed in hexadecimal format.
- %d Prints a decimal (base 10) number.
- %i Prints an integer in base 10.
- %u Prints an unsigned decimal (base 10) number.
- %x Prints a number in hexadecimal (base 16) lowercase format.
- %X Prints a number in hexadecimal (base 16) uppercase format.
- %% Prints a percent sign.

# get_next_line
## Reading a line from a fd is way too tedious
| Function name       | get_next_line                                               |
|---------------------|-------------------------------------------------------------|
| Prototype           | char \*get_next_line(int fd);                                 |
| Turn in files       | get_next_line.c, get_next_line_utils.c, get_next_line.h      |
| Parameters          | fd: The file descriptor to read from                         |
| Return value        | Read line: correct behavior                                  |
|                     | NULL: there is nothing else to read, or an error occurred    |
| External functs.    | read, malloc, free                                          |
| Description         | Write a function that returns a line read from a file descriptor |

