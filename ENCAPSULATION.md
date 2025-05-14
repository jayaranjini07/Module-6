# Exp.No:29  
## Encapsulation

---

### AIM  
To create a class student with members name ,age,rollno and an user defined function show() to display the details of the student ,use the getter and setter method Information Hiding and conditional logic for setting an object attributes.

---

### ALGORITHM

1. **Start the Program.**
2. Define a class Student with:
- An __init__ constructor method that initializes:
  - name (public attribute)
  - __roll_no and __age (private attributes, using double underscores)
4. Create a method show() to display the student's name and roll number.
5. Create a getter method get_roll_no(): Returns the value of private member __roll_no.
6. Create a setter method set_roll_no(number):
- Checks if number > 50:
  - If yes, it prints a warning and does not update __roll_no.
  - If no, it updates __roll_no to the given number.
7. Create an object jessa with:
-name = 'Jessa', roll_no = 10, age = 15
8. Call jessa.show(): Displays: "Student Details: Jessa 10"
9. Call jessa.set_roll_no(120):
- Since 120 > 50, the setter rejects the change and prints:
 - "Invalid roll no. Please set correct roll number"
10. Call jessa.set_roll_no(25):
- Since 25 ≤ 50, the setter updates __roll_no to 25.
11. Call jessa.show() again: Displays: "Student Details: Jessa 25"
12. **End the program.**

---

### PROGRAM

```
class Student:
    def __init__(self, name, roll_no, age):
        # private member
        self.name = name
        # private members to restrict access
        # avoid direct data modification
        self.__roll_no = roll_no
        self.__age = age

    def show(self):
        print('Student Details:', self.name, self.__roll_no)

    # getter methods
    def get_roll_no(self):
        return self.__roll_no

    # setter method to modify data member
    # condition to allow data modification with rules
    def set_roll_no(self, number):
        if number > 50:
            print('Invalid roll no. Please set correct roll number')
        else:
            self.__roll_no = number

jessa = Student('Jessa', 10, 15)
jessa.show()
# before Modify
# call show()
jessa.set_roll_no(120)
# changing roll number as 120 using setter



jessa.set_roll_no(25)
jessa.show()

```

### OUTPUT

![image](https://github.com/user-attachments/assets/28a9e23c-873d-4b4c-9c5b-2ab444b75427)

### RESULT
Thus the python program to create a class student with members name ,age,rollno and an user defined function show() to display the details of the student ,use the getter and setter method Information Hiding and conditional logic for setting an object attributes was implemented and executed successfully.
