# Use an official Python runtime as a parent image
FROM python:3.9

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy requirements.txt to the working directory
COPY requirements.txt ./

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code to the working directory
COPY . .

# Expose port 5000 to the outside world
EXPOSE 5000

# Define environment variables (optional, adjust as needed)
ENV FLASK_APP=app.py
ENV FLASK_ENV=production

# Start the application
CMD ["flask", "run", "--host=0.0.0.0"]
# Your Solution
