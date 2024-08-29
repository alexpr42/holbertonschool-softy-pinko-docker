# Use the latest official Ubuntu image as the base
FROM ubuntu:latest

# Update the package list and upgrade installed software
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Remove the EXTERNALLY-MANAGED file to allow pip installations
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set /app as the working directory
WORKDIR /app

# Copy the api.py file to the Docker image
COPY ./api.py /app/api.py

# Command to run the Flask app
CMD ["python3", "api.py"]
