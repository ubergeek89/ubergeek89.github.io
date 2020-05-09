# Using Function Argument Annotations In Python


Function argument annotations can be a useful way to give programmers hints about how a function is supposed to be used. For example, consider the following annotated function:

```python
def add(x:int, y:int) -> int:
	return x + y
```

The Python interpreter does not attach any semantic meaning to the attached annotations. They are not type checks, nor do they make Python behave any differently than it did before. However, they might give useful hints to others reading the source code about what you had in mind. Third-party tools and frameworks might also attach semantic meaning to the annotations. They also appear in documentation:

```python
>>> help(add)
Help on function add in module __main__:
add(x: int, y: int) -> int
```

Although you can attach any kind of object to a function as an annotation (e.g., numbers, strings, instances, etc.), classes or strings often seem to make the most sense. Function annotations are merely stored in a function’s __annotations__ attribute. For example:

```python
>>> add.__annotations__
{'y': <class 'int'>, 'return': <class 'int'>, 'x': <class 'int'>}
```

Although there are many potential uses of annotations, their primary utility is probably just documentation. Because Python doesn’t have type declarations, it can often be difficult to know what you’re supposed to pass into a function if you’re simply reading its source code in isolation. An annotation gives someone more of a hint.
