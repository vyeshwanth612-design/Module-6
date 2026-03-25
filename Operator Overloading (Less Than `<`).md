# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```p
class A:
    def __init__(self, a):
        self.a = a

    def __lt__(self, other):
        if self.a < other.a:
            return "ob1 is less than ob2"
        else:
            return "ob2 is less than ob1"

ob1 = A(15)
ob2 = A(25)

print("Comparing ob1 (15) and ob2 (25):")
print(ob1 < ob2)

ob3 = A(50)
ob4 = A(30)
print("\nComparing ob3 (50) and ob4 (30):")
print(ob3 < ob4)
```

## Output
<img width="1011" height="500" alt="image" src="https://github.com/user-attachments/assets/c4132de4-757a-424a-9df7-7d8ec0bd6950" />

## Result
The Python program was executed successfully, demonstrating operator overloading using the less than (<) operator. The custom comparison logic worked correctly, and the appropriate message was displayed based on the comparison of the two objects.
