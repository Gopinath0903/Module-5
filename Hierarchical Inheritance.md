# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to Get the employee  and patient details & display it using Hierarchical inheritance.
---

### ALGORITHM

1. **Start**
2. Define a base class `Details` with:

   * `id`, `name`, and `gender`
3. Define a class `Employee` that inherits from `Details`:

   * Add `company` and `department`
4. Define a class `Patient` that inherits from `Details`:

   * Add `hospital` and `department`
5. Take input for employee:

   * `id`, `name`, `gender`, `company`, `department`
6. Create `Employee` object
7. Display employee details
8. Take input for patient:

   * `id`, `name`, `gender`, `hospital`, `department`
9. Create `Patient` object
10. Display patient details
11. **End**



### PROGRAM
```
Reg  no-212223070007
Name-Gopinath G

# Base class
class Details:
    def __init__(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

    def display_basic(self):
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)

# Derived class: Employee
class Employee(Details):
    def __init__(self, id, name, gender, company, department):
        super().__init__(id, name, gender)
        self.company = company
        self.department = department

    def display_employee(self):
        print("\nEmployee Object")
        self.display_basic()
        print("Company: ", self.company)
        print("Department: ", self.department)

# Derived class: Patient
class Patient(Details):
    def __init__(self, id, name, gender, hospital, department):
        super().__init__(id, name, gender)
        self.hospital = hospital
        self.department = department

    def display_patient(self):
        print("\nPatient Object")
        self.display_basic()
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)

# Get Employee details
emp_id = int(input())
emp_name = input()
emp_gender = input()
emp_company = input()
emp_dept = input()

# Create Employee object
employee = Employee(emp_id, emp_name, emp_gender, emp_company, emp_dept)

# Get Patient details
pat_id = int(input())
pat_name = input()
pat_gender = input()
pat_hospital = input()
pat_dept = input()

# Create Patient object
patient = Patient(pat_id, pat_name, pat_gender, pat_hospital, pat_dept)

# Display both
employee.display_employee()
patient.display_patient()


```

### OUTPUT  
![image](https://github.com/user-attachments/assets/e93d5231-d583-4640-9f23-87aab3b5e96a)


### RESULT
Thus the Python program to Get the employee  and patient details & display it using Hierarchical inheritance  was executed successfully.
