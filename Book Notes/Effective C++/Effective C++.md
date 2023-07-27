# Chapter 1: Accustoming Yourself to C++

## Item 1: View C++ as a federation of languages.
- Today's C++ is a multiparadigm programming language, one suppporting a combination of procedural, obect-oriented, functional, generic, and metaprogramming features.
-Four bacis sublanguages: *C*, *Object-Oriented C++*, *Template C++*, *STL*. Best strategy changes when switch from one sublanguage to another.

# Chapter 2: Constructors, Destructors, and Assignment Operators

## Item 7: Declare destructors virtual in polymorphic base classes.
- When a derived class object is deleted through a pointer to a base class with a non-virtual destructor, results are undefined.
- Don't define virutal destructor for non-virtual function cause vptr has overhead.
- STL container are usually *final* (lack a virtual destructor).
- Can use pure virtual destructor to define abstract class.

# Chapter 3: Resource Management


# Chapter 4: Design and Declarations

## Item 20: Prefer **pass-by-reference-to-*const*** to **pass-by-value**.
- Avoid unnecessary calls to copy constructor and destructor.
- Avoid *Slicing* problem, copy a child to a parent type would lose the runtime property.
- **Pass-by-reference-to-*const*** ususally implemented by pointer.
- This rule doesn't apply to built-in types and STL iterator and function object types.

## Item 23: Prefer non-member non-friend functions to member functions.
- The more something is encapsulated, the fewer things can see it.
- Namespace, unlike classes, can be spread across multiple source files.
- Best way is to put function and class into same namespaces. User can incluse the header needed. That's how STL is organized, e.g. vector, algorithm.

# Chapter 5: Implementations


# Chapter 6: Inheritance and Object-Oriented Design


# Chapter 7: Template and Generic Programming


# Chapter 8: Customizing *new* and *delete*


# Chapter 9: Miscellany
