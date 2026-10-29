solid principles/ design principles
s -> single responsibility principle(srp)
o - > open close principle
l - > liskov substituion principle
i -> interface segragation principle
d - > dependency inversion principle

![alt text](image.png)

![alt text](image-1.png)

instead of modifying the code
just use abstract class 
and have the existing and new 
class be inherited from the abstract class

![alt text](image-2.png)
Liskov is broken most of the time in production  

![alt text](image-6.png)

in this case , account has two methods deposit and withdraw
if there is new type of account which can't withdraw then we can't do it 
and since tha account class is abstract it will throw exception 
![alt text](image-7.png)

![alt text](image-8.png)
it is bad to have some other data type in the overriding because it breaks the contract that is 
the abstraction class
it is a promise that the classes that will be inherited will follow this contract and this contracts says string . 

so the language independent rule is to have either the same datatype or broader datatype of this stuff. 

![alt text](image-9.png)

![alt text](image-10.png)

all good with this one (image 10)
return narrow or same type in returning but not it's broader type
![alt text](image-11.png)

![alt text](image-12.png)


google - docs system design
![alt text](image-13.png)
![alt text](image-14.png)
starts to look like this below image
![alt text](image-15.png)
![alt text](image-16.png)
solution -> strategy design pattern
![alt text](image-17.png)
![alt text](image-18.png)
now just pass the property that u want in the robot and i can choose any permutation 
to get whatever i need.
this makes it runtime 
consclusion -> composition > inheritance


now comes factory design pattern -> separate business logic and object creation logic
![alt text](image-19.png)
![alt text](image-20.png)
here the business logic is separate and is in different file
![alt text](image-21.png)

Abstract factory method
![alt text](image-22.png)
![alt text](image-23.png)

![alt text](image-24.png)



singleton design pattern
it prints 0 so we want something so that only one instance is allowed
![alt text](image-25.png)
![alt text](image-26.png)
using mutex
![alt text](image-27.png)
