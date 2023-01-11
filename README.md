# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![OUTPUT](./crop_scr)

## DESIGN STEPS

### STEP 1:
    Commit all the updates

### STEP 2:
    Change the URL of the GitHub remote repository

### STEP 3:
    Push the changes in the branch to the Github repository


## PROGRAM
```
admin.py

    from django.contrib import admin
    from .models import Employee,EmployeeAdmin
    admin.site.register(Employee,EmployeeAdmin)

models.py

    from django.db import models
    from django.contrib import admin
    class Employee(models.Model):
        eid=models.CharField(max_length=20,help_text="Employee ID")
        name=models.CharField(max_length=100)
        salary=models.IntegerField()
        age=models.IntegerField()
        email=models.EmailField()

    class EmployeeAdmin(admin.ModelAdmin):
        list_display=('eid','name','salary','age','email')
```
## OUTPUT

![OUTPUT](./Output_Ex02.png)


## RESULT

THE PROGRAM HAS BEEN EXECUTED SUCCESSFULLY

