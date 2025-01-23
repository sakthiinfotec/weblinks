#### Python

**Decorators**
Python supports "decorators," which are functions that modify the behavior of other functions or methods. They are commonly used for logging, enforcing access control, memoization, and more. For example: 

```python
def decorator (func):
  def wrapper():
    print("Before the function call")
    func()
    print("After the function call")
return wrapper

@decorator
def say_hello():
  print("Hello!")

say_hello()
```
