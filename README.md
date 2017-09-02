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

