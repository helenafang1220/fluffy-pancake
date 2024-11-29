# fluffy-pancake
Python refresher note 
### Python Classes/Objects

Python is an object oriented programming language. 
A Class is like an object constructor. 

 
#### Step 1: Create a class named MyClass, with a property named x:
```python
class MyClass:
x = 5
```
#### Step 2: Use class named MyClass to create objects:
```python
result = MyClass()
print(result.x)
```

### The \_\_init\_\_() Function
This is a python built-in function. It gets executed everytime a class is inititated. 
We can use the \_\_init\_\_() function to assign values to object properties or other operations.

#### Create a class for a flight route, use the __init__() function to assign values for departure and destinaton:

```python
class Route:
  def __init__(self, dep, des):
    self.dep = dep
    self.des = des

result = Route("LGW", "AMS")
print(result.dep)
print(result.des)
```

### The \_\_str\_\_() Function
This built-in function allows us to specify the data type as a string and its format
```python
class Route:
  def __init__(self, dep, des):
    self.dep = dep
    self.des = des

  def __str__(self):
    return f"{self.dep}-{self.des}"

result = Route("LGW", "AMS")
print(result)
```
### Object methods
Objects can contain methods, we can create methods that belongs to the object

> [!NOTE]
> ###### In python, <ins>methods</ins> are essentially functions that can be called using dot notation. 

```python
class Route:
  def __init__(self, dep, des):
    self.dep = dep
    self.des = des

  def myMethod(self):
    print("The flight route is " + self.dep + "-" + self.des)

result = Route("LGW", "AMS")
result.myMethod()
```

### The <code>self</code> Parameter
As you can see from the previous examples, we use <code>self</code> as the first variable in class and method functions. 
It is essentially a placeholder that is used to access varibales that belongs to the class.
It does not have to be named <code>self</code>, but it has to be the <b>first</b> parameter of any function in the class.
#### An example of naming self differently, the code would still work
```python
class Route:
  def __init__(whatever, dep, des):
    whatever.dep = dep
    whatever.des = des

  def myMethod(aloha):
    print("The flight route is " + self.dep + "-" + self.des)

result = Route("LGW", "AMS")
result.myMethod()

### Modify Object Properties
We can modify properties on objects like:
```python
result.des = "LAX"
```

### Delete Object Properties
```python
del reuslt.des
```

### Delete Object
```python
del result
```

### The pass statement
<code>class</code> definitions cannot be empty, so we could use <code>pass</code> statement to avoid getting an error
```python
class Route:
  pass
```
