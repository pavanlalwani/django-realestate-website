# Real Estate Website (Using Django framework)

This project is consistent with the Udemy course [Python Django Dev To Deployment](https://www.udemy.com/course/python-django-dev-to-deployment/) by Brad Traversy.

## Instructions
 
### Prerequisites
After setting up PostgreSQL 10 on your machine, run the following on the prompt

```
CREATE DATABASE btredb OWNER postgres;
```


Configure database login credentials in file /btre/settings.py 


```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'btredb',
        'USER' : '<USERNAME>',
        'PASSWORD' : '<PASSWORD>',
        'HOST' : 'localhost'
     }
}
``` 
### Execution
```python3 manage.py runserver``` to run the project on localhost.

## Features
* Customized admin area to control Listings, Realtors, Contact inquiries and be consistent with the main site theme.
* Pagination & Lightbox for images in Listings.
* User can register/login to send inquiries to a realtor about a listing. Inquiry form saved in database and emailed to Realtor.
* Ability to set Listings as unpublished, via admin area and control "Seller of the month" to be displayed on "About" page.
* Registered users can submit only 1 inquiry per listing.
