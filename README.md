# Ex02 Django ORM Web Application

## Date: 04-04-24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

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
Models.py

from django.db import models
from django.contrib import admin

class footballplayer (models.Model):
    numofmatch=models.IntegerField()
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    height=models.IntegerField()

class footballplayerAdmin(admin.ModelAdmin):
    list_display=('numofmatch','name','salary','age','height')

Admin.py

from django.contrib import admin
from .models import footballplayer,footballplayerAdmin
admin.site.register(footballplayer,footballplayerAdmin)

```


## OUTPUT


![Screenshot 2024-04-04 093429](https://github.com/Ranjanranjan/ORM/assets/130027697/edf005b9-e3d0-46c3-b1fe-59b120c607c6)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
