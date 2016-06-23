# <a name="number-and-string-data-types"></a>Number and String data types

* [Numbers](#numbers)
* [String](#string)
* [Constants](#constants)
* [Built-in Operators](#built-in-operators)

<br>
### <a name="numbers"></a>Numbers

* Integer examples

```
>>> num1 = 7
>>> num2 = 42
>>> sum = num1 + num2
>>> print(sum)
49
>>> sum
49

>>> 34 ** 32
10170102859315411774579628461341138023025901305856

>>> 9/5
1.8
>>> 9//5
1
>>> 9%5
4
```

* Floating point examples

```
>>> appx_pi = 22 / 7
>>> area = 42.16
>>> appx_pi + area
45.30285714285714

>>> num1
7
>>> num1 + area
49.16
```

* the [E scientific notation](https://en.wikipedia.org/wiki/Scientific_notation#E_notation) can be used as well

```
>>> sci_num1 = 3.982e5
>>> sci_num2 = 9.32e-1
>>> sci_num1 + sci_num2
398200.932
```

* Octal numbers are prefixed with `0o` or `0O` (i.e digit 0 followed by lower/upper case letter o)
* Similarly, Hexadecimal numbers are prefixed with `0x` or `0X`

```
>>> oct_num = 0o12
>>> hex_num = 0xF
>>> oct_num
10
>>> hex_num
15
>>> oct_num + hex_num
25
```

**Further Reading**

* [Python docs - numbers](https://docs.python.org/3/tutorial/introduction.html#numbers)
* [decimal](https://docs.python.org/3/library/decimal.html)
* [fractions](https://docs.python.org/3/library/fractions.html)
* [complex](https://docs.python.org/3/library/functions.html#complex)

<br>
### <a name="string"></a>String

* strings can be declared using single or double quotes
* Use `\` to escape quotes which are part of string itself if the string contains both single and double quotes

```
>>> str1 = 'This is a string'
>>> str1
'This is a string'
>>> greeting = "Hello World!"
>>> greeting
'Hello World!'
>>> weather = "It's a nice and warm day"
>>> weather
"It's a nice and warm day"
>>> print(weather)
It's a nice and warm day
```

* Escape sequences like newline character `\n` can be used within string declaration

```
>>> colors = 'Blue\nRed\nGreen'
>>> colors
'Blue\nRed\nGreen'
>>> print(colors)
Blue
Red
Green
```

* Use `r` prefix if you do not want escape sequences to be interpreted

```
>>> raw_str = r"tr '\n' ' ' < list.txt"
>>> raw_str
"tr '\\n' ' ' < list.txt"
>>> print(raw_str)
tr '\n' ' ' < list.txt

>>> normal_str = "tr '\n' ' ' < list.txt"
>>> print(normal_str)
tr '
' ' ' < list.txt
```

* String concatenation and repetition

```
>>> str1
'This is a string'
>>> str2 = ' with concatenation'
>>> print(str1 + str2)
This is a string with concatenation

>>> style_char = '-'
>>> style_char * 10
'----------'

>>> word = 'buffalo '
>>> print(word * 8)
buffalo buffalo buffalo buffalo buffalo buffalo buffalo buffalo 
```

**Further Reading**

* [Python docs - strings](https://docs.python.org/3/tutorial/introduction.html#strings)
* [Python docs - List of Escape Sequences and more info on strings](https://docs.python.org/3/reference/lexical_analysis.html#strings)
* [Python docs - Binary Sequence Types](https://docs.python.org/3/library/stdtypes.html#binary-sequence-types-bytes-bytearray-memoryview)

<br>
### <a name="constants"></a>Constants

Paraphrased from [Python docs - constants](https://docs.python.org/3/library/constants.html)

* `None` The sole value of the type `NoneType`
    * `None` is frequently used to represent the absence of a value
* `False` The false value of the `bool` type
* `True` The true value of the `bool` type
* [Python docs - Truth Value Testing](https://docs.python.org/3/library/stdtypes.html#truth)

```
>>> bool(2)
True
>>> bool(0)
False
>>> bool('')
False
>>> bool('a')
True
```

<br>
### <a name="built-in-operators"></a>Built-in Operators

* arithmetic operators
    * `+` addition
    * `-` subtraction
    * `*` multiplication
    * `/` division (float output)
    * `//` division (integer output)
    * `**` exponentiation
    * `%` modulo
* string operators
    * `+` string concatenation
    * `*` string repetition
* comparison operators
    * `==` equal to
    * `>` greater than
    * `<` less than
    * `!=` not equal to
    * `>=` greater than or equal to
    * `<=` less than or equal to
* boolean logic
    * `and` logical and
    * `or` logical or
    * `not` logical not
* bitwise operators
    * `&` and
    * `|` or
    * `^` exclusive or
    * `~` invert bits
    * `>>` right shift
    * `<<` left shift
* and many more...

**Further Reading**

* [Python docs - Numeric types](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex) - complete list of operations and precedence
* [Python docs - String methods](https://docs.python.org/3/library/stdtypes.html#string-methods)


