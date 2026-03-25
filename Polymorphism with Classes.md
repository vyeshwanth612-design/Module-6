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
```p
class Beans:
    def type(self):
        print("Type: Vegetable")
        
    def color(self):
        print("Color: Green")

class Mango:
    def type(self):
        print("Type: Fruit")
        
    def color(self):
        print("Color: Yellow")

def func(obj):
    obj.type()
    obj.color()

bean_obj = Beans()
mango_obj = Mango()

print("--- Testing Polymorphism with Beans ---")
func(bean_obj)

print("\n--- Testing Polymorphism with Mango ---")
func(mango_obj)
```
## Output
<img width="984" height="417" alt="image" src="https://github.com/user-attachments/assets/89f06e8f-fa6b-42fc-8ee6-b5f5f39f0e84" />


## Result
The Python program was executed successfully, demonstrating polymorphism using a generic function. The function correctly identified the type and color of both objects:

For Beans → Output: Vegetable, Green
For Mango → Output: Fruit, Yellow

Thus, the program confirmed that a single function can work with different object types using polymorphism.
