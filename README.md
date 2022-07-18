**In summary, in object oriented programming, each object has three dimensions: identity, attributes, and behavior. **

**attributes** : - the current state of an object is called attributes.

Objects also have characteristics, which are used to describe them.
For example, a car can be red or blue, a mug can be full or empty, and so on. .
These characteristics are also called attributes. 
An attribute describes the current state of an object. 

**behavior** : - behavior is specific to the object's type.

In the real world, each object behaves in its own way. 
The car moves, the phone rings, and so on.
The same applies to objects: behavior is specific to the object's type. 

** A class defines 1. Behaviour and 2. Attributes**

**The keyword void**

Notice the void keyword in the definition of the main method
- this means that main does not return anything.

**Dot notation**

The dot notation is used to access the object's attributes and methods. 

**Defining Attributes**

 The attributes are basically variables within a class. 

**Access Modifiers**

You can use access modifiers for classes, attributes, and methods. 

**For classes, the available modifiers are public or default (left blank), as described below:**

**public:** The class is accessible by any other class.
**default:** The class is accessible only by classes in the same package. 

**The following choices are available for attributes and methods: **

**default:** A variable or method declared with no access control modifier is available to any other class in the same package.
**public:** Accessible from any other class.
**protected:** Provides the same access as the default access modifier, with the addition that subclasses can access protected methods and variables of the superclass (Subclasses and superclasses are covered in upcoming lessons).
**private:** Accessible only within the declared class itself. 

**Getter and Setter**

Getters and Setters are used to effectively protect your data, particularly when creating classes.
For each variable, the get method returns its value, while the set method sets the value. 

simple rules :
         Getters start with get, followed by the variable name, with the first letter of the variable name capitalized.
         Setters start with set, followed by the variable name, with the first letter of the variable name capitalized. 

**Constructors**


A single class can have multiple constructors with different numbers of parameters.
The setter methods inside the constructors can be used to set the attribute values. 


**Example:**
    

    public class Vehicle {

      private String color;

      Vehicle() {

        this.setColor("Red");

      }

      Vehicle(String c) {

        this.setColor(c);

      }

      // Setter
      public void setColor(String c) {

        this.color = c;

      }
    }


**Static**

When you declare a variable or a method as static, it belongs to the class, rather than to a specific instance.
This means that only one instance of a static member exists, even if you create multiple objects of the class, or if you don't create any. 
It will be shared by all objects.

**Example**

    public class Counter {

      public static int COUNT=0;

      Counter() {

        COUNT++;

      }

    }

The COUNT variable will be shared by all objects of that class.
Now, we can create objects of our Counter class in main, and access the static variable. 

**It’s a common practice to use upper case when naming a static variable, although not mandatory.**

**Static Method**

  The same concept applies to static methods.

    public class Vehicle {
        public static void horn() {
            System.out.println("Beep");
        }
    }

    public class MyClass {
        public static void main(String[ ] args) {
            Vehicle.horn();
        }
    }


**final keyword**

Use the final keyword to mark a variable constant, so that it can be assigned only once. 

