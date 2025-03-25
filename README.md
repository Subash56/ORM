# Ex02 Django ORM Web Application
# Date:24/03/25
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
admin.py:
```
from django.contrib import admin                                             
from .models import book,bookAdmin                                           
admin.site.register(book,bookAdmin)
```
Models.py
```
from django.db import models                                                                                                                      
from django.contrib import admin                                             
class book(models.Model):                    				      
   bookno=models.IntegerField(primary_key=True);                                                      
   authorname=models.CharField(max_length=50);                                                            
   price=models.IntegerField(help_text="enter price");                       
   qty=models.IntegerField();                                                
   bookname=models.CharField(max_length=50);                                 
class bookAdmin(admin.ModelAdmin):                                           
   list_display=("bookno","authorname","price","qty","bookname");
   ```
# OUTPUT
Include the screenshot of your admin page.
![alt text](image.png)
![alt text](image-1.png)
# RESULT
Thus the program for creating a database using ORM hass been executed successfully
