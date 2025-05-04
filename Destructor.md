# Exp.No:22  
## Destructor

---

### AIM  
Add destructor in the following python code
---

### ALGORITHM

1. **Start**
2. Define a class `Person`
3. Inside the class:

   * Create a constructor to accept `name` and `age`
   * Print "Person Created" inside the constructor
   * Create a `display()` method to print name and age
   * Define a destructor to print "`name` Object Destroyed"
4. Take `name` as input from the user
5. Take `age` as input from the user
6. Create an object of the `Person` class using the input values
7. Call the `display()` method to show the data
8. Delete the object to trigger the destructor (optional)
9. **End**


### PROGRAM

```
Reg no-212223070007
Name-Gopinath G

class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
        print("Person Created")

    def display(self):
        print(f"{self.name} {self.age}")

    def __del__(self):
        print(f"{self.name} Object Destroyed")

# Example usage:
name_input = input()
age_input = int(input())

person1 = Person(name_input, age_input)
person1.display()

# Optional: manually delete to trigger destructor immediately
del person1
```

### OUTPUT
![image](https://github.com/user-attachments/assets/8d5c404c-d504-4578-87d1-c951225cf844)


### RESULT
Thus the Add destructor in the following python code was executed successfully
