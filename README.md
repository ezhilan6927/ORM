# Ex02 Django ORM Web Application
## Date: 
20/3/2024
## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://github.com/ezhilan6927/ORM/assets/160242249/5af27704-fcd8-4585-b2df-a3f1b168f848)


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
admin.py

from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)

models.py

from django.db import models
from django.contrib import admin
class Book(models.Model):
    book_id=models.IntegerField(primary_key=True)
    book_name=models.CharField(max_length=50)
    publisher_name=models.CharField(max_length=50)
    author_name=models.CharField(max_length=50)
    publisher_year=models.IntegerField()

class BookAdmin(admin.ModelAdmin):
    list_display=('book_id','book_name','publisher_name','publisher_year','author_name')
```

## OUTPUT

![image](https://github.com/ezhilan6927/ORM/assets/160242249/f4541b99-062a-4548-8bba-618e2828ff60)
![image](https://github.com/ezhilan6927/ORM/assets/160242249/903a4141-db41-4f4f-83b6-5b083c617d60)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
