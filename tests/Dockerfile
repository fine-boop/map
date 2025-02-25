# Use an official Python runtime as a parent image
FROM python:3.11-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install Flask and any other dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port the app runs on
EXPOSE 8000

# Define the environment variable for Flask app
ENV FLASK_APP=app.py

# Run the app when the container starts
CMD ["flask", "run", "--host=0.0.0.0", "--port=8000", "--debug"]
