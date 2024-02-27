# Docker Project Calculator

This is a simple web application built with Docker that provides a calculator interface for performing basic operations.

## Features

- Allows users to input numbers and select an operation (addition, subtraction, multiplication, division).
- Performs the selected operation and displays the result to the user.
- Provides a simple web interface for performing calculations.

## Requirements

- [Install Docker](https://docs.docker.com/get-docker/)
- [Install Docker Compose](https://docs.docker.com/compose/install/)
- [Docker Hub](https://hub.docker.com/)
- [Flask](https://flask.palletsprojects.com/en/3.0.x/)
- [CSS](https://www.w3schools.com/css/)
## Process

1. Created an [app.py](https://github.com/dylpall/docker-project/blob/main/app.py) file which represents the web application using Flask.  
![image](https://github.com/dylpall/docker-project/assets/112408682/942831af-f0f7-4273-a45e-8a79f12f61d9)
* Defines the main Flask application
* Contains route definitions to handle HTTP requests
* Implements the logic of a calculator
---
2. Made a directory called [static](https://github.com/dylpall/docker-project/blob/main/static) which holds a [script.js](https://github.com/dylpall/docker-project/blob/main/static/script.js) file and [styles.css](https://github.com/dylpall/docker-project/blob/main/static/styles.css) file.  
![image](https://github.com/dylpall/docker-project/assets/112408682/238148e0-a3a9-4123-ab70-8c96a9251bca)
* Gives the UI for the calculator presentation and styling
* Specifies the layout, colors, visual effects, etc
* Make it visually appealling and user friendly.
---
3. Made a directory called [templates](https://github.com/dylpall/docker-project/blob/main/templates) which holds an [index.html](https://github.com/dylpall/docker-project/blob/main/templates/index.html) file.  
![image](https://github.com/dylpall/docker-project/assets/112408682/c1f73376-ee37-403a-a3b5-9c9dd73e1659)
* Defines the structure and content of the web page
* Contains HTML elements for user input and displays results.
---
4. The [dockerfile](https://github.com/dylpall/docker-project/blob/main/dockerfile) is the instructions to build the Docker image.  
![image](https://github.com/dylpall/docker-project/assets/112408682/2acd77b9-79bc-44fe-a4c6-90b207e6f09d)
* Specifies a base image to build upon.
* Sets the working directory inside the container.
* Copies files from the host into the container.
---
5. [YAML](https://github.com/dylpall/docker-project/blob/main/docker-compose.yml) File  
![image](https://github.com/dylpall/docker-project/assets/112408682/4e62faee-0f14-4a9b-9649-9400136a94ef)
* Defines a multi-container Docker application using Docker Compose
* Specifies services, networks, and volumes for running the Flask application and any associated services (e.g., database).
* Configures container settings such as ports, environment variables, and volumes mappings.
---
6. [Requirements](https://github.com/dylpall/docker-project/blob/main/requirements.txt) TXT File  
![image](https://github.com/dylpall/docker-project/assets/112408682/dc55c0e2-353c-4b1d-80a8-1a85b3713480)
* Had to use 2.0.2 of Flask and Werkzeug because later versions weren't as compatible and causing HELLA issues. [Link to fix](https://github.com/python-restx/flask-restx/issues/460)
* Ran the requirements.txt file in the `dockerfile` file using PIP
---
## Results

Below is a screenshot of the final outcome of the web page.  
![image](https://github.com/dylpall/docker-project/assets/112408682/1f692b67-758d-4369-b000-c96a187865fe)

https://github.com/dylpall/docker-project/assets/112408682/900b9703-7ba2-4b59-8427-4f3681774774

docker01 configuration
