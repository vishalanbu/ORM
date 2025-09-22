# Ex02 Django ORM Web Application
# Date:22/09/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
  models.py
  
from django.contrib import admin
class Car(models.Model):
    car_id = models.AutoField(primary_key=True)  
    brand = models.CharField(max_length=50)
    model = models.CharField(max_length=50)
    year = models.IntegerField()
    fuel_type = models.CharField(max_length=20)
    mileage = models.IntegerField()
    color = models.CharField(max_length=30)
    price=models.DecimalField (max_digits=10, decimal_places=2)
class CarAdmin(admin.ModelAdmin):
     list_display = ('car_id', 'brand', 'model', 'year','fuel_type', 'mileage', 'color')

     
     admin.py
     from django.contrib import admin
from .models import Car

class CarAdmin(admin.ModelAdmin):
    list_display = ('car_id', 'brand', 'model', 'year', 'fuel_type', 'mileage', 'color')

admin.site.register(Car, CarAdmin)
  ```
    
# OUTPUT

![alt text](<../Screenshot 2025-09-22 101742.png>)
Include the screenshot of your admin page.

# RESULT
Thus the program for creating a database using ORM hass been executed successfully

# OUTPUT
Include the screenshot of your admin page.

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
