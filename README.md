# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://github.com/Rajaraman77/ORM/assets/150319383/9991f641-acaf-4820-9fac-5035e7e1131b)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
## admin.py
from django.contrib import admin
from .models import books,booksAdmin
admin.site.register(books,booksAdmin)
## modal.py
from django.db import models
from django.contrib import admin
class books(models.Model):
	name=models.CharField(max_length=20);
	author=models.CharField(max_length=20);
	id=models.IntegerField(primary_key=True);
	copies=models.IntegerField();
	price=models.IntegerField();
class booksAdmin(admin.ModelAdmin):
	list_display=("name","author","id","copies","price");
```
## OUTPUT
![image](https://github.com/Rajaraman77/ORM/assets/150319383/d7f329ae-e3fb-4c4c-a6eb-b6f24ad074b8)
![image](https://github.com/Rajaraman77/ORM/assets/150319383/ddf1085f-bf5e-4400-8d0f-307747462072)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
