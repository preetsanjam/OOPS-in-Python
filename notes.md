## Notes

- **Object-Oriented Programming System (OOPS)** is a programming paradigm that provides a blueprint for organizing and structuring code using objects and classes.
- It allows us to define our own data types and move from generalization to specialization.

- **Class:**
    
    - "A `class` is a user-defined data type in object-oriented programming (OOP). It can be thought of as a blueprint for creating objects
    - All data types are built-in classes in Python.

- **Object:**

    - An object is an instance of a class.
    - **Everything in Python is an object.** 
    - Python provides **object literals** (`[]` for lists, `{}` for dictionaries, `""` for strings) for built-in data types.
    - Objects in Python have **attributes** (data) and **methods** (functions) that define their behavior and properties.

- Constructor `self`:

    - Whenever we create (or construct) an object of a class, a special built-in method called `__init__` is automatically invoked. This method is known as the constructor, and its first parameter is always `self`, which refers to the instance being created.
    - When we create an object of a class, Python automatically calls the `__init__` method. This is where we initialize the object — i.e., set up its default or user-defined values.
    
        For example:
        ```
        class MyClass:
            def __init__(self):
            print("Object created!")

        obj = MyClass()  # __init__ is called automatically
        ``` 

         Now, consider this example:
         ```
         c1 = complex()
        print(c1.real, c1.imag)  # Output: 0.0 0.0
         ```

         Here’s what’s happening under the hood:
        
        - Python's built-in complex type is actually a class.
        - When we do `c1 = complex()`, Python internally calls the **constructor**:

            ```
            complex.__init__(self, real=0.0, imag=0.0)
            ```
            Since we didn’t pass any arguments, the default values `0.0` (for both real and imaginary parts) are used.
