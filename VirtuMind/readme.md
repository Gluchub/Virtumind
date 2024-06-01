how to render models in view 

#use the followinng commands

for rendering all commands and attribute use
- ModelName.objects.all()

To render the specific model
- ModelName.objects.get()

how to setup the login dartabase
    for  that first we need to import smth in the models.py file
    -from django.contrib.auth.models import User

for deleting anything
    from django.db.models.deletion import CASCADE

for going back to previous page by clicking the button do attach the following link in the link component if you are using django
example:
    <a href="{{request.META.HTTP_REFERER}}">Go back</a>

there is also a create function for models and for excessing it :
suppose Message be the model
Model.objects.create(
    {userdatas}
)


*how to configure the static folder

    1- create static folder in main directory
    2- create styles folder in the static folder
    3- create images folder in the static folder 
    4- create main.css file in the styles folder

    create STATICFILES_DIRS under STATIC_URLS variable in settings.py 
    like this
    - STATICFILES_DIRS=[
        BASE_DIR / 'static'
    ]

    now in thhe templates folder in main.html file
    paste the following link:

    <link rel="stylesheet" type="text/css" media="screen" href="{% static 'styles/main.css' %}">

    and the following command above the html tag

    {% load static %}


