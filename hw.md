## Homework

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

To change form. 

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

It is the ability for a method to take on different forms when applied to different objects.

`public String outputData(String data) {
        return this.print(data);
    }` 

`public interface iDataOutput {

    String outputData(String data);



}`

3. What can we use to implement polymorphism in Java?

Examples of how polymorphism can be implemented are the use of methods from an implemented interface, method overriding/overloading within a subclass and inheritance of abstract methods.  

4. How many 'forms' can an object take when using polymorphism?

an object can change forms as many times as you allow for in the code. 

5. Give an example of when you could use polymorphism.

 `public void setOutputDevice(iDataOutput newOutputDevice){
         this.outputDevice = newOutputDevice;`
    }



---

# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

composition refers to a high dependency relationship in which a class object is necessary to another class object's existence. 

7. When would you use composition? Provide a simple example in Java.

`public Computer(int ram, int hddSize, iDataOutput outputDevice) {
        this.ram = ram;
        this.hddSize = hddSize;
        this.outputDevice = outputDevice;
    }`

8. What is/are the advantage(s) of using composition?

Composition allows for concepts to be broken down into smaller parts for simplification and seperation. Separation is useful if some parts will have certain behaviours that others won't. 

9. What happens to the behaviours when the object composed of them is destroyed?
the particular instances of those behaviours will be destroyed but the super class or interfaces containing those behaviours are still in existence to give them to any class that extends or implements them. 
