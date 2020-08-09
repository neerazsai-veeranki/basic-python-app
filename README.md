app.py is a Basic python app that prints hello world when visited http://localhost:5000

requirements.txt has the required python packages to be installed to get app.py working

Dockerfile 

// this command builds an docker image of pyhton app with name "my-python-app" 

docker build --tag my-python-app ./ 

// this starts a docker container "python-app" with the docker image created in the previous step  in port 5000

docker run --name python-app -p 5000:5000 my-python-app
