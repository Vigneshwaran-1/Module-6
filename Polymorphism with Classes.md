# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
~~~
class Beans:
    def type(self):
        return "Vegetable"
    
    def color(self):
        return "Green"

class Mango:
    def type(self):
        return "Fruit"
    
    def color(self):
        return "Yellow"

def describe_item(item):
    print(f"Type: {item.type()}")
    print(f"Color: {item.color()}")

# Creating objects
beans_obj = Beans()
mango_obj = Mango()

print("Beans:")
describe_item(beans_obj)

print("\nMango:")
describe_item(mango_obj)
~~~

## Output
~~~
Beans:
Type: Vegetable
Color: Green

Mango:
Type: Fruit
Color: Yellow
~~~

## Result
Thus given program is verifed succesfully.
