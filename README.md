# quine

Tried to create quine in python.

Seems, I understand, how it works.

When `eval(var)` is called, `repr(val)` is expanded, and then print is called.

Also, code from [source](https://www.codespeedy.com/quine-in-python/):

```Python
var = "print('var = ', repr(var), '\\neval(var)')"
eval(var)
```

Prints this (look at that extra space after `var = `):
```bash
var =  "print('var = ', repr(var), '\\neval(var)')"
eval(var)
```

But if you remove space like this `var = "print('var =', ...`, output stays the same as code:

```bash
var = "print('var =', repr(var), '\\neval(var)')"
eval(var)
```

[Source](https://www.codespeedy.com/quine-in-python/)

