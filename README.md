# Ex02 Django ORM Web Application
# Date:o6.12.2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2024-12-07 152712](https://github.com/user-attachments/assets/3958c11c-8526-41f3-8878-a3e01953a301)

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
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
     serialno=models.IntegerField(primary_key="serialno");
     bookname=models.CharField(max_length=20);
     publisher=models.CharField(max_length=20);
     Dop=models.DateField();
     totalpg=models.IntegerField();
class Book_DBAdmin(admin.ModelAdmin):
     list_display=("serialno","bookname","publisher","Dop","totalpg");
```

# OUTPUT
![Screenshot 2024-12-07 152757](https://github.com/user-attachments/assets/6e6494be-393c-4364-b2a7-618f90ea5ddc)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
