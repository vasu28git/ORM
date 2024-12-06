# Ex02 Django ORM Web Application
# Date:28-10-2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![entity diagram ORM](https://github.com/user-attachments/assets/0cd750e9-0f7b-4a5b-b6cc-4867a8c8502d)

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
admin.py
~~~
from django.contrib import admin
from .models import book,bookadmin
admin.site.register(book,bookadmin)
~~~
models.py
~~~
from django.db import models
from django.contrib import admin
class book(models.Model):
    Book_name=models.CharField(max_length=100)
    Author=models.CharField(max_length=100)
    Co_author=models.CharField(max_length=100)
    Book_code=models.IntegerField()
    Publisher=models.CharField(max_length=100)
    MRP=models.IntegerField()
class bookadmin(admin.ModelAdmin):
    list_display=("Book_name","Author","Co_author","Book_code","Publisher","MRP")
~~~
# OUTPUT
![userbooks](https://github.com/user-attachments/assets/5e16010f-af7d-4481-bc5a-cdcfd275913a)

![users](https://github.com/user-attachments/assets/f78774d7-6a2e-4fa7-b121-ecf44a463704)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
