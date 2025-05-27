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
~~~
# Python program demonstrating Encapsulation

class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length  # Private variable
        self.__breadth = breadth  # Private variable

    # Method to get the length
    def get_length(self):
        return self.__length

    # Method to set the length
    def set_length(self, length):
        if length > 0:
            self.__length = length
        else:
            print("Invalid length! Must be positive.")

    # Method to get the breadth
    def get_breadth(self):
        return self.__breadth

    # Method to set the breadth
    def set_breadth(self, breadth):
        if breadth > 0:
            self.__breadth = breadth
        else:
            print("Invalid breadth! Must be positive.")

    # Method to calculate area
    def calculate_area(self):
        return self.__length * self.__breadth

# Creating an object of Rectangle
rect = Rectangle(10, 5)

# Accessing private variables through methods
print(f"Length: {rect.get_length()}")
print(f"Breadth: {rect.get_breadth()}")
print(f"Area: {rect.calculate_area()}")

# Modifying private variables using methods
rect.set_length(15)
rect.set_breadth(7)

print("\nUpdated Values:")
print(f"Length: {rect.get_length()}")
print(f"Breadth: {rect.get_breadth()}")
print(f"Area: {rect.calculate_area()}")
~~~

## Output
~~~
Length: 10
Breadth: 5
Area: 50

Updated Values:
Length: 15
Breadth: 7
Area: 105
~~~

## Result
Thus given program is verified successfully.
