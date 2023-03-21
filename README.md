# FLASK-app

This is flask app to add the entries in database

# To run locally:

export SQLALCHEMY_DATABASE_URI=<your SQLALCHEMY DATABASE URI >
python main.py

# To Build the docker 

docker build -t my_flask_app --build-arg SQLALCHEMY_DATABASE_URI=your_database_uri -f docker/Dockerfile .

# To run docker build

docker run -e SQLALCHEMY_DATABASE_URI=your_database_uri -p 5000:5000 my_flask_app