# Object Oriented Programming
## OOP
Revolves around the idea of creating objects that encapsulate data and behaviour. Objects interact with data/other objects through methods. There are 4 principles of OOP: 
- Encapsulation
- Abstraction
- Inheritance
- Polymorphism

## Encapsulation
Bundling common data and behaviour in single entity called an object is called Encapsulation. It hides all the internal details from the outisde world and provides methods to interact with other objects/data. Provides data protection and modification of member data through controller methods. 

> Example: Before the existence of mobile phones, there was a pager for messaging, and telephone for calls. These common functionalities have been bundled up in one single entity called the mobile phone.

## Abstraction
Hiding all the complex functionalities and providing a simple interface for the user is called an abstraction. 

> Example: A mobile phone call involves a lot of complex procedures like using the antenna bands to reach the nearest mobile tower and so on, but the user is only exposed to one call button.

## Inheritance 
Allows to inherit properties and methods from other classes. Can create specialised classes from generic classes. 

> Example: A vehicle class could be inherited by a car class, truck class, bike class

## Polymorphism 
Morphism means to change, and poly means many. Polymorphism is when an entity behaves like another entity. 

> Example: An animal class could be inherited by a Dog class and a Cat class. The same method sound() in animal class, "makes a sound". But in dog class, "barks" and in cat class, "meows".

## Class
Class is a blueprint or a template to create objects. A class defines its properties(attributes) and behaviour(functions). Classes encapsulate data and behaviour, to provide a way to model real world entities. The key components of a class are: 
- Attributes: Variables to hold data
- Methods(Functions): Functions that define the behaviour
- Constructor: A specialised method to "construct" an object
- Destructor: A specialised method to "destruct" an object
- Access Modifiers: Used to control the accessibility of class members

```c++
#include <iostream>
using namespace std;

class Animal
{
private: //private Access Modifier
    string name; //Attributes
    int legs;

public:
    Animal(string n, int l) //Constructor
    {
        name = n;
        legs = l;
    }

    ~Animal() //Destructor
    {
        ;
    }

    void makeSound() //Method
    {
        cout << "Animal making sounds..." << endl;
    }
};
```

## Object
An instance of a class. Fundamental building blocks of OOP. The key components are: 
- State: Attributes
- Methods(Functions): Behaviour
- Identity: Name/Address of the object that distinguishes objects

```c++
int main()
{
    Animal animal1 = Animal("dog", 4);
    animal1.makeSound();
}
```

## Constructors
A special method to instantiate an object and "construct" it. It is called automatically called when an object is created, in some cases to set intial values to its attributes. The name of the constructor is the same as the name of the class. 

## Destructors
A special method to "destruct" an object. It is automatically called when an object is destroyed, or when it goes out of scope. Its major functionality is cleanup, releasing resources, and prevent resource leaks. It takes no parameters and the name of the destructor is the same as the name of the class. 

## Access Modifiers
It sets the accessibility or visibility of the member data and methods. The different types of access modifiers are: 
- Public: Can be accessed from outside the class. Inherited classes can also access this.
- Private: Can't be accessed from outside the class. But inherited classes can't access this.
- Protected: Can't be accessed from outside the class. But inherited classes can access this.
- Default: In C++ and Java, by default they are set to private.

## Overloading
It enables multiple methods to have the same name but different parameters(no of parameters, or type of parameters, or both). It is a type of **static polymorphism**. Additionally, operators can also be overloaded to redifine the behaviour of certain operators for user-defined types(classes). It is just syntactic sugar, and can be achieved through functions as well. But it makes the code more intuitive and user-friendly. The type of overloading are: 
- Function Overloading
- Operator Overloading
  








