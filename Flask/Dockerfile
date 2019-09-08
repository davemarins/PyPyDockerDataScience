FROM pypy:3.6-7.1.1

# WORKDIR /app

# install essential package
RUN apt update 
RUN apt install -y libpython3-dev build-essential libpcre3 libpcre3-dev 
RUN apt install -y libssl-dev libffi-dev 

# requirements
COPY ./requirements.txt /requirements.txt
RUN pip install --upgrade pip
RUN pip install --no-cache-dir --ignore-installed -r requirements.txt

# source code
COPY . /app

# run the app
EXPOSE 5000
CMD pypy3 app/server.py
