# Ex02 Django ORM Web Application
# Date: 18/10/2024
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
admin.py

from django.contrib import admin 
from.models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)

models.py

from django.db import models
from django.contrib import admin
class Loan(models.Model):
        Name=models.CharField(max_length=10)
        Accountno=models.IntegerField(primary_key="Refno")
        Address=models.CharField(max_length=30)
        Aadharno=models.IntegerField()
        Email=models.EmailField()
class LoanAdmin(admin.ModelAdmin):
         list_display=('Name','Accountno','Address','Aadharno','Email')
```
# OUTPUT
![Screenshot 2024-12-16 002006](https://github.com/user-attachments/assets/6130e691-f2c5-4140-892f-957c15a71973)

![Screenshot 2024-12-07 231733](https://github.com/user-attachments/assets/4e4c3414-44d3-4e1c-bf7a-5ae19d0d132d)

![Screenshot 2024-12-07 231657](https://github.com/user-attachments/assets/8fe61218-5229-4171-9be5-bf9c9191dbde)

![Screenshot 2024-12-07 231611](https://github.com/user-attachments/assets/f6e56d40-f08c-4828-9f82-0d61fee5f63e)




# RESULT
Thus the program for creating a database using ORM hass been executed successfully
