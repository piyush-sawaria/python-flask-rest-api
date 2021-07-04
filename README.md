# python-flask-rest-api
Rest api using python flask

### install virtualenv
- pip3 install virtualenv
- virtualenv venv --python=python3.9.6
- source venv/bin/activate

### install Flask-RESTful 
- pip install Flask-RESTful

### Apis
- for generating jwt
```
curl --location --request POST 'http://127.0.0.1:5000/auth' \
--header 'Content-Type: application/json' \
--data-raw '{
    "username": "user1",
    "password": "abcxyz"
}'
```
- by using jwt
```
curl --location --request GET 'http://127.0.0.1:5000/item/table' \
--header 'Authorization: JWT eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MjU0MTYxNDAsImlhdCI6MTYyNTQxNTg0MCwibmJmIjoxNjI1NDE1ODQwLCJpZGVudGl0eSI6MX0.cXBO9Y3ori7p2VyEa4w4gCHs_CQBv9qSYEsQpAVy9ZM' \
--header 'Content-Type: application/json'
```