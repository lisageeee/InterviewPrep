# Interview Prep

## Strings
#### [StringBuffer](https://docs.oracle.com/javase/7/docs/api/java/lang/StringBuffer.html) 
- Like a String but mutable! Also better O. 
- To create: `StringBuffer sb = new StringBuffer();`
- To clear: `sb.setLength(0);`
- To set character at index: `sb.setCharAt(index, char);`
#### To return the first index of a substring:
- `str.indexOf("substring");`
#### Getting rid of non-alphanumeric characters:
- `input.replaceAll("[^a-zA-Z]+", "");`
#### Trim whitespace:
- `str.trim();`
#### Determining whether a character is uppercase:
- `isUpperCase(char)`
#### Turning a string into a char array:
- `char[] ch = str.toCharArray();`
#### Turning a char array into a string:
- `String str = new String(ch);`
#### Getting rid of spaces:
- `string.replace(“ “, “”);`
#### Getting the numeric value of a character:
- `int x = Character.getNumericValue(char);`
- ex; 'a' = 1
#### Things to thing about
- Letter case
- White spaces
- ASCII or Unicode. Unicode uses ASCII for the first 128 characters
#### String reversal questions:
- Reversing a string: simply return `new StringBuffer(input).reverse().toString();`
- Reversing only vowels: turn the input string into a character array & iterate through it to see if it contains any vowels. Save the index of the vowels in a list. Iterate through the list & change around the corresponding indices in the char array. 
- Reversing words in a string: Create a string array by splitting the input by " ". Create a new StringBuffer `sb`. For each string in the string array turn it into a StringBuffer, reverse it, and append it + " " to our `sb`. Return `sb` as a string.
- When reversing in place we do not need to iterate through the entire string, can stop half way.

## [ArrayLists](https://docs.oracle.com/javase/7/docs/api/java/util/ArrayList.html)
#### Finding the index of an element:
- `array.indexOf(element);`

## Bit Manipulation
#### Shifting:
- 0001<< 1 = 0010
- 1 << 1 = 2
- 1100 >> 2 = 0011
- The right shift operator is signed.
- Right shift divide a number by 2. Rounds down.
- A negative number’s most significant bit is 1. A signed right shift operator will shift the value of the sign.
- Use >>> for unsigned shift ~ forces a 0
- Left shift multiplies a number by 2.
#### Creating a bit mask:
- If we want to create 00000100 we can do `int bm = 1 << 2;`
#### Bitwise Operators:
- 1010 & 0101 == 0000
- 1010 | 0101 == 1111
- ~1010 == 0101
- 1100 ^ 0110 == 1010
#### Creating an integer from a binary string:
- `Integer.toBinaryString(number);`
#### Getting the position of the highest ordered bit:
- `highestOneBit(int i)` - 1.
#### ParseInt:
- `Integer.parseInt(“1011”, 2)` ~ creates an integer with binary value of 1011. 
#### Number of bits:
- An integer has 32 bits.
#### Determining whether an integer is a power of 2:
- Since power of 2 means only one bit of n is 1, we can just check whether `n&(n-1) == 0`
#### Setting a bit number:
- `100010 |= (1<<2) === 100110`
#### Turning off a bit number:
- `100110 &= ~(1<<2) === 100010`
#### Check whether xth bit is 1:
- `result = 101010 & (1 << 3)` If this is `!= 0` then the xth bit is 1.
#### Flip the xth bit:
- `101000 ^= (1 << 2) === 101100`
#### To get value of least significant bit that is 1:
- ` X & ~X`
#### Turn on all bits in a set of size n:
- `(1 << n) - 1`


