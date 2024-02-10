# Use a Python image available on Docker Hub
FROM python:3.9

# Set the working directory
WORKDIR /app/back

# Copy the requirements.txt file into the container
COPY ./requirements.txt /app/back/requirements.txt

# Install Python libraries from requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the code into the container
COPY . /app

# Expose the necessary port
EXPOSE 5000

# Command to start the application
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]
