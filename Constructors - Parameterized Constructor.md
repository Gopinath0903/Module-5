# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
To write a  python program using class to perform addition of two numbers using parameterised constructor.
---

### ALGORITHM

1. **Start**
2. Define a class called `Addition`
3. Inside the class, define:

   * A constructor method to initialize two numbers (`num1` and `num2`)
   * A method `calculate()` to compute the sum of the two numbers
   * A method `display()` to print the numbers and their sum
4. Take two integer inputs from the user
5. Create an object of the `Addition` class using the inputs
6. Call the `calculate()` method to perform addition
7. Call the `display()` method to show the result
8. **End*

---

### PROGRAM

```
Reg no-212223070007
Nmae-Gopinath G

class Addition:
    first=0
    second=0
    answer=0
    def __init__(self,num1,num2):
        self.num1=num1
        self.num2=num2
    def display(self):
        print("First number = "+str(self.num1))
        print("Second number = "+str(self.num2))
        print("Addition of two numbers = "+str(self.answer))
    def calculate(self):
        self.answer=self.num1+self.num2
x=int(input())
y=int(input())
obj = Addition(x,y)
obj.calculate()
obj.display()
```

### OUTPUT
![image](https://github.com/user-attachments/assets/5ea7dbf5-b56f-4d22-8080-d4e3d2f0d328)

### RESULT
Thus the python program using class to perform addition of two numbers using parameterised constructor wass executed successfully
