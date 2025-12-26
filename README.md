# Ex02 Django ORM Web Application
## Date: 9.11.2025

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 5 Car 

## PROGRAM
```
models.py
from django.db import models
from django.contrib import admin
class Car(models.Model):
    car_name= models.CharField()
    car_model = models.CharField()
    release_date = models.DateField()
    millage = models.IntegerField()
    color = models.CharField()

class CarAdmin(admin.ModelAdmin):
    list_display = ('car_name', 'car_model', 'release_date', 'millage', 'color')
   
admin.py
from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin)
```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/948ae4a6-cbd3-4052-8977-0dbf40ecc68d" />




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
