# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```p
class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length
        self.__breadth = breadth
       
        self.display_private_data()

    def display_private_data(self):
        print(f"Inside Class: Length is {self.__length}")
        print(f"Inside Class: Breadth is {self.__breadth}")

print("--- Creating Rectangle Object ---")
rect = Rectangle(50, 20)

try:
    print(rect.__length)
except AttributeError:
    print("\nAccess Denied: Cannot access '__length' from outside the class.")
```

## Output
<img width="831" height="375" alt="image" src="https://github.com/user-attachments/assets/fc526837-c578-4be4-bb5c-ea55fc43be1a" />


## Result
The Python program was executed successfully, demonstrating encapsulation using private member variables. The private attributes __length and __breadth were accessed within the class, ensuring data hiding.
