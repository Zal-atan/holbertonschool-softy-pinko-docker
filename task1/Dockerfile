# Add latest environment
FROM ubuntu:latest

# Update APT
RUN apt-get update

# Upgrade APT
RUN apt-get upgrade -y

# Download python3
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask

# Working Directory
WORKDIR /app

COPY ./api.py /app/api.py

# Run the program
CMD ["python3", "api.py"]
