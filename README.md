# Python-Notes


# Function: 
 It a small segment of a program. In python function are just like other data types. We can perform all functions on it, which we can apply on other data types.
 **Benefits of using a Function**
  - Code Modularity
  - Code Readibility
  - Code Reusability 
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
- del function_name: it will delete the function
- Storing: e.g 
  ```
     L=[1,2,3,function_name]
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

## Lambda Function

A lambda function is a small anonymous function. A lambda function can take any number of arguments, but can only have one expression.
```
 lambda parameters : Expression
 where 
 lambda is a keyword,it creates lambda expression
 parameters: one or more parameters are supported but separated by commas
 expression: must be single valid python expression
 
```
**Difference between lambda vs Normal Function**
- No name
- lambda has no return value(infact,returns a function)
- lambda is written in 1 line
- not reusable
WHY?
for HOF
## Higher Order Function
 - Function which return function. 
 - Function which take input a function
 ```
  def square(x)
    return x**2
  def fun_hof(f,L):
    data=[]
    for i in L:
      data.append(f(i))
   print(data)
 L = [1,2,3,4,5]
 fun_hof(square,L)     
 ```
 
 ```
 def fun_hof(f,L):
    data=[]
    for i in L:
      data.append(f(i))
   print(data)
 L = [1,2,3,4,5]
 fun_hof(lambda x:x**2,L)    
 
 ```
