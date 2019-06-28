# Movies API

This is an API interface to search for movies having different filters to search by name, imdb score, director and genres.
You can use order filter on different fields. And direct search from filter search for given keyword.

There are two layer of access. An admin user can add, remove or edit movies. Other users can only view the search result. And any unauthorized request can't even see the movies.

I have added plenty of fliter to the project as well.

######admin => can add, remove or edit movies.
######staff => can just view the movies.
######users => can just view the movies.

## Steps to make project up and running

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


This project is also deployed on [Heroku](https://sleepy-caverns-15668.herokuapp.com)

###### ```python3 manage.py dump_movies``` This will dump the data from json file to the database using imdb.json provided on the project.
###### Note: I have used pip3 and python3, you can use python version 2 if you like.
