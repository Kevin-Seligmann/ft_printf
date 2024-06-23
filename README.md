# ft_printf

This is a small implementation of the C's printf function, based on MAC implementation (e.g, it prints '(NULL)' for an string that is a null pointer instead of '(nil)').

## Format

- width, a number specifying the smallest posible size of the transformation 
- '-', changes the by-default right padding
- '0', padding is replaced by 0's.
- '.', sets a precision for numeric specifications (minimum digits), or for strings (maximum length)
- '#', modifies some of the specifications' result
- ' ', places a space before a signed number
- '+', places a + before a signed number

## Specifications

- %c - A character
- %s - A string
- %p - An address printed in hexadecimal
- %d - An INT printed in base 10
- %i - An INT printed in base 10
- %u - An UNSIGNED INT printed in base 10
- %x - A hexadecimal number in lowercase
- %X - A hexadecimal number in uppercase
- %% - The % symbol

Disclaimer: Neither this document or printf's [manual](https://developer.apple.com/library/archive/documentation/System/Conceptual/ManPages_iPhoneOS/man3/printf.3.html) will fully describe the behaviour of this function. This is due to the amount of decisions that are not written on the manual
and only come up experimenting with the original printf, which might also be SO dependant.

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
