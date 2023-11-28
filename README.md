# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![SANJAY ER DIAGRAM](https://github.com/sanjayofficial2005/django-orm-app/assets/148048602/1248b241-cc35-4d1a-be2b-908e863f24be)


## DESIGN STEPS

### STEP 1:
close the empty repository from gitup

### STEP 2:
under the directory Dataproject install a Django project named 'myapp'.check database engine 'sqlite'.

### STEP 3:
write our code in models.py and setting.py and admin.py.Run Django Project

Write your own steps

## PROGRAM
### models.py:
```python

models.py
from django.db import models 
from django.contrib import admin

create your models here.
class Student (models.Model): 
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    mobileno=models.IntegerField()

    class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','mobileno')

admin.py

 from django.contrib import admin
from .models import Student,StudentAdmin

# Register your models here.
admin.site.register(Student,StudentAdmin)
```



## OUTPUT

![studentuser](https://github.com/sanjayofficial2005/django-orm-app/assets/148048602/7a921837-176b-4e16-81b7-90170d1a0696)



## RESULT
The program is executed succesfully
