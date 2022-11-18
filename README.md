# Python-Notes


# Function: 
 It a small segment of a program. In python function are just like other data types. We can perform all functions on it, which we can apply on other data types.<br> 
## **Syntax:**
```
def function_name():
 body of fynction<br>
function_name()
```
**Explanation:**
  whenever control find def keyword it will jump to the next line of functiondefinition end. it execute all line of code wen it find call of function it will jump to def and start executing the function definition body.
  always rember, whenever the function call there is a memory space allocated to it other than main program memory space. the life of the function end when it returns the value.
 ```
def message():
  print('this program return none')
 message()
 ```
 In this example the function return none. but it will print the result in function


## Nested Function
 The function in another function.Example
 ```
def f():
 def g():
   print('Inside g function')
 g()
 print('Inside F function')
```
## **Function are First Class Citizens:**
 As in programming data types are the first class citizens.You can apply all operations on it. In python function are Ist Class Citizen<br>type(function_name) it defines the type which is function in this case <br>id(function_name) it defines the address in memory
 
- Assignement x = function_name
- del function_name: it will delete the function<br>
- Storing: e.g 
  ```L=[1,2,3,function_name]
    L[-1](3)
    ```
- Returning one function to another function:
  ```
 def f():
  def x(a,b):
    return a+b
 return x 
 
 val = f()(3,4)
 print(val)
```
