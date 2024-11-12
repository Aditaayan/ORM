# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![image](https://github.com/user-attachments/assets/8843c903-daa6-462e-a09f-657caa8e2f00)


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

# Register your models here.
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin)
```

```
models.py

from django.db import models

# Create your models here.
from django.contrib import admin
class bankloan(models.Model):
    accno=models.IntegerField(primary_key=True);
    name=models.CharField(max_length=100);
    loanamt=models.IntegerField();
    loanlimit=models.IntegerField();
    phoneno=models.IntegerField();

class bankloanAdmin(admin.ModelAdmin):
    list_display=('accno','name','loanamt','loanlimit','phoneno')
```

## OUTPUT

![image](https://github.com/user-attachments/assets/115231fd-0372-4dcd-9ab8-cc245546ffde)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
