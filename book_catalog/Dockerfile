# Use an official Python runtime as a parent image
FROM python:3.12

# Set the working directory in the container
WORKDIR /app

# Copy the requirements file into the container at /app
COPY ./book_catalog/. ./

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Run the application using uvicorn when the container launches
CMD uvicorn main:app --host 0.0.0.0 --port $PORT