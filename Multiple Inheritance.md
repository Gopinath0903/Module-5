# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance and Id of a student and check they are eligible for Next Module using multiple inheritance.
---

### ALGORITHM

1. **Start**
2. Input `name`
3. Input `attendance`
4. Input `id` (used as attendance percentage)
5. If `id` > 75
     → Print name, attendance, and "Eligible for Module Exam"
6. Else
     → Print name, attendance, and "Not Eligible for Module Exam"
7. **End**

---

### PROGRAM

```
Reg no-212223070007
Name-Gopinath G

class one():
    def student1(self,name,att,id):
        print(name)
        print(att)
        print("Eligible for Module Exam")
class two():
    def student2(self,name,att,id):
        print(name)
        print(att)
        print("Not Eligible for Module Exam")
class valid(one,two):
    def valid(self,name,att,id):
        if id>75:
            one().student1(name,att,id)
        else:
            two().student2(name,att,id)
name=input()
att=int(input())
id=int(input())
x=valid()

x.valid(name,att,id)
```

### OUTPUT
![image](https://github.com/user-attachments/assets/4a23fb76-9ab8-4eba-8f65-a5ecb3bf2771)


### RESULT
Thus the Python program to get the name, attendance and Id of a student and check they are eligible for Next Module using multiple inheritance was executed successfully




