# Django ORM Web Application

## AIM:
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:
![entity diagram](https://user-images.githubusercontent.com/122762773/230107024-e6dd7279-b88e-466f-a1c3-a9d1255116b5.png)


## DESIGN STEPS:

### STEP 1:
A Django application is created inside dataproject folder.
### STEP 2:
A python program is written to create a table to store and retrieve data.
### STEP 3:
Then the project files migrated. A superuser is also created.
### STEP 4:
Now the server side program is executed .
### STEP 5:
The admin page of our website is accessed using username and password.
### STEP 6:
Records are added and saved in the table inside the database.

## PROGRAM:
```
from django.db import models
from django.contrib import admin

class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```

## OUTPUT:


![django](https://user-images.githubusercontent.com/122762773/230101993-ffd6f7f0-efb3-40f6-bda9-3701e0171699.png)


## RESULT:
Thus a Django application is successfully developed to store and retrieve data from a database using Object Relational Mapping(ORM).
