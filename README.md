# ft_printf

int ft_printf(char *str, ... );

This is a small implementation of the C's printf function, based on MAC implementation (e.g, it prints '(NULL)' for an string that is a null pointer instead of '(nil)').

ft_printf will read each character until it finds a '%', then it will replace the substring that starts in '%' and ends in the next specification, to another substring that is the product of the formatting rules.

Every specification should be matched by an argument after the input string. If there are not enough arguments, the behaviour is undefined. If there's too many arguments, the extra arguments will be ignored.

When no specification is found, the substring is replaced by an empty string. 

ft_printf will return the length of the string printed, or -1 in case of error.

## Specifications

- %c - A character
- %s - A string
- %p - A pointer's address printed in hexadecimal
- %d - An INT printed in base 10
- %i - An INT printed in base 10
- %u - An UNSIGNED INT printed in base 10
- %x - A hexadecimal number in lowercase
- %X - A hexadecimal number in uppercase
- %% - The % character

## Format

#### width

The substring will be at leeast of width size. By default, it will be padded to the right with spaces.

#### '-'

The substring will be paded to the left.

#### '0'

Overrides the default padding from spaces to 0s

#### '.'

Sets a precision. The default value is 0, writting a number after '.' will change it. 

For numeric specifications the substring will be of at least 'precision' size, it will be padded to the left with 0s.

For strings the precision will set a maximum length.

#### '#'

Will write a '0x' or '0X' before x or X specifications' results.

#### ' '

Before the number of a signed specification, would place a space before positive numbers.

#### '+'

Before a signed specification, would place a plus before positive numbers.

Neither this document or printf's [manual](https://developer.apple.com/library/archive/documentation/System/Conceptual/ManPages_iPhoneOS/man3/printf.3.html) will fully describe the behaviour of this function. This is due to the amount of decisions that are not written on the manual and only come up experimenting with the original printf.

To fully understand the scope of this project, I invite you to read the subject.

To learn about the styleguide we need to follow, I invite you to read the [Norminette](https://github.com/42School/norminette). 

# Building

By cloning the repository and using [GNU Make](https://www.gnu.org/software/make/).

The original project was written for Mac and works for Debian and Ubuntu. The updated version might work only on Debian and Ubuntu.

## 42

[42](https://www.42network.org/about-us/) Is a programming school that teaches in an innovative way, focused on an strict model of peer to peer evaluation and self learning via the writting of, mostly, coding projects.

## Score/Testing

 - Evaluation (125/125)
 - [Francinette](https://github.com/xicodomingues/francinette) (All OK)
