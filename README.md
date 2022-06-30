# URL Shortener

### Technology Used
- Python Flask Microframework for the backend.
- React for the frontend.
- Postgres for the database.
- Docker and docker-compose for the setup.

### Folder structure:
- All backend code is in the folder named backend and all frontend code is the folder named frontend.

### Running the Application:

A make file is provided at the root of the repository.
- The setup uses docker and docker-compose, please ensure that you have them setup on your local machine.
- Run "make server" to start the application, this will also in turn run make setup
- The API can be accessed at http://localhost:5000
- The frontend can be accessed at http://localhost:3000
- Run "make test" to run tests
- Run "make clean" to tear down everything.

### API endpoints implemented
- POST /api/v1/shorturl , expects json object with a key url e.g {"url": "https://www.rockethealth.shop/"} and will return a json body with url, shortlink and Slug
- GET /api/v1/shorturl, returns all the the shortlinks
