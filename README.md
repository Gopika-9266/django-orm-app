# Django ORM Web Application

## AIM:
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:


![entity diragram](https://user-images.githubusercontent.com/122762773/231185475-22ae2400-8385-4c43-80db-22b003a1222b.png)

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
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    department=models.CharField(max_length=100)


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','department')
  

```

## OUTPUT:


![django orm app](https://user-images.githubusercontent.com/122762773/231179332-4b5d59bb-cd38-421d-81e4-6eb06937da67.png)



## RESULT:
Thus a Django application is successfully developed to store and retrieve data from a database using Object Relational Mapping(ORM).
