# Django ORM Web Application

## AIM:
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram:
![image](https://user-images.githubusercontent.com/121222763/234187796-cec217bb-252a-465b-97d9-a8a31bfaa799.png)

## DESIGN STEPS:

### STEP 1:
clone the repository from github.
### STEP 2:
create an admin interface for django.
### STEP 3:
create an app and edit settings.py
### STEP 4:
make migrations and migrate the changes.
### STEP 5:
create admin user and write python code for admin and models.
### STEP 6:
make all the migrations to 'myapp'.
### STEP 7:
create an student database with 10 fields using runserver command.

## PROGRAM:
```python
admin.py

from django.contrib import admin
from.models import student,studentAdmin
admin.site.register(student,studentAdmin)

models.py

from django.db import models
from django.contrib import admin
class student(models.Model):
    sid=models.CharField(max_length=200)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class studentAdmin(admin.ModelAdmin):
    list_display=('sid','name','salary','age','email')
```

## OUTPUT:
## CLIENT OUTPUT:
![image](https://user-images.githubusercontent.com/121222763/234188444-09a1e768-9be5-4934-9222-9aa716e7d0bf.png)
## SERVER OUTPUT:
![image](https://user-images.githubusercontent.com/121222763/234188564-580e6b6b-6ce3-417b-afd5-fb6f2b213161.png)

## RESULT:
The program for creating an student database using ORM is executed sucessfully.


