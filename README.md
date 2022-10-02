# qa_app_test
This is a Q&A model using the following: 

1. pre-trained HuggingFace model
2. FastAPI to expose the endpoints
3. Docker for containerization

How to use:
* Build the docker image based on Dockerfile contents >> `docker build . -t your-image-name`
* Run the container using port 8000 >> `docker run -p 8000:8000 your-image-name`
* To test the endpoints, open the notebook `test.ipynb`. POST a new question to the `get_answer` endpoint.