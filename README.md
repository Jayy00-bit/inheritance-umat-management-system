# Inheritance-UMaT-Management-System
Case Study Activity: UMaT Management System

# UMaT Management System

A simple Python case study demonstrating **Object-Oriented Programming (OOP)** concepts — specifically inheritance and method overriding — through a mock student/lecturer management system for UMaT (University of Mines and Technology).

# Overview

This project was built as part of a lab session case study activity. It models two types of people within a university system, `Student` and `Lecturer`, both of which inherit shared attributes and behavior from a common `Person` base class.

#  Class Structure

### `Person` (Base Class)
| Attribute | Description |
|---|---|
| `name` | Full name of the person |
| `age` | Age of the person |

**Methods:**
- `display_info()` — Prints the person's name and age.

### `Student` (inherits from `Person`)
Adds student-specific attributes on top of `Person`.

| Attribute | Description |
|---|---|
| `student_id` | Unique student identifier |
| `enroll_course` | Enrollment status (`True`/`False`) |

**Methods:**
- `display_info()` — Overrides the parent method to print full student details, including ID and enrollment status.

### `Lecturer` (inherits from `Person`)
Adds lecturer-specific attributes on top of `Person`.

| Attribute | Description |
|---|---|
| `employee_id` | Unique employee identifier |
| `teach_course` | Teaching status (`True`/`False`) |

**Methods:**
- `display_info()` — Inherited directly from `Person` (not overridden).
- `show_more_info()` — Prints additional lecturer-specific details.

##  Example Usage

```python
student = Student("Jayy", 18, 9016915325, True)
student.display_info()

lecturer = Lecturer("Dr.Matthew Cobbinah", 40, "12/06/89", True)
lecturer.display_info()
lecturer.show_more_info()
```

### Sample Output

```
This is Jayy 
He is 18 
He has Student ID 9016915325 
Course Enrollment Status = True
Name:Dr.Matthew Cobbinah, Age:40
Here stands a Honorable Lecturer with Employee_id: 12/06/89 and Course Teaching Status: True 
```

##  Key Concepts Demonstrated

- **Inheritance** — `Student` and `Lecturer` both extend the `Person` class.
- **Method Overriding** — `Student` overrides `display_info()` with custom formatting, while `Lecturer` uses the inherited version unchanged.
- **`super().__init__()`** — Used to initialize inherited attributes (`name`, `age`) from the parent class.
- **Encapsulation of role-specific data** — Each subclass manages attributes relevant only to its role.

##  Requirements

- Python 3.x
- Jupyter Notebook (to run the `.ipynb` file)

## Files

| File | Description |
|---|---|
| `UMaT Management System.ipynb` | Jupyter notebook containing the full case study code and output |

##  Running the Notebook

1. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
2. Open `UMaT Management System.ipynb` and run all cells.

## Author
Tannoh Andrews Jezreel  
EL1B, Electrical And Electronic Engineering  
University of Mines And Technology(UMaT),Tarkwa
