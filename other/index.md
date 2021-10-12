# Python Documentation

## Data Types:

### Strings:

- A string contains a set of characters that can be manipulated to do several things such as, print statements and store information.
  - Strings start and end with " or ' (double or single quotations), but you cannot start with one and end with the other.

##### Example 1:

```
  print("Hello world!")
```
- This string starts and ends with "
  - In this case, the string is: "Hello world!"

##### Example 2:

```
  answer = input('What is your name? ')
```
- This string starts and ends with '
  - In this case, the string is: 'What is your name? '

### Integers:

- An integer is like a string except it can only have whole numbers and it doesn't use quotations.
  - Integers can be divided ( using / ), added together ( using + ), subracted from one another ( using - ), multiplied ( using * ), and so on.

##### Example 1:

```
  a = "1"
  b = int(a)
```
- *a* is equal to the string "1", but it is not an integer. While, *b* is equal to the integer of a, so 1, and can be used as so.

##### Example 2:

```
  a = "4"
  b = int(a)

  print(a / 2)
  print(b / 2)
```
- *a* will give you an error because Python thinks you are trying to divide a string. But, *b* will print 2 because it is an integer and functions as so.

### Floats:

- A float is like an integer, except it is able to use decimals as well as whole numbers.

##### Example 1:

```
  a = "1.5"
  b = int(a)
  c = flaot(a)
```
- In this example, *b* will not assign, but error out because the int() function does not take decimals, and *c* will turn the string "1.5" into 1.5.

##### Example 2:

```
  a = "4.5"
  b = int(a)
  c = float(a)

  print(a * 2)
  print(b * 2)
  print(c * 2)
```

- In this example, multiplying *a* by 2 will not error out, but instead of printing 9, which is the correct answer, it will just print the string "4.5" twice. As with the last example, assigning *b* will not work because the int() function does not work with decimal points. But, *c* will work as intended and print 9.

### Lists:

- Lists are used to store a lot of the previous types of data in one referenceable name.

##### Example 1:

```
  list1 = ["word1", 1, 1.0]

  print(list1[0])
```

- In this example, the items in the list are being assigned ahead of time, and separated with commas.
  - As shown with the print statement, the first item of the list is being printed. To reference specific items in a list, you take the item place, and subtract one number.

##### Example 2:

```
  number = 1.0
  list1 = ["word1", 1]

  list1.append(number)

  print(list1[2])
```

- In this example, the **.append()** option is used to add another item to the list, since it wasn't there in the beginning.

## Variables:

- Variables are words or recognizable arrangements of characters that can be assigned a specific value that can be referenced later or changed.
  - Variables are assigned using the = symbol, and can contain letters and numbers, but must never start with a number.

##### Example 1:

```
  var1 = "Hi"
```

- In this example, the variable is *var1* is assigned the string "Hi".

##### Example 2:

```
  var1 = "Hello "
  var2 = "World!"
  var3 = var1 + var2

  print(var3)
```

- This example uses the string combining feature to take the two variables and combine them into one, and then print it.

## Conditionals:

### If, Else Statements:

- An if, then statement is used to execute code when a certain thing is true.

##### Example 1:

```
  a = 1
  b = 2

  if a == b:
    print("a is equal to b. ")

  else:
    print("a is not equal to b. ")
```

- In this example, the if, then statement is being used to detect if *a* is equal to *b* or not, and to print something depending on the outcome.

##### Example 2:

```
  a = 1
  b = 2
  c = 3

  if a == b:
    print("a is equal to b. ")

  elif a == c:
    print("a is equal to c. ")
  
  else:
    print("a is not equal to b or c. ")
```

- If this example, the code demostrates another use of the if, else conditional statement, the **elif** statement. 
  - This gives the coder the ability to have several things checked before ending the if, else statement.
  - The elif statement can be used as many times as necessary.

### Try and Except:

- The try and except statement is used to attempt to run a piece of code, and if it doesn't work, do something else.

##### Example 1:

```
  a = "1.0"
  
  try:
    b = int(a)
  
  except:
    print("b is not an integer or it contains a decimal point.")
```

- In this example, try and except is used to try to convert *a* or "1.0" into an integer, but since it contains a decimal point, it fails and moves on to the except statement.

##### Example 2:

```
  a = "1.0"
  b = "1.5"

  try:
    c = int(a)

  except:
    print("a is not an integer or it contains a decimal point.")
    c = int(b)

  finally:
    print("a and b are not integers or they contain a decimal point.")
```

- In this example, the try and except statement is used to attempt to convert *a* or "1.0" into an integer, but since it has a decimal point, it doesn't work, and the except attempts to convery *b* or "1.5" into an integer, but since it also contains a decimal point, it didn't work as well.

  - Finally is used at the end as the finishing statement to say, if nothing else works, do this.

