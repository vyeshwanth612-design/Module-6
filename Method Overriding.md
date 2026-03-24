# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
```p
class Fish:
    def type(self):
        print("This is a fish")

class Shark(Fish):
    # Overriding the parent's type() method
    def type(self):
        print("This is a shark")

obj_goldfish = Fish()
obj_hammerhead = Shark()

print("--- Method Overriding in Action ---")
for sea_creature in (obj_goldfish, obj_hammerhead):
    sea_creature.type()
```

## OUTPUT
<img width="997" height="450" alt="image" src="https://github.com/user-attachments/assets/2567d153-ce58-4289-b664-4bd71d68dfa0" />

## RESULT
