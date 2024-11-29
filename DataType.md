### Built-in Data Types

|Example|Data Type|Description
|:--------|:----------|:-------|
|<code>python x = "Fluffy Pancake"</code>|str|
|<code>x = 20 </code>|int|a whole number, positive or negative, without decimals of unlimited length|
|<code>x = 20.5 </code>|float|floating point number, positive or negative, containing one or more decimals|
|<code>x = 1j</code>|complex|Complex numbers are written with a "j" as the imaginary part
|<code>x = ["a", "b", "c"]</code>|list|
|<code>x = ("a", "b", "c")</code>|tuple|
|<code>x = range(6)</code>|range|
|<code>x = {"name": "John", "age": 36}</code>|dict|
|<code>x = frozenset({"a", "b", "c"})</code>|frozenset|
|<code>x = True</code>|bool|
|<code>x = b"Hello"</code>|bytes|
|<code>x = bytearray</code>|bytearray|
|<code>x = memoryview(bytes(5))"</code>|memoryview|
|<code>x = None</code>|NoneType|


### Numbers

#### Random numbers
Python does not have built-in random() function, but there is a built in module for this:

```python
import random
print(random.randrange(1,10))
```

### Strings
#### Slicing strings
##### Example 1: get characters from position 2 to position 5
```python
b = 'hello world'
print(b[2:5]
```

##### Example 2: Slice from start
```python
b = 'hello world'
print(b[:5]
```

##### Example 3: Slice to the end
```python
b = 'hello world'
print(b[2:])
```

##### Example 4: Negative Indexing
```python
b = 'hello world'
print(b[-5:-2]
```

#### Modify strings
##### Remove white space with <code>strip</code>
This function removes the whitespace that is before and/or after the actual text
```python
a = 'hello world   '
print(a.strip)) #returns 'hello world'
```

#### Replacing string
This function replaces a string with another string:
```python
a = 'hello world'
print(a.replace('h', 'b')) #returns bello world
```

#### Split string
The <code>split()</code> method returns a list where the text between the specified separator becomes list items. 
This is useful for strings that comes in patterns.
```python
a = 'hello world'
print(a.split(" ")) #separated by space, return ['hello', 'world']
```

#### Format strings
##### F-strings
the <code>{}</code> is used as a placeholder for variables, operations, funtions, and modifiers to format the value
```python
adult_pax = 5
txt = f"There are {adult_pax} adult passengers."
print(txt) # "There are 5 adult passengers."
```
##### placeholder as modifiers
a modifier is included by adding a colon <code>:</code> followed by a legal formatting type, for example <code>.2f</code> which means fixed fixed point number with 2 decimals:
```python
revenue = 289.984
txt = f"The total revenue is {revenue:.2f} pounds."
print(txt) # "The total revenue is 289.98 pounds."
```
or, to perform math operations
```python
adult_pax = 5
flight_price = 20.34
txt = f"The revenue is {adult_pax * flight_price} pounds."
print(txt) #return "The revenue is 101.7 pounds."
```




