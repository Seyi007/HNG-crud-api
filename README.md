# HNG CRUD API 
A simple REST API capable of CRUD operations on a "person" resource, interfacing with Postgres database using psycopg. The API dynamically handles parameters, adds or retrieves a person by name.
 
 - Source file here: [crud.py](https://github.com/Seyi007/HNG-crud-api/blob/main/api/crud.py)

## REST API Development:
API endpoints fuction:
- CREATE: Adding a new person.  ` /api`
- READ: Fetching details of a person.  => `/api/user_id`
- UPDATE: Modifying details of an existing person => `/api/user_id`
- DELETE: Removing a person => `/api/user_id`

## Run App
To run app:
- Clone repo: `git clone https://github.com/Seyi007/HNG-crud-api.git`

- Enter into project repo: `cd HNG-crud-api`
- Enter into file directory: `cd api`
- Install dependencies: `pip install -r requirement.txt`
- To start developent: `flask --app crud run`


## API Usage
- Create person: POST request to `https://hng-crud-api-500v.onrender.com/api` then send data through request body, eg: `{"name": "Daisy"}`.

- Get person: GET request to `https://hng-crud-api-500v.onrender.com/api/<person id>`, it returns person `id` and `name` eg: `{"id": <person id>, "name": "<person name>"`.
- Update person: PUT request to `https://hng-crud-api-500v.onrender.com/api/<person id>`, the send data through request body eg: `{"name": "<new name>"}`. it returns a success message with new name.

- Delete person: DELETE request to `https://hng-crud-api-500v.onrender.com/api/<person id>`, it retrun a success message.

## UML Diagram
- ![alt text](https://lucid.app/lucidchart/67c04a12-250a-4061-a1e4-63c3ba5d9ee8/edit?invitationId=inv_df8649ea-4021-409b-b3b0-07e1b1744c17)
## Authors

- [@seyi007](https://www.github.com/seyi007)


## Tech stack
- Python
- flask
- Json
- gunicorn
- psycopg2

## Test
- Postman create person test:
![alt text](https://github.com/Seyi007/HNG-crud-api/blob/main/api/images/create_person.png)

- Postman get person test:
![alt text](https://github.com/Seyi007/HNG-crud-api/blob/main/api/images/get_by_id.png)

- Postman update person test:
![alt text](https://github.com/Seyi007/HNG-crud-api/blob/main/api/images/update_person.png)

- Postman delete test:
![alt text](https://github.com/Seyi007/HNG-crud-api/blob/main/api/images/delete_person.png)
## License
MIT License
