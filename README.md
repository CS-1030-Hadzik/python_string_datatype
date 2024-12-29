 # Advanced Strings
 ## Strings -- List of Characters

>Characters can be: 
>  - Letters  ` [A-Za-z] `
>  - Numbers  ` [0-9] ` 
>  - Symbols  ` [@ $ # ~ ]`
>  - [Unicode Characters Site](https://pythonforundergradengineers.com/unicode-characters-in-python.html)
>  - Spaces   `[' ']`
>  - Escape Character `[\n \r \t \' \\ \b \f \ooo \xhh]`

 ## String Indexing
> Strings in Python are sequences of characters, where each character has an index (positive or negative).
>
> Positive indexing starts at 0 and goes from left to right.
> Negative indexing starts at -1 and goes from right to left.
>
>|Char#  |1  |2  |3  |4  |5  |6  |7  |8  |9  |10 |11|
>|:-:    |:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
>|Char   |W  |E  |B  |E  |R  |   |S  |T  |A  |T  |E  |
>|+ Index|0  |1  |2  |3  |4  |5  |6  |7  |8  |9  |10 |
>|- Index|-11|-10|-9 |-8 |-7 |-6 |-5 |-4 |-3 |-2 |-1 |
>
>```python
># Select characters out of a string
>school = 'WEBER STATE'
>print ('character 1 :' + school[0])        -->
>print ('character 4 :' + school[3])        -->
>print ('character 7 :' + school[-4])       -->
>```
>
## Slicing Strings

>- ### SYNTAX -- string [`start` : `end`]
>	- begin at `start` and extending up to but not including `end`
>	- school[0:3] --> `WEB`	
>	- `start` blank
>		- start at index 0
>		- **school[:3] r--> `WEB`**
>	- `end` blank
>		- go until the end of the string
>		- school[8:] --> `ATE` 
>```python
># Select a substring
>print ('start = 0 end = 4: ' + school[0:4])    --> 
>print ('start = 0 end = 5: ' + school[0:5])    -->
>```
>```python
>print ('start = 2 end = 5: ' + school[2:5])    -->
>print ('start = -5 end = : ' + school[-5:-1])  -->
>```
>```python
>print ('start = -5 end = : ' + school[-5:])    -->
>print ('start =  end = : ' + school[:])        -->
>```

- String have a length property

## Combining Strings

>- ### String Operators
>  - \+  `concatenate (combine strings)` 
>  - \*  `create multiple copies of the string`
>```python
># combine string
> a = 'apple'
> b = 'sauce'
>
> print (a + b)       -->
> print (a + b + a)   -->
>
>
> print (a * 3)       -->
> print (3 * a)       -->
>
>


## Formating Strings
>  - `Can't combine strings and numbers unless you use format`
>```python
># This will produce a TypeError
> age = 75
> person = 'Scott is ' + age
> print (person)
>   
> # Using .format()
> age = 25
> name = "Alice"
> print("{} is {} years old.".format(name, age))
> # Output: Alice is 25 years old.

> # Using f-strings (Python 3.6+)
> print(f"{name} is {age} years old.")
> # Output: Alice is 25 years old.
> 
> #Using the format string method for multiple items
> age = 75
> hours = 10
> person = 'Scott is {} he sleeps {} hours a day'
> print (person.format(age, hours))
>
> hours = 8
> dogs = 2
> print("{0} sleeps {1} hours and owns {2} dogs.".format(name, hours, dogs))
> # Output: Alice sleeps 8 hours and owns 2 dogs.


## Escape characters and strings
>  - `illegal characters in a string require an escape character`
>  - `Use ` \ ` followed by the character `
>  - Escape Character `[\n \r \t \' \\ \b \f \ooo \xhh]`
>```python
># use of single quote in string
> txt = "Scott's Dog"
> # or
> txt = 'Scott\s Dog'
>   
> #Using the format string method
> age = 75
> person = 'Scott is {}'
> print (person.format(age))
> 
> #Using the format string method for multiple items
> age = 75
> hours = 10
> person = 'Scott is {} he sleeps {} hours a day'
> print (person.format(age, hours))
>
> #Using the format string method for multiple items with index
> age = 75
> hours = 10
> dogs = 5
> person = 'Scott sleeps {1} hours a day. He is {0} years old. He has {2} dogs'
> print (person.format(age, hours, dogs))

## Common string methods
>  - `capitalize()` first character to uppercase
>  - `title()` first character of each word to uppercase
>  - `casefold()` lowercase
>  - `len()` return the length of the string
>  - `count()` number of times a value occurs in a string
>  - [additional string methods](https://realpython.com/python-strings/#built-in-string-methods)

>```python
># capitilize the first letter
> name = 'scott'
> print (name.capitalize())
> 
> name = 'sCoTt'
> print (name.capitalize())




## More info on Strings
- [realpython.org -> Strings](https://realpython.com/python-strings/)
- [w3schools.org -> Strings](https://www.w3schools.com/python/python_strings.asp)
- [python.org  -> Strings](https://docs.python.org/3/tutorial/introduction.html#strings)
