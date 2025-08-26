
CodeBlocks are a useful way to capture small bits of code in your notes, and with the [CodeEmitter](https://github.com/mokeyish/obsidian-code-emitter) plugin they can be run inside your [[obsidian]] markdown notes vault!

Here's some examples which can be run directly in [[obsidian]]:

A simple hello world:
``` python
print("Hello World")
```

A syntax error:
``` python
print(this is a test)
```

A more complex error (recursion depth): 
``` python
def f(a):
	print(f(a+1))
f(0)
```
