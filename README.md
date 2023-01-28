# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://user-images.githubusercontent.com/118708624/215239773-a39d9a15-1ff0-41bf-9ea9-0c78837ca380.png)

## DESIGN STEPS

### STEP 1:Clone the repository from GitHub

### STEP 2:Create Django admin user interface

### STEP 3:Create admin and models python programs for implementing employee database

## PROGRAM
```
models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
     list_display=('eid','name','salary','age','email')   

admin.py

from django.contrib import admin
from.models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```
## OUTPUT
![image](https://user-images.githubusercontent.com/118708624/215239902-7e8b7257-a960-4f6c-aa15-66b07d545e9b.png)



## RESULT
Program executed sucessfully
