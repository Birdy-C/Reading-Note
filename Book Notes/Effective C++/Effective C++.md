# Chapter 1: Accustoming Yourself to C++


# Chapter 2: Constructors, Destructors, and Assignment Operators

## Item 7: Declare destructors virtual in polymorphic base classes.
- When a derived class object is deleted through a pointer to a base class with a non-virtual destructor, results are undefined.
- Don't define virutal destructor for non-virtual function cause vptr has overhead.
- STL container are usually *final* (lack a virtual destructor)
- Can use pure virtual destructor to define abstract class.

# Chapter 3: Resource Management


# Chapter 4: Design and Declarations


# Chapter 5: Implementations


# Chapter 6: Inheritance and Object-Oriented Design

# Chapter 7: Template and Generic Programming


# Chapter 8: Customizing *new* and *delete*

# Chapter 9: Miscellany
