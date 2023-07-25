
# FROM python:3.8-alpine 
# ## base image

# COPY . /app  
# ## copy all files from current directory to /app directory in container

# WORKDIR /app   
# ## set working directory to /app

# RUN pip install -r requirements.txt 
# ## install all dependencies

# CMD python app.py  
# run app.py file  





FROM python:3.7-alpine  
## base image

WORKDIR /code  
## set working directory to /code

ENV FLASK_APP = app.py  
## set environment variable

ENV FLASK_RUN_HOST =0.0.0.0   
## set environment variable

COPY . . 
 ## copy all files from current directory to /code directory in container

RUN pip install -r reuirements.txt 
 ## install all dependencies

EXPOSE 5000  
 ## expose port 5000

CMD ["flask", "run"]  ## run app.py file

