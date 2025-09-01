---
theme: solarized
---

# Your Spec

![[Pasted image 20250831072358.png|x50]]

----



![[Pasted image 20250831072419.png|x200]]

----


![[Pasted image 20250831072445.png]]


----
# Activities

1. Litmus Test - OOP Puzzles<!-- element class="fragment" -->
2. Introduction to OOP md worksheet<!-- element class="fragment" -->
3. OOP Continued md worksheet<!-- element class="fragment" -->
4. Objectifying Your Y10 PPP task<!-- element class="fragment" -->
5. Python Challenges XXIVC: My Object Oriented Restaurant<!-- element class="fragment" -->
6. *Other Python Challenges tasks as needed*<!-- element class="fragment" -->
7. SpaceInvaders Project<!-- element class="fragment" -->

---
## Keywords Lesson 1


- Object<!-- element class="fragment" -->
- Class<!-- element class="fragment" -->
- Instance<!-- element class="fragment" -->
- Property / Attribute<!-- element class="fragment" -->
- Method<!-- element class="fragment" -->
- `self`<!-- element class="fragment" -->
- Constructor / `__init__()`<!-- element class="fragment" -->
- Getter<!-- element class="fragment" -->
- Setter<!-- element class="fragment" -->
- Private `__`<!-- element class="fragment" -->
- Protected `_`<!-- element class="fragment" -->
- Pubic<!-- element class="fragment" -->
- Modifier<!-- element class="fragment" -->


---

## Keywords Lesson 2

- Parent / Superclass<!-- element class="fragment" -->
- Child / Subclass<!-- element class="fragment" -->
- `super()`<!-- element class="fragment" -->
- Inheritance<!-- element class="fragment" -->
- Composition<!-- element class="fragment" -->
- Aggregation<!-- element class="fragment" -->
- Overriding<!-- element class="fragment" -->

---
# 'Do Now's Lesson 1

_With your partner, discuss each code snippet. What will be output, and why?_

----

```python
class A:
	def __init__(self, thing):
		A.name = thing
		
class B:
	def __init__(self, thing):
		self.name = thing
		
		
var1 = A("Tim")
var2 = A("Tom")
var3 = B("Tin")
var4 = B("Ton")

print("var2 is called", var2.name)
print("var1 is called", var1.name)
print("var4 is called", var4.name)
print("var3 is called", var3.name)

```

---


```python

class X:
	def __init__(self):
		self.x = "fish"
		self.y = "cat"
	
	def test(self):
		return self.x == self.y
		
thing = X()
if thing.test:
	print("Fishcat")
```

----


```python

class Y:
	def __init__(self):
		self.__x = "horsey"
		self.__y = "frogs"
	

		
test = Y()
print(f"I like {test.__x}s and I like {test.__y}s!")
```

---
