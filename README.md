# API to search Movies or any data in database

This is an API interface to search for movies having different filters to search by name, imdb score, director and genres.
You can use order filter on different fields. And direct search from filter search for given keyword.

There are two layer of access. An admin user can add, remove or edit movies. Other users can only view the search result. And any unauthorized request can't even see the movies.


###### admin => can add, remove or edit movies.
###### staff => can just view the movies.
###### users => can just view the movies.

## Steps to make project up and running

###### Note: If you decide to download and deploy the project locally then its better that you first flush the database and for that use the below command. 
```
python3 manage.py flush
```
### create a virtual environment
```
python3 -m venv env
source env/bin/activate
```
### Install required packages
```
pip3 install -r reuqirements.txt
```
### Commandas to initiate the project
```
python3 manage.py migrate
python3 manage.py createsuperuser
python3 manage.py dump_movies
python3 manage.py runserver
```


This project is also deployed on [Heroku](https://sleepy-caverns-15668.herokuapp.com).
###### username - admin
###### password - Passw0rd
For staff and user
###### username - staff or user
###### password - Passw@rd

###### ```python3 manage.py dump_movies``` This will dump the data from json file to the database using imdb.json provided on the project.


###### I have used pip3 and python3 for the project, you can use python version 2 if you like.
