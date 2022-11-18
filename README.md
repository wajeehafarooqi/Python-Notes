# Python-Notes


Function: it a small segment of a program. In python function are just like other data types. We can perform all functions on it, which we can apply on other data types.<br> 
<u>**Syntax:**</u><br>
def function_name():<br>
&nbsp;&nbsp;&nbsp;&nbsp;body of fynction<br>
function_name() # call of function<br>
<u>**Explanation:**</u><br>
  <p>whenever control find def keyword it will jump to the next line of functiondefinition end. it execute all line of code wen it find call of function it will jump to def and start executing the function definition body.
  always rember, whenever the function call there is a memory space allocated to it other than main program memory space. the life of the function end when it returns the value.</p>
<p>def message():<br>
 &nbsp;&nbsp;&nbsp;&nbsp;print('this program return none')<br>
 message()
 In this example the function return none. but it will print the result in function
</p>

<u>**Nested Functions**</u><br>
<p> The function in another function.Example<br>
def f():<br>
&nbsp;&nbsp;&nbsp;&nbsp;def g():<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;print('Inside g function')<br>
&nbsp;&nbsp;&nbsp;g()<br>
&nbsp;&nbsp;&nbsp;print('Inside F function')</p>
<u>**Function are First Class Citizens:**</u><br>
<p> As in programming data types are the first class citizens.You can apply all operations on it. In python function are Ist Class Citizen<br>type(function_name) it defines the type which is function in this case <br>id(function_name) it defines the address in memory<br>
Assignement x = function_name<br>
del function_name: it will delete the function<br>
Storing: e.g L=[1,2,3,function_name]<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;L[-1](3)<br>
**Returning one function to another function:**<br>
def f():<br>
&nbsp;&nbsp;&nbsp;&nbsp;def x(a,b):<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return a+b<br>
&nbsp;&nbsp;&nbsp;&nbsp;return x <br>
val = f()(3,4)<br>
print(val)</p>
