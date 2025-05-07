# Exp.No:30  
## POLYMORPHISM

---

### AIM  
To create two classes Cat and Dog. They share a similar structure and have the same method names info() and make_sound() pack these two different objects into a tuple and iterate through it using a common animal variable. It is possible due to polymorphism.

---

### ALGORITHM

1. Define the Cat class:
- Initialize with parameters name and age.
- Define a method make_sound() that prints "Meow".
- Define a method info() that prints the cat's name and age.
2. Define the Dog class:
- Initialize with parameters name and age.
- Define a method make_sound() that prints "Bark".
- Define a method info() that prints the dog's name and age.
3. Take input from the user:
- Input cname: name of the cat.
- Input cage: age of the cat.
- Input dname: name of the dog.
- Input dage: age of the dog.
4. Create objects:
- Create cat1 object from the Cat class using cname and cage.
- Create dog1 object from the Dog class using dname and dage.
5. Iterate through the animals (cat1 and dog1):
- For each animal in the tuple (cat1, dog1):
  - Call make_sound() → prints the animal sound.
  - Call info() → prints the animal's name and age.
  - Call make_sound() again → prints the sound once more.

---

### PROGRAM

```
class Cat:
    def __init__(self,name,age):
        self.name = name
        self.age = age
    def make_sound(self):
        print("Meow")
    def info(self):
        print(f"I am a cat. My name is {self.name}. I am {self.age} years old.")
    #Add your code here

class Dog:
    def __init__(self,name,age):
        self.name = name
        self.age = age
    def make_sound(self):
        print("Bark")
    def info(self):
        print(f"I am a dog. My name is {self.name}. I am {self.age} years old.")
    #Add your code here
cname=input()
cage=input()
dname=input()
dage=input()
cat1 = Cat(cname,cage)
dog1 = Dog(dname,dage)

for animal in (cat1, dog1):
    animal.make_sound()
    animal.info()
    animal.make_sound()

```

### OUTPUT

![image](https://github.com/user-attachments/assets/46c9173a-b136-4896-bb3b-2588978716b7)

### RESULT
Thus the program to create two classes Cat and Dog was implemented and executed successfully.
