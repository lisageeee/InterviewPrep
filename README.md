# Interview Prep

## Strings
#### [StringBuffer](https://docs.oracle.com/javase/7/docs/api/java/lang/StringBuffer.html) 
- Like a String but mutable!
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
### Getting rid of spaces:
- `string.replace(“ “, “”);`

## [ArrayLists](https://docs.oracle.com/javase/7/docs/api/java/util/ArrayList.html)
#### Finding the index of an element:
- `array.indexOf(element);`

