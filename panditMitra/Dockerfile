FROM python:3

# setting work directory    
WORKDIR /usr/src/app

# env variables
ENV PYTHONUNBUFFERED 1
ENV PYTHONDONTWEITEBYTECODE 1

# install dependencies
# RUN pip install --upgrade pip pipenv flake8
# COPY Pipfile* ./
# RUN pipenv install --system --ignore-pipfile

# ADD . /app  

COPY requirements.txt ./

RUN pip install -r requirements.txt

COPY . .

# lint
# RUN flake8 --ignore=E501,F401 .